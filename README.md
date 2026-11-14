# Einrichten von Claude Code

> Vorbereitung für das Seminar «Claude Code für Einsteiger», HWZ, Durchführung 25./26.11.2026. Version 0.3.0, Stand 14.11.2026.

Für das Seminar brauchst Du vier Dinge:

1. einen eigenen Laptop mit Installationsrechten
2. ein Claude-Pro-Abo
3. Claude Code, installiert und angemeldet
4. die Editoren Obsidian und Visual Studio Code

Die Vorbereitung dauert ca. 30 Minuten. Erledige sie bis spätestens **Dienstag, 24.11.2026**.

**Die Reihenfolge ist zwingend:** Zuerst das Abo, danach Claude Code installieren. Die Anmeldung in Claude Code funktioniert nur mit einem bezahlten Konto.

## Schritt 1: Laptop bereitstellen

Bring einen **privaten Laptop** mit macOS 13 oder neuer oder Windows 10 (Version 1809) oder neuer mit. Auf Firmengeräten sind Installationen und das Terminal häufig gesperrt, und Internetdienste können blockiert sein. Tablets und Chromebooks funktionieren nicht.

## Schritt 2: Claude Pro abonnieren

Claude Code ist im kostenlosen Claude-Konto nicht enthalten. Es braucht mindestens **Claude Pro**.

1. Öffne https://claude.ai und melde Dich an oder erstelle ein Konto.
2. Wähle **Upgrade** und das Abo **Pro** mit monatlicher Zahlung (USD 20 pro Monat, monatlich kündbar). Das Jahresabo lohnt sich für das Seminar nicht.
3. Schliesse das Abo frühestens eine Woche vor dem Seminar ab.

Du nutzt schon Claude Pro, Max oder ein Team-Konto? Dann ist dieser Teil erledigt.

**Optional: Zusatzguthaben.** Das Pro-Abo hat ein Nutzungskontingent. Zwei intensive Seminartage können es ausschöpfen, danach heisst es einige Stunden warten. Wer ohne Unterbruch weiterarbeiten will, kann in den Einstellungen von claude.ai Zusatzguthaben (Usage Credits) kaufen. Für das Seminar genügen einmalig rund USD 20. Der Kauf ist freiwillig und nur nötig, wenn das Kontingent im Seminar ausgeht.

## Schritt 3: Claude Code installieren

Claude Code läuft im **Terminal**. Das Terminal ist ein Fenster, in das Befehle als Text eingegeben werden. Für die Installation genügt ein einziger Befehl. Administratorrechte braucht es dafür nicht.

### Mac

1. Öffne das Terminal: `cmd` + `Leertaste`, «Terminal» tippen, `Enter`.
2. Kopiere diesen Befehl ins Terminal und drücke `Enter`:

```bash
curl -fsSL https://claude.ai/install.sh | bash
```

3. Die Installation zeigt keinen Fortschritt an. Warte, bis die Eingabezeile wieder erscheint.
4. Schliesse das Terminal und öffne es neu.

### Windows

1. Installiere zuerst **Git for Windows**: https://git-scm.com/downloads/win. Die Standardeinstellungen im Installationsassistenten passen.
2. Öffne **PowerShell**: Startmenü, «PowerShell» tippen, `Enter`. Die Eingabezeile beginnt mit `PS C:\`.
3. Kopiere diesen Befehl in PowerShell und drücke `Enter`:

```powershell
irm https://claude.ai/install.ps1 | iex
```

4. Warte, bis die Eingabezeile wieder erscheint. Schliesse PowerShell und öffne es neu.

### Installation prüfen

Tippe im neuen Terminalfenster:

```bash
claude --version
```

Erscheint eine Versionsnummer, zum Beispiel `2.1.211 (Claude Code)`, ist die Installation gelungen.

### Anmelden

1. Tippe `claude` und drücke `Enter`.
2. Wähle das Farbschema und danach die Anmeldung mit dem **Claude-Konto (Pro)**.
3. Der Browser öffnet sich. Melde Dich mit dem Konto aus Schritt 2 an und bestätige den Zugriff.
4. Zurück im Terminal: Bestätige die Fragen zur Sicherheit und zum Ordner.
5. Tippe als ersten Test `Hallo, was kannst du?` und drücke `Enter`. Antwortet Claude, ist alles bereit.
6. Beende Claude Code mit `/exit`.

## Schritt 4: Editoren installieren

Beide Programme sind kostenlos. Einrichten musst Du nichts, das machen wir im Seminar gemeinsam.

1. **Obsidian**, der Editor für Dein Personal OS: https://obsidian.md. Installieren, einmal starten, schliessen.
2. **Visual Studio Code**, der Editor für die eigene Website am zweiten Tag: https://code.visualstudio.com. Installieren, einmal starten, schliessen.

## Kurztest

Vor dem Seminar alles einmal prüfen:

- [ ] `claude --version` zeigt eine Versionsnummer.
- [ ] `claude` startet ohne neue Anmeldung und antwortet auf eine Frage.
- [ ] Obsidian und Visual Studio Code starten.
- [ ] Du kennst die Zugangsdaten zu Claude.

## Wenn etwas nicht klappt

- **`claude` wird nicht gefunden** (Mac: «command not found», Windows: «not recognized»): Terminal schliessen und neu öffnen. Hilft das nicht, `claude doctor` ausprobieren oder die Hilfe von Anthropic lesen: https://code.claude.com/docs/en/troubleshoot-install
- **Windows: Fehlermeldung «The token '&&' is not a valid statement separator» oder «'irm' is not recognized»:** Du bist im falschen Fenster. Den Befehl in PowerShell eingeben, nicht in der Eingabeaufforderung (CMD).
- **Anmeldung schlägt fehl oder Claude Code verlangt ein Abo:** Das Konto hat kein Pro-Abo. Auf claude.ai unter Einstellungen den Plan prüfen.
- **Etwas anderes:** Melde Dich bei Ralph Hutter, ralph.hutter@fh-hwz.ch. Bring Deinen Laptop auf jeden Fall mit, wir lösen den Rest am Morgen vor Beginn.
