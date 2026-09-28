# Rundgang durch die Webseite

## Verbotene Klicks (NIE, auch nicht „nur zum Schauen")
Knöpfe und Links mit diesen Bedeutungen — egal in welcher Sprache — werden nicht angeklickt:

- **Sitzung/Konto:** Abmelden, Logout, Sign out, Konto löschen, Delete account, Passwort
  ändern, Zwei-Faktor, Sitzungen beenden
- **Absenden/Speichern:** Senden, Submit, Speichern, Save, Übernehmen, Apply, Bestätigen,
  Confirm, Veröffentlichen, Publish, Posten, Teilen/Share (mit Versand), Einladen/Invite
- **Geld:** Kaufen, Buy, Bestellen, Checkout, Zur Kasse, Jetzt buchen, Upgrade, Abo
  abschließen, Subscribe, Probezeitraum starten (wenn Zahlungsdaten nötig), Spenden
- **Zerstörend/Ändernd:** Löschen, Delete, Entfernen, Remove, Archivieren, Kündigen, Cancel
  subscription, Zurücksetzen, Reset, Deaktivieren, Import, Upload, Verbinden/Connect (Konten)
- **Anmeldung:** Registrieren, Sign up, Konto erstellen, Login mit Google/Apple/…, Newsletter
  eintragen, Kontaktformular abschicken, Demo buchen, Rückruf anfordern
- **Einstellungen:** Seiten unter „Einstellungen/Settings/Konto/Billing/Team" dürfen
  angeschaut werden, aber dort nichts umschalten, auswählen oder eintippen.

Im Zweifel: **nicht klicken**, im Bericht „nicht geprüft, weil Aktion nötig" vermerken.
Anmelde- und Kaufformulare dürfen *angesehen* werden (welche Felder, welche Schritte) —
ausgefüllt oder abgeschickt wird nichts.

Cookie-Banner: „Ablehnen" / „Nur notwendige" wählen, nie „Alle akzeptieren".
Pop-ups (Newsletter, Chat-Widgets): schließen, nicht ausfüllen.

## Eingeloggtes Tool / Dashboard (Hauptfall)

**Zusätzlich verboten im Tool** (weil es das echte Konto des Nutzers ist):
- Schalter/Toggles umlegen, Häkchen setzen, Auswahl in Einstellungen oder Formularen treffen
  (viele Tools speichern sofort automatisch)
- in Felder tippen (auch nicht „nur zum Testen"), Dateien hochladen, Ziehen & Ablegen
- **Guthaben- oder Kosten-Aktionen:** Generieren, Erstellen, Starten, Ausführen, Run,
  Analyse starten, Export, Senden, Test-Mail, Veröffentlichen
- Einladungen, Team-Änderungen, Rollen, API-Schlüssel erzeugen oder anzeigen lassen
- Abrechnung: Tarif wechseln, Zahlungsart, Kündigen

**Erlaubt:** Menüpunkte und Reiter öffnen, Listen und Detailansichten ansehen, Dropdowns
**aufklappen** um Optionen zu lesen (dann mit Esc schließen), Tooltips/Info-Symbole lesen,
„Neu anlegen"-Dialoge öffnen um die Felder zu sehen und **mit Abbrechen/✕/Esc schließen**,
reine Ansichts-Filter in Listen/Berichten (Zeitraum, Sortierung), Hilfe-Center lesen.

**Menükarte zuerst:** Bevor tiefer geklickt wird, die komplette Navigation erfassen:
```
Hauptmenü
├── Menüpunkt 1  → Unterpunkte / Reiter
├── Menüpunkt 2  → …
├── „+ Neu"-Menü → welche Dinge man anlegen kann
├── Konto-Menü   → Profil, Team, Abrechnung, Einstellungen (NICHT Abmelden)
└── Hilfe        → Doku, Chat, Tutorials
```

**Pro Bildschirm festhalten:**
```
Bildschirm / URL:
Zweck:
Sichtbare Funktionen und Knöpfe (nicht ausgelöst):
Felder / Optionen (aus Dialogen, Dropdowns):
Leerzustand / Einführungs-Hinweise:
Gesperrt / „Pro" / Upsell:
So funktioniert es (abgeleitete Schritte):
Auffällig (gut / schlecht, Bedienung):
```

**Typische Bereiche eines Tools** (alle ansehen, wenn vorhanden): Dashboard/Übersicht,
Kernobjekte (Projekte, Kampagnen, Kunden, Dokumente …), Anlegen/Editor, Vorlagen,
Automatisierungen/Workflows, Berichte/Statistiken, Integrationen/Apps, Team & Rollen,
Einstellungen, Abrechnung/Tarife & Limits, Benachrichtigungen, Hilfe/Onboarding.

Nach dem Tool nur noch die öffentlichen Seiten **Preise**, **Funktionen** und
**Integrationen** ergänzen (was kostet welcher Umfang, was bewerben sie).

## Reihenfolge und Seitentypen (Vorrang von oben nach unten)

| Seitentyp | Woran erkennbar | Was notieren |
|---|---|---|
| Startseite | Domain-Wurzel | Hauptversprechen, Zielgruppe, Handlungsaufforderung, Menüstruktur |
| Funktionen / Produkt | „Features", „Produkt", „Funktionen", „Leistungen" | jede Funktion + wie sie funktioniert |
| Preise | „Preise", „Pricing", „Pakete", „Tarife" | Pakete, Preise, Grenzen, Testphase, Zahlweise |
| Lösungen / Anwendungsfälle | „Lösungen", „Für wen", „Branchen", „Use cases" | Zielgruppen, Beispiele |
| So funktioniert's | „So geht's", „How it works", „Ablauf" | Schritte der Nutzerreise |
| Integrationen / Schnittstellen | „Integrationen", „API", „Apps", „Partner" | angebundene Dienste |
| Hilfe / FAQ / Doku | „Hilfe", „FAQ", „Support", „Docs" | versteckte Funktionen, Einschränkungen, Häufige Fragen |
| Über uns / Vertrauen | „Über uns", „Referenzen", „Bewertungen" | Firma, Größe, Belege, Siegel |
| Anmeldung / Konto (nur ansehen) | „Login", „Registrieren", „Start" | welche Daten, wie viele Schritte, Anmeldearten |
| App-Bereich (falls eingeloggt) | `app.`, „Dashboard" | Menüpunkte, Kernfunktionen, Bedienung |
| Blog / Ratgeber (Stichprobe) | „Blog", „Magazin" | Themen, SEO-Strategie (2–3 Beispiele) |
| Rechtliches (überfliegen) | Impressum, AGB, Datenschutz | Firma/Sitz, auffällige Klauseln, eingesetzte Dienste |

Zusätzlich, wenn schnell möglich: `/sitemap.xml` ansehen (zeigt den Umfang der Seite) —
nur lesen, nicht jede Adresse daraus besuchen.

## Was pro Seite festhalten (kurz, Stichworte)
```
URL:
Zweck der Seite:
Funktionen / Angebote:
So funktioniert es (Schritte):
Preise / Grenzen:
Auffällig (gut / schlecht):
Handlungsaufforderung:
```

## Regeln für Links
- Nur dieselbe Domain und ihre Unterdomains. Externe Links nur notieren (z. B. „nutzt
  Stripe", „Hilfe läuft über Zendesk"), nicht besuchen.
- Keine Dateien herunterladen (PDF, ZIP, Apps). PDF-Titel notieren reicht.
- Links mit Parametern, die etwas auslösen (`?action=`, `/delete`, `/logout`, `/unsubscribe`,
  `/cancel`), nicht öffnen.
- Endlos-Listen (Filter, Suche, Paginierung) nicht durchblättern — erste Seite reicht.

## Schluss des Rundgangs
Nach ca. 30 Seiten oder wenn alle Seitentypen abgedeckt sind. Liste der besuchten Seiten
behalten — sie kommt in den Bericht. Bereiche, die offen blieben, benennen.
