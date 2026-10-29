# Übungen

Alle Übungen arbeiten mit den Unterlagen im Ordner `fall/`. Sie beschreiben einen erfundenen Fall: Ein Servicebereich will ein internes Wissensportal beschaffen, zwei Anbieter haben Angebote abgegeben. Die Datei im Ordner `spaeter/` öffnen Sie erst, wenn die Kursleitung dazu auffordert.

| Datei | Inhalt |
|---|---|
| `S01-projektauftrag.docx` | Projektauftrag: Ziel, Umfang, Budget, Termin |
| `S02-besprechungsnotiz.docx` | Notiz aus einer Besprechung |
| `S03-angebot-a.pdf` | Angebot Anbieter A |
| `S04-angebot-b.pdf` | Angebot Anbieter B |
| `S05-kriterien.xlsx` | Kriterienliste für die Auswahl |
| `S07-rahmenvertrag-b.pdf` | Vertragsentwurf von Anbieter B, rund 25 Seiten |

Prompts in Schreibmaschinenschrift können Sie kopieren und anpassen. Bei Aufgaben mit **Tipp vorab** schreiben Sie Ihre Vermutung in den Teams-Chat, bevor Sie Claude fragen. Danach vergleichen Sie.

---

## Lab 0 · Anmelden und Unterlagen laden

1. Öffnen Sie claude.ai im Browser und melden Sie sich mit Ihrem Firmenkonto an.
2. Öffnen Sie die Seite des Übungsrepositorys (Link im Teams-Chat). Wählen Sie **Code** → **Download ZIP** und entpacken Sie die Datei.
3. Starten Sie einen neuen Chat. Suchen Sie die Schaltfläche zum Anhängen von Dateien und die Schalter für Websuche und Research.
4. Hängen Sie `S01-projektauftrag.docx` an und fragen Sie:

   `Worum geht es in diesem Dokument? Antworte in einem Satz.`

Fertig, wenn: Claude den Inhalt von S01 in einem Satz wiedergibt.

---

## Lab 1 · Erstes Briefing

1. Neuer Chat. Hängen Sie S01 und S02 an.
2. **Tipp vorab:** Welche Kontenzahl wird im Briefing stehen?
3. Fragen Sie:

   `Fasse die beiden Dokumente in einem kurzen Briefing für die Bereichsleitung zusammen.`

4. Lesen Sie das Briefing. Welche Zahl für die Konten steht darin, und aus welchem Dokument stammt sie? Prüfen Sie eine Zahl im Original nach.
5. Fragen Sie im selben Chat:

   `Welche Angaben in S01 und S02 widersprechen sich? Nenne zu jeder Angabe Dokument und Abschnitt.`

Fertig, wenn: Sie wissen, ob das erste Briefing einen Widerspruch zwischen den Dokumenten erwähnt hat, und eine Angabe im Original geprüft haben.

---

## Lab 2 · Einen Auftrag schärfen

1. Neuer Chat mit S01 und S02. Fragen Sie:

   `Was muss die Projektleitung jetzt tun?`

2. Neuer Chat mit denselben Dateien. Fragen Sie:

   ```
   Rolle: Assistenz der Projektleitung bei einer Beschaffung.
   Ziel: Die Projektleitung soll vor Ablauf der Angebotsfrist wissen, was sie entscheiden oder veranlassen muss.
   Kontext: S01 ist der freigegebene Auftrag. S02 ist eine Arbeitsnotiz ohne Änderungsfreigabe.
   Ausgabe: Tabelle mit den Spalten Aufgabe, Wer, Bis wann, Quelle (Dokument und Abschnitt).
   Kriterien: Nur Aufgaben, die sich aus den Dokumenten ergeben. Jede Zeile mit Quelle. Was offen ist, steht als offen da.
   ```

3. **Tipp vorab:** Welche der beiden Antworten enthält mehr Aufgaben, die in keinem der Dokumente stehen?
4. Vergleichen Sie beide Antworten mit Ihrer Partnerin oder Ihrem Partner im Breakout-Raum. Streichen Sie in der ersten Antwort alles, was sich nicht auf die Dokumente zurückführen lässt.

Fertig, wenn: Sie benennen können, welche Zeile des zweiten Auftrags den größten Unterschied gemacht hat.

---

## Lab 3 · Eine Prompt-Vorlage bauen

1. Öffnen Sie `prompt-vorlagen.md` und wählen Sie die Vorlage **Angebot zusammenfassen**, oder schreiben Sie eine eigene mit Platzhaltern in eckigen Klammern.
2. Neuer Chat mit S03. Setzen Sie die Platzhalter ein und schicken Sie die Vorlage ab.
3. **Tipp vorab:** Funktioniert dieselbe Vorlage für S04 ohne Änderung?
4. Neuer Chat mit S04, dieselbe Vorlage. Vergleichen Sie: Fehlt im Ergebnis etwas, das für die Entscheidung wichtig ist?
5. Ändern Sie die Vorlage so, dass sie für beide Angebote trägt. Speichern Sie sie in Ihrer eigenen Prompt-Bibliothek (eine Textdatei oder ein Dokument reicht).

Fertig, wenn: Ihre Vorlage für beide Angebote ein vollständiges Ergebnis liefert und gespeichert ist.

---

## Lab 4 · Marktübersicht mit Websuche

1. Neuer Chat, Websuche einschalten. Fragen Sie:

   ```
   Recherchiere Software für interne Wissensportale, die Service-Teams im deutschsprachigen Raum nutzen.
   Erstelle eine Tabelle mit 5 Anbietern: Name, Hosting-Region, Exportformate für Artikel, Quelle (Link).
   Nenne danach 5 Fragen, die ein Einkauf vor der Beschaffung an jeden Anbieter stellen sollte.
   Kennzeichne jede Angabe, für die keine Quelle vorliegt.
   ```

2. **Tipp vorab:** Sie prüfen gleich drei Angaben aus der Tabelle. Wie viele davon stehen genau so in der verlinkten Quelle?
3. Wählen Sie drei Angaben, öffnen Sie jeweils den Link und suchen Sie die Stelle. Notieren Sie: steht dort, steht dort anders, steht dort nicht.
4. Kür: Stellen Sie dieselbe Frage mit **Research** und vergleichen Sie Umfang und Quellen.

Fertig, wenn: Sie für drei Angaben das Ergebnis Ihrer Prüfung notiert haben.

---

## Lab 5 · Angebote vergleichen und einen Vertrag auswerten

**Teil A: Vergleich**

1. Neuer Chat mit S01, S03, S04 und S05. Fragen Sie:

   ```
   Vergleiche die Angebote S03 und S04 anhand der Kriterien in S05.
   Ausgabe: Tabelle mit einer Zeile je Kriterium, Spalten Anbieter A, Anbieter B, Fundstelle.
   Rechne danach die Kosten für Einrichtung und zwölf Nutzungsmonate für 24 und für 30 Konten, mit Rechenweg.
   ```

2. **Tipp vorab:** Welchen Betrag nennt Claude für Anbieter B bei 30 Konten?
3. Rechnen Sie den Betrag für Anbieter B bei 30 Konten selbst nach, mit den Preisen aus S04. Stimmt er?

**Teil B: Vertrag**

4. Neuer Chat mit S07. Fragen Sie:

   ```
   Werte den Vertragsentwurf für den Auftraggeber aus.
   Liste getrennt: Risiken, Aufgaben des Auftraggebers mit Frist, Entscheidungen vor der Unterschrift.
   Nenne zu jedem Punkt den Paragraphen oder die Anlage.
   ```

5. Hängen Sie S04 an und fragen Sie: `Weicht der Vertragsentwurf beim Export vom Angebot S04 ab? Zitiere beide Stellen.`
6. Prüfen Sie zwei Fundstellen im PDF nach.

Fertig, wenn: Ihr Kostenbetrag für B bei 30 Konten nachgerechnet ist und Sie zwei Fundstellen aus S07 im Original gefunden haben.

---

## Lab 6 · Ergebnisse in andere Formate bringen

Arbeiten Sie im Chat von Lab 5 Teil A weiter.

1. **Tipp vorab:** Was geht verloren, wenn Claude den Vergleich auf fünf Sätze kürzt?
2. Fragen Sie: `Schreibe eine Management-Zusammenfassung des Vergleichs in höchstens fünf Sätzen.`
3. Legen Sie die Zusammenfassung neben die Tabelle. Welche Bedingung oder Einschränkung fehlt?
4. Fragen Sie: `Schreibe eine E-Mail an Anbieter B mit den Fragen, die vor einer Entscheidung beantwortet sein müssen.`
5. Fragen Sie: `Erstelle eine PowerPoint-Datei mit drei Folien: Ausgangslage, Vergleich, offene Punkte.` Laden Sie die Datei herunter und öffnen Sie sie.

Fertig, wenn: Sie eine fehlende Bedingung benennen können und die PowerPoint-Datei geöffnet haben.

---

## Lab 7 · Project mit LLM Wiki

1. Legen Sie ein Project „Wissensportal Service“ an. Laden Sie S01 bis S05 und S07 in das Projektwissen.
2. Tragen Sie als Project Instructions ein:

   ```
   Rolle: Assistenz der Projektleitung bei der Beschaffung eines Wissensportals.
   Die Dokumente S01 bis S07 sind Originale und werden nie verändert.
   Jede Aussage zu Zahlen, Terminen und Zusagen nennt Dokument und Abschnitt.
   Eine interne Notiz ändert keine Anbieterzusage.
   Offene Punkte stehen als offen da.
   ```

3. Starten Sie im Project einen Chat und fragen Sie:

   `Erstelle aus den Projektdokumenten eine Wiki nach der Vorlage in wiki-vorlage.md, Version v1. Erstelle sie als Artifact.`

   (Hängen Sie `wiki-vorlage.md` an.) Prüfen Sie zwei Zahlen am Original. Speichern Sie die Wiki und laden Sie sie als `wiki-v1.md` ins Projektwissen.
4. Jetzt gibt die Kursleitung `spaeter/S06-aenderung.pdf` frei. **Tipp vorab:** Kann nach S06 noch einer der beiden Anbieter den Pilottermin halten?
5. Hängen Sie S06 an und fragen Sie:

   `Arbeite S06 in die Wiki ein: Version v2. Markiere ersetzte Angaben, ergänze das Änderungslog und prüfe die Anbietertermine gegen den neuen Bedarf.`

6. Fragen Sie: `Erstelle aus der Wiki v2 eine Entscheidungsvorlage für die Projektleitung als Artifact. Keine Bestellung, nur Empfehlung und offene Fragen.`

Fertig, wenn: Wiki v2 die neue Kontenzahl und den neuen Termin überall gleich nennt, das Log S06 nennt und die Entscheidungsvorlage keine Anbieterantwort erfindet.

---

## Lab 8 · Praxisworkshop mit eigener Aufgabe

Nehmen Sie eine Aufgabe aus Ihrem Arbeitsalltag, ohne vertrauliche Daten. Wer keine hat, erstellt aus S01 und S03 eine FAQ für die Pilotgruppe.

1. Schreiben Sie den Auftrag mit Ziel, Kontext, Ausgabe und Kriterien, oder nehmen Sie eine Vorlage aus Ihrer Prompt-Bibliothek.
2. Lassen Sie das Ergebnis als Artifact oder als Datei erstellen und verbessern Sie es in zwei Schritten.
3. Prüfen Sie es mit `pruefcheckliste.md`. Lassen Sie es im Breakout-Raum von einer zweiten Person gegenlesen.
4. Speichern Sie den Auftrag als Vorlage in Ihrer Prompt-Bibliothek.

Fertig, wenn: Ergebnis und Vorlage gespeichert sind und Sie einen Punkt aus der Checkliste nennen können, an dem Sie nachbessern mussten.
