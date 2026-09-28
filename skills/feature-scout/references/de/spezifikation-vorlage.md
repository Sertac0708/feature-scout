# Vorlage: Nachbau-Spezifikation (Modus 3)

Ziel: eine Beschreibung, nach der man ein Tool mit gleichem **Funktionsumfang** bauen kann.
Funktionen, Abläufe, Felder, Regeln und Formeln vollständig. Texte, Bilder, Logo, Name und
Design nicht kopieren, sondern neutral beschreiben.

**Arbeitsweise:** Das Gerüst mit allen Überschriften sofort anlegen, oben die Statuszeile.
Nach jedem erkundeten Bereich dessen Abschnitt **sofort** füllen. Gesperrtes als
„gesperrt, rekonstruiert aus …" kennzeichnen, Abgeleitetes als „abgeleitet".

```markdown
# Nachbau-Spezifikation: <eigener Arbeitstitel> nach Vorbild <Tool> — <TT.MM.JJJJ>

**Status:** ⏳ In Arbeit — Abschnitt <x> von 7   ← am Ende: ✅ Fertig — <Datum>

## 0. Überblick
- Was die Spezifikation abdeckt (Menüstruktur, Bildschirme, Formulare mit allen Feldern und
  Werten, Kennzahlen mit Formeln, Zustände, Regeln, beobachtete Technik)
- **Erfasst:** Kontostufe (z. B. Free, nicht verifiziert), Anzahl Menüpunkte, Reiter,
  Formulare, Hilfe-Artikel, Changelog-Einträge, Netzwerkanfragen, öffentliche Seiten.
  Alles nur angesehen.
- **Nicht direkt einsehbar (gesperrt):** Liste, und woraus rekonstruiert
- **Grenze für den Nachbau:** Funktionen ja, Texte/Design/Name nein

## 1. Informationsarchitektur und Zugangslogik
### 1.1 Seitenleiste / Navigation
| Gruppe | Menüpunkt | Route | Zugang | Status |
|---|---|---|---|---|
| … | … | /… | frei / 🔒 | ✅ / 🔒 rekonstruiert / ⏭ |
Zusätzliche Routen, versteckte (einblendbare) Menüpunkte, Verhalten der Navigation
(aufklappbar, Hervorhebung, Sperr-Weiterleitung mit Parameter).
### 1.2 Rollen und Zugangsstufen
| Stufe | Wie erreicht | Schaltet frei |
### 1.3 Regeln (Zugang behalten, Fristen, Limits, Neuprüfung)

## 2.–5. Module (ein Abschnitt je Bereich der Navigation)
Für jeden Bildschirm/Reiter:
### <Nr> <Modulname> (<Route>)
- **Aufbau** von oben nach unten (Karten, Blöcke, Leerzustände, Banner)
- **Steuerung:** Filter, Chips, Umschalter, Zeitzonen, Suche
- **Formulare** — je Formular eine Tabelle:
  | Feld | Typ (Text, Zahl, Auswahl, Mehrfachauswahl, Datei, Datum …) | Werte / Optionen | Pflicht / Standard |
- **Auswahllisten vollständig** (z. B. alle Instrumente, alle Gründe, alle Zeitzonen)
- **Kennzahlen:** Tabelle Kennzahl · Definition/Formel · Beispiel aus den angezeigten Zahlen
  (Formeln wenn möglich aus den gezeigten Werten nachrechnen und so kennzeichnen)
- **Zustände:** leer, gesperrt, Fehler, Laden, Erfolg
- **Abläufe:** Schritt für Schritt (abgeleitet, nicht ausgelöst)
- **Benachrichtigungen**, die dieses Modul auslöst
- **Nachbau-Hinweis:** was man besser machen sollte (z. B. Autofill-Sperre, serverseitiger
  Fortschritt)

Typische Gliederung: 2 Dashboard/Onboarding/Konto-Anbindung · 3 Kern-Module · 4 wichtigstes
Modul im Detail · 5 weitere Module, Einstellungen (alle Reiter), Hilfe/Support, Changelog.

## 6. Datenmodell, Technik, Datenquellen
### 6.1 Datenmodell (Vorschlag, aus den Feldern abgeleitet)
| Tabelle | Wichtige Felder |
### 6.2 Beobachtete Technik
Frontend, Hosting, Backend/Datenbank, API-Routen, Karten/Charts, Zahlungen, Push/PWA,
Analyse — nur was im Browser/Netzwerk sichtbar war.
### 6.3 Externe Datenquellen (benötigt)
| Zweck | Beobachtet / Vorschlag |

## 7. Fehler, Lücken, Recht und Bau-Reihenfolge
### 7.1 Gefundene Fehler (beim Nachbau vermeiden)
### 7.2 Nicht einsehbar (und woraus rekonstruiert)
### 7.3 Rechtliche Hinweise (Einschätzung, keine Rechtsberatung)
Was frei nachbaubar ist, was nicht übernommen werden darf, regulatorische Risiken der
Funktionen (z. B. Signale/Empfehlungen, Gesundheitsversprechen), Datenschutz.
### 7.4 Empfohlene Bau-Reihenfolge
| Stufe | Inhalt | Aufwand (klein/mittel/groß) |
```

Prüfen vor „✅ Fertig": Jede Zeile der Tabelle 1.1 hat einen gefüllten Abschnitt oder steht
unter 7.2. Zahlen im Überblick (Menüpunkte, Formulare, Artikel) stimmen mit dem Inhalt.
