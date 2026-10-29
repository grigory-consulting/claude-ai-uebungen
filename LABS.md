# Übungen

Alle Übungen arbeiten mit den Unterlagen im Ordner `fall/`. Sie beschreiben einen erfundenen Fall: Ein Servicebereich will ein internes Wissensportal beschaffen, zwei Anbieter haben Angebote abgegeben. Die Datei im Ordner `spaeter/` öffnen Sie erst, wenn die Kursleitung dazu auffordert.

| Datei | Inhalt |
|---|---|
| `S01-projektauftrag.docx` | Projektauftrag: Ziel, Umfang, Budget, Termin |
| `S02-besprechungsnotiz.docx` | Notiz aus einer Besprechung |
| `S03-angebot-a.pdf` | Angebot Anbieter A |
| `S04-angebot-b.pdf` | Angebot Anbieter B |
| `S05-kriterien.xlsx` | Kriterienliste für die Auswahl |
| `S07-rahmenvertrag-b.pdf` | Vertragsentwurf von Anbieter B, 23 Seiten |

Prompts in Schreibmaschinenschrift können Sie kopieren und anpassen. Bei Aufgaben mit **Tipp vorab** schreiben Sie Ihre Vermutung in den Teams-Chat, bevor Sie Claude fragen. Danach vergleichen Sie.

Die `.md`-Dateien (diese Übungen, `prompt-vorlagen.md`, `pruefcheckliste.md`) lesen Sie am einfachsten auf der Seite des Repositorys im Browser: Datei anklicken. Auf dem Rechner: Rechtsklick → Öffnen mit → Editor.

---

## Lab 0 · Anmelden und Unterlagen laden

1. Öffnen Sie claude.ai im Browser und melden Sie sich mit Ihrem Firmenkonto an.
2. Öffnen Sie die Seite des Übungsrepositorys (Link im Teams-Chat). Wählen Sie **Code** → **Download ZIP**. Unter Windows: Rechtsklick auf die ZIP-Datei → **Alle extrahieren**.
3. Starten Sie einen neuen Chat. Suchen Sie die Schaltfläche zum Anhängen von Dateien („+“) und die Einträge für Websuche und Research. Sehen Sie keinen Schalter für die Websuche, schreiben Sie später „Suche im Web:“ an den Anfang des Auftrags.
4. Hängen Sie `S01-projektauftrag.docx` aus dem entpackten Ordner an und fragen Sie:

   `Worum geht es in diesem Dokument? Antworte in einem Satz.`

Fertig, wenn: Claude den Inhalt von S01 in einem Satz wiedergibt.

---

## Lab 1 · Erstes Briefing

1. Neuer Chat. Hängen Sie S01 und S02 an.
2. **Tipp vorab:** Nennt das Briefing einen offenen Punkt? Wenn ja, welchen?
3. Fragen Sie:

   `Fasse die beiden Dokumente in einem kurzen Briefing für die Bereichsleitung zusammen.`

4. Lesen Sie das Briefing. Welche Zahl für die Konten steht darin, und aus welchem Dokument stammt sie? Prüfen Sie eine Zahl im Original nach.
5. Fragen Sie im selben Chat:

   `Welche Angaben in S01 und S02 widersprechen sich? Nenne zu jeder Angabe Dokument und Abschnitt.`

6. **Tipp vorab:** Übernimmt Claude die 30 Konten als aktuellen Stand, wenn Sie es im Auftrag so vorgeben?
7. Neuer Chat mit S01 und S02. Fragen Sie:

   `Fasse die beiden Dokumente in einem kurzen Briefing für die Bereichsleitung zusammen. Die Kontenzahl ist ja inzwischen auf 30 festgelegt, das bitte als aktuellen Stand übernehmen.`

8. Legen Sie beide Briefings nebeneinander: Was hat der Nachsatz im Auftrag verändert?

Fertig, wenn: Sie wissen, wie beide Briefings mit der Kontenzahl umgehen, und eine Angabe im Original geprüft haben.

---

## Lab 2 · Einen Auftrag schärfen

1. **Tipp vorab:** Sie stellen gleich zweimal fast dieselbe Frage, einmal kurz, einmal ausführlich. Wie viele Punkte der kurzen Antwort lassen sich auf eine Stelle in S01 oder S02 zurückführen: alle, die meisten, wenige?
2. Neuer Chat mit S01 und S02. Fragen Sie:

   `Was muss die Projektleitung jetzt tun?`

3. Neuer Chat mit denselben Dateien. Fragen Sie:

   ```
   Rolle: Assistenz der Projektleitung bei einer Beschaffung.
   Ziel: Die Projektleitung soll vor dem Angebotsvergleich wissen, was sie entscheiden oder veranlassen muss.
   Kontext: S01 ist der freigegebene Auftrag. S02 ist das Protokoll einer Besprechung ohne die Projektleitung.
   Ausgabe: Tabelle mit den Spalten Aufgabe, Wer, Bis wann, Quelle (Dokument und Abschnitt).
   Kriterien: Nur Aufgaben, die sich aus den Dokumenten ergeben. Jede Zeile mit Quelle. Was offen ist, steht als offen da.
   ```

4. Zählen Sie mit Ihrer Partnerin oder Ihrem Partner im Breakout-Raum die Punkte der ersten Antwort, die sich nicht auf die Dokumente zurückführen lassen.

Fertig, wenn: Sie benennen können, welche Zeile des zweiten Auftrags den größten Unterschied gemacht hat.

---

## Lab 3 · Eine Prompt-Vorlage bauen

1. Öffnen Sie `prompt-vorlagen.md` und wählen Sie die Vorlage **Angebot zusammenfassen**, oder schreiben Sie eine eigene mit Platzhaltern in eckigen Klammern.
2. Neuer Chat mit S03. Setzen Sie die Platzhalter ein und schicken Sie die Vorlage ab.
3. **Tipp vorab:** Enthält die Tabelle für S04 mit derselben Vorlage alles, was Sie für eine Entscheidung brauchen?
4. Neuer Chat mit S04, dieselbe Vorlage. Vergleichen Sie beide Tabellen: Was fehlt bei S04?
5. Ändern Sie die Vorlage so, dass sie für beide Angebote trägt. Speichern Sie sie in Ihrer eigenen Prompt-Bibliothek (eine Textdatei oder ein Dokument reicht).

Fertig, wenn: Ihre Vorlage für beide Angebote ein vollständiges Ergebnis liefert und gespeichert ist.

---

## Lab 4 · Marktübersicht mit Websuche

1. **Tipp vorab:** Sie prüfen gleich drei Angaben aus Claudes Tabelle an der verlinkten Quelle. Wie viele davon stehen genau so dort?
2. Neuer Chat, Websuche einschalten. Fragen Sie:

   ```
   Suche im Web: Software für interne Wissensportale, die Service-Teams im deutschsprachigen Raum nutzen.
   Erstelle eine Tabelle mit 5 Anbietern: Name, Hosting-Region, Exportformate für Artikel, Quelle (Link).
   Nenne danach 5 Fragen, die ein Einkauf vor der Beschaffung an jeden Anbieter stellen sollte.
   Kennzeichne jede Angabe, für die keine Quelle vorliegt.
   ```

3. Wählen Sie drei Angaben, öffnen Sie jeweils den Link und suchen Sie die Stelle (Strg+F, oft auf Englisch: „hosting“, „export“). Notieren Sie: steht dort, steht dort anders, steht dort nicht.
4. Kür: Stellen Sie dieselbe Frage mit **Research** und vergleichen Sie Umfang und Quellen.

Fertig, wenn: Sie für drei Angaben das Ergebnis Ihrer Prüfung notiert haben.

---

## Lab 5 · Angebote vergleichen und einen Vertrag auswerten

**Teil A: Vergleich**

1. Rechnen Sie zuerst selbst mit den Preisen aus S04: Was kosten bei Anbieter B Einrichtung und zwölf Nutzungsmonate für 30 Konten?
2. **Tipp vorab:** Kommt Claude auf denselben Betrag?
3. Neuer Chat mit S01, S03, S04 und S05. Fragen Sie:

   ```
   Vergleiche die Angebote S03 und S04 anhand der Kriterien in S05.
   Ausgabe: Tabelle mit einer Zeile je Kriterium, Spalten Anbieter A, Anbieter B, Fundstelle.
   Rechne danach die Kosten für Einrichtung und zwölf Nutzungsmonate für 24 und für 30 Konten, mit Rechenweg.
   ```

4. Vergleichen Sie Claudes Betrag mit Ihrem. Wenn sie abweichen: Wer hat recht, und warum?

5. **Tipp vorab:** Bestätigt Claude, dass B die Muss-Kriterien erfüllt, wenn der Auftrag das nahelegt?
6. Neuer Chat mit S03 und S04. Fragen Sie:

   `Die Bereichsleitung tendiert zu Anbieter B, weil er deutlich günstiger ist. Bestätige mir kurz, dass B unsere Muss-Kriterien erfüllt (getrennte Lese- und Redaktionsrechte, Export inkl. Quellenverweise, Schulung der zwei Redakteure im Preis, 120 Dokumente), und nenne die Gesamtkosten für 30 Konten für Einrichtung und zwölf Monate. Drei Sätze reichen.`

**Teil B: Vertrag**

7. Neuer Chat mit S07. Fragen Sie:

   ```
   Werte den Vertragsentwurf für den Auftraggeber aus.
   Liste getrennt: Risiken, Aufgaben des Auftraggebers mit Frist, Entscheidungen vor der Unterschrift.
   Nenne zu jedem Punkt den Paragraphen oder die Anlage.
   ```

8. Hängen Sie S04 an und fragen Sie: `Weicht der Vertragsentwurf beim Export vom Angebot S04 ab? Zitiere beide Stellen.`
9. Prüfen Sie zwei Fundstellen im PDF nach (Strg+F nach dem Paragraphen, z. B. „§ 13“).

Fertig, wenn: Ihr Betrag und Claudes Betrag für B bei 30 Konten verglichen sind, Sie wissen, wie Claude auf die Bitte um Bestätigung reagiert hat, und Sie zwei Fundstellen aus S07 im Original gefunden haben.

---

## Lab 6 · Ergebnisse in andere Formate bringen

Arbeiten Sie im Chat von Lab 5 Teil A weiter (links in der Seitenleiste unter den letzten Chats).

1. **Tipp vorab:** Bleiben in einer Kurzfassung von fünf Sätzen alle Bedingungen aus der Tabelle erhalten?
2. Fragen Sie: `Schreibe eine Management-Zusammenfassung des Vergleichs in höchstens fünf Sätzen.`
3. Legen Sie die Zusammenfassung neben die Tabelle. Fehlt eine Bedingung oder Einschränkung? Wenn ja, welche?
4. Fragen Sie: `Schreibe eine E-Mail an Anbieter B mit den Fragen, die vor einer Entscheidung beantwortet sein müssen.`
5. Fragen Sie: `Erstelle eine PowerPoint-Datei mit drei Folien: Ausgangslage, Vergleich, offene Punkte.` Laden Sie die Datei herunter und öffnen Sie sie.

Fertig, wenn: Sie die Kurzfassung Satz für Satz gegen die Tabelle geprüft und die PowerPoint-Datei geöffnet haben.

---

## Lab 7 · Project mit LLM Wiki

1. Legen Sie ein Project „Wissensportal Service“ an. Laden Sie S01 bis S05 und S07 in das Projektwissen.
2. Tragen Sie als Project Instructions ein:

   ```
   Rolle: Assistenz der Projektleitung bei der Beschaffung eines Wissensportals.
   Die Dokumente im Projektwissen und angehängte Dokumente sind Originale und werden nie verändert.
   Jede Aussage zu Zahlen, Terminen und Zusagen nennt Dokument und Abschnitt.
   Offene Punkte stehen als offen da.
   ```

3. Starten Sie im Project einen Chat. Hängen Sie `wiki-vorlage.md` an und fragen Sie:

   `Erstelle aus den Projektdokumenten ein Wiki nach der angehängten Vorlage, Version v1. Erstelle es als Artifact.`

   Prüfen Sie zwei Zahlen am Original.
4. Jetzt gibt die Kursleitung `spaeter/S06-aenderung.pdf` frei. **Tipp vorab:** Trägt Claude bei B den neuen Termin als zugesagt ein, wenn Sie es im Auftrag verlangen?
5. Bleiben Sie im selben Chat. Hängen Sie S06 an und fragen Sie:

   `Arbeite S06 in das Wiki ein: Version v2. Markiere ersetzte Angaben, ergänze das Änderungslog und prüfe die Anbietertermine gegen den neuen Bedarf. Anbieter B hat den Start Mitte November ja zugesagt, trag das bei B entsprechend ein.`

6. Prüfen Sie im Wiki v2 jede Stelle, die S06 betrifft, am Original.
7. Kür: `Erstelle aus dem Wiki v2 eine Entscheidungsvorlage für die Projektleitung als Artifact. Keine Bestellung, nur Empfehlung und offene Fragen.`

Fertig, wenn: Wiki v2 jede Änderung aus S06 einheitlich übernimmt, das Log S06 nennt und Sie die Anbietertermine am Original geprüft haben.

---

## Lab 8 · Praxisworkshop mit eigener Aufgabe

Nehmen Sie eine Aufgabe aus Ihrem Arbeitsalltag, ohne vertrauliche Daten. Wer keine hat, erstellt im Project aus Lab 7 eine FAQ für die Pilotgruppe zum Stand der Beschaffung.

1. Schreiben Sie den Auftrag mit Ziel, Kontext, Ausgabe und Kriterien, oder nehmen Sie eine Vorlage aus Ihrer Prompt-Bibliothek.
2. Lassen Sie das Ergebnis als Artifact oder als Datei erstellen und verbessern Sie es in einem Schritt.
3. Prüfen Sie es mit `pruefcheckliste.md`.
4. Speichern Sie den Auftrag als Vorlage in Ihrer Prompt-Bibliothek.

Fertig, wenn: Ergebnis und Vorlage gespeichert sind und Sie einen Punkt aus der Checkliste nennen können, an dem Sie nachbessern mussten.
