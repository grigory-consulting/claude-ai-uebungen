# Prompt-Vorlagen

Startsammlung für Ihre eigene Prompt-Bibliothek. Begriffe in eckigen Klammern ersetzen Sie vor dem Absenden. Passen Sie jede Vorlage an Ihre Aufgaben an und notieren Sie, was Sie geändert haben.

## Aufbau eines Auftrags

```
Rolle: [aus welcher Sicht Claude arbeitet]
Ziel: [wofür das Ergebnis gebraucht wird, von wem]
Kontext: [Dokumente, Stand, was schon entschieden ist]
Ausgabe: [Format, Länge, Gliederung, Dateityp]
Kriterien: [woran Sie ein gutes Ergebnis erkennen]
```

## Briefing aus Dokumenten

```
Fasse die angehängten Dokumente als Briefing für [Zielgruppe] zusammen.
Ziel: [Entscheidung oder Termin, für den das Briefing gebraucht wird]
Ausgabe: höchstens [Anzahl] Stichpunkte, danach eine Liste offener Punkte.
Kriterien: Jede Zahl und jeder Termin mit Dokument und Abschnitt. Widersprüche zwischen den Dokumenten ausdrücklich nennen.
```

## Angebot zusammenfassen (Startfassung)

```
Fasse das angehängte Angebot für [Zielgruppe] zusammen.
Ausgabe: Tabelle mit den Zeilen Leistung, Preis, Termin, Export enthalten (ja/nein).
Kriterien: Nur Angaben aus dem Angebot, jede mit Abschnitt.
```

## Dokumente vergleichen

```
Vergleiche [Dokument A] und [Dokument B] anhand von [Kriterienliste oder Prüffragen].
Ausgabe: Tabelle mit einer Zeile je Kriterium, Spalten [A], [B], Fundstelle.
Kriterien: Unterschiede und fehlende Angaben markieren. Keine Bewertung ohne Beleg. Rechnungen mit Rechenweg.
```

## Rechercheauftrag

```
Recherchiere [Frage] für [Region, Zeitraum].
Quellen: bevorzugt [Herstellerseiten, Behörden, Fachverbände], keine Vergleichsportale.
Ausgabe: Tabelle [Spalten] mit Link je Zeile, danach offene Fragen.
Kriterien: Angaben ohne Quelle kennzeichnen. Datum der Quelle nennen, wenn es sichtbar ist.
```

## Langes Dokument auswerten

```
Werte das angehängte Dokument für [Rolle] aus.
Liste getrennt: Risiken, Aufgaben mit Frist, Entscheidungen.
Kriterien: Zu jedem Punkt Abschnitt oder Seite. Wörtliche Zitate nur bei Fristen und Beträgen.
```

## E-Mail aus einem Ergebnis

```
Schreibe eine E-Mail an [Empfänger] zu [Anlass].
Ziel: [Antwort oder Entscheidung, die Sie brauchen, bis wann]
Inhalt: [Punkte aus dem Ergebnis]
Ton: sachlich, Anrede „Sehr geehrte …“, höchstens [Anzahl] Sätze, Fragen nummeriert.
```

## Ergebnis prüfen lassen

```
Prüfe das folgende Ergebnis gegen die angehängten Originale.
Liste jede Aussage, die so nicht in den Originalen steht, und jede Zahl, die sich nicht nachrechnen lässt.
```
