# Einrichten von Claude Code

> Vorbereitung für das Seminar «Claude Code für Einsteiger», HWZ, Durchführung 25./26.11.2026. Version 0.5.0, Stand 20.11.2026. Ersetzt die Anleitung von Juni 2026 (`../PREREQUISITES.md`, `../../0000 GITBOOK/prerequisites.md`).

Für das Seminar brauchst Du fünf Dinge:

1. einen eigenen Laptop mit Installationsrechten
2. ein Claude-Pro-Abo
3. die Claude Desktop App, installiert und angemeldet
4. Claude Code im Terminal, installiert und angemeldet
5. den Editor Obsidian

Die Vorbereitung dauert ca. 30 Minuten. Erledige sie bis spätestens **Dienstag, 24.11.2026**.

**Die Reihenfolge ist zwingend:** Zuerst das Abo, danach Claude Desktop und Claude Code installieren. Die Anmeldung funktioniert nur mit einem bezahlten Konto. Im Seminar kommen beide Zugänge zum Einsatz, die Desktop App und das Terminal.

## Schritt 1: Laptop bereitstellen

Bring einen **privaten Laptop** mit macOS 13 oder neuer oder Windows 10 (Version 1809) oder neuer mit. Auf Firmengeräten sind Installationen und das Terminal häufig gesperrt, und Internetdienste können blockiert sein. Tablets und Chromebooks funktionieren nicht.

## Schritt 2: Claude Pro abonnieren

Claude Code ist im kostenlosen Claude-Konto nicht enthalten. Es braucht mindestens **Claude Pro**.

1. Öffne https://claude.ai und melde Dich an oder erstelle ein Konto.
2. Wähle **Upgrade** und das Abo **Pro** mit monatlicher Zahlung (USD 20 pro Monat, monatlich kündbar). Das Jahresabo lohnt sich für das Seminar nicht.
3. Schliesse das Abo frühestens eine Woche vor dem Seminar ab.

Du nutzt schon Claude Pro, Max oder ein Team-Konto? Dann ist dieser Teil erledigt.

**Optional: Zusatzguthaben.** Das Pro-Abo hat ein Nutzungskontingent. Zwei intensive Seminartage können es ausschöpfen, danach heisst es einige Stunden warten. Wer ohne Unterbruch weiterarbeiten will, kann in den Einstellungen von claude.ai Zusatzguthaben (Usage Credits) kaufen. Für das Seminar genügen einmalig rund USD 20. Der Kauf ist freiwillig und nur nötig, wenn das Kontingent im Seminar ausgeht.

## Schritt 3: Claude Desktop installieren

Die **Claude Desktop App** enthält Claude Code in der Registerkarte **Code**. Node.js ist dafür nicht nötig. Die Installation im Terminal (Schritt 4) bleibt trotzdem nötig, weil das Seminar in beiden Umgebungen arbeitet.

1. Lade die App für das eigene Betriebssystem herunter (Übersicht auf https://claude.ai/download):
   - macOS (Intel und Apple Silicon): https://claude.ai/api/desktop/darwin/universal/dmg/latest/redirect
   - Windows x64 (die meisten Windows-Laptops): https://claude.ai/api/desktop/win32/x64/setup/latest/redirect
   - Windows ARM64 (nur Geräte mit ARM-Prozessor, z.B. Surface mit Snapdragon): https://claude.ai/api/desktop/win32/arm64/setup/latest/redirect
2. Mac: Öffne die heruntergeladene Datei und ziehe **Claude** in den Ordner **Programme**. Windows: Führe den Installer aus.
3. Starte Claude (Mac: Programme, Windows: Startmenü) und melde Dich mit dem Konto aus Schritt 2 an.
4. Öffne in der Seitenleiste die Registerkarte **Code**. Sind nur Symbole sichtbar, zeigt das Daraufzeigen den Namen.
5. Schliesse die App. Die erste Session folgt im Seminar.

Voraussetzung: macOS 13 oder neuer, Windows 10 oder neuer. Die App aktualisiert sich selbst.

Verlangt die App ein Abo, hat das Konto kein Pro-Abo: Prüfe auf claude.ai unter Einstellungen den Plan. Erscheint die Aufforderung, sich online anzumelden, schliesse die Anmeldung im Browser ab und starte die App neu.

## Schritt 4: Claude Code im Terminal installieren

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

## Schritt 5: Obsidian installieren

Obsidian ist der Editor für Dein Personal OS und kostenlos. Einrichten musst Du nichts, das machen wir im Seminar gemeinsam.

1. Lade Obsidian von https://obsidian.md herunter und installiere es.
2. Starte es einmal und schliesse es wieder.

## Kurztest

Vor dem Seminar alles einmal prüfen:

- [ ] Claude Desktop startet, die Anmeldung steht, die Registerkarte **Code** ist sichtbar.
- [ ] `claude --version` zeigt eine Versionsnummer.
- [ ] `claude` startet ohne neue Anmeldung und antwortet auf eine Frage.
- [ ] Obsidian startet.
- [ ] Du kennst die Zugangsdaten zu Claude.

## Wenn etwas nicht klappt

- **`claude` wird nicht gefunden** (Mac: «command not found», Windows: «not recognized»): Terminal schliessen und neu öffnen. Hilft das nicht, `claude doctor` ausprobieren oder die Hilfe von Anthropic lesen: https://code.claude.com/docs/en/troubleshoot-install
- **Windows: Fehlermeldung «The token '&&' is not a valid statement separator» oder «'irm' is not recognized»:** Du bist im falschen Fenster. Den Befehl in PowerShell eingeben, nicht in der Eingabeaufforderung (CMD).
- **Anmeldung schlägt fehl oder Claude Code verlangt ein Abo:** Das Konto hat kein Pro-Abo. Auf claude.ai unter Einstellungen den Plan prüfen.
- **Etwas anderes:** Melde Dich bei Ralph Hutter, ralph.hutter@fh-hwz.ch. Bring Deinen Laptop auf jeden Fall mit, wir lösen den Rest am Morgen vor Beginn.

---

## Intern: Checkliste Dozent 25./26.11.2026 (nicht an Teilnehmende)

Grundlage: `TEACH/_templates/prerequisites/standard-vorbereitungsauftrag.md` 0.1.0 (liegt derzeit nur auf Branch `claude/midjourney-vorbereitungsauftrag-86e3b6`, Commit `1733d29e`).

**Termine**

- [ ] Programme Manager HWZ informieren, Mail über die Programmleitung (Entwurf: `0300 Marketing und Komm/vorbereitungsmail-2026-11-25.md`).
- [ ] Mail spätestens **Mittwoch, 18.11.2026** versenden. Der Standard verlangt zwei Wochen Vorlauf für die fertige Anleitung; dieser Termin ist bereits verpasst.
- [ ] Erinnerung am 23.11.2026 (Vorlage `whatsapp-kursvorbereitung.md` oder kurze Mail).
- [ ] Frist Teilnehmende: 24.11.2026.

**Prüfen vor dem Versand**

- [ ] Preis Claude Pro: am 14.11.2026 auf claude.com/pricing geprüft, USD 20 monatlich, Jahresabo USD 200. Vor Versand erneut prüfen.
- [x] Zusatzguthaben (Ausschreibung: einmalig ca. USD 20): optional, nur bei Mehrverbrauch. Entscheid Ralph 14.11.2026.
- [ ] Menüpfad für den Kauf von Usage Credits auf claude.ai beim Screenshot-Termin prüfen und in der Anleitung präzisieren.
- [ ] Installationsbefehle gegen https://code.claude.com/docs/en/setup prüfen (Stand 14.11.2026).
- [ ] Ablauf einmal auf einem frischen Mac und einem frischen Windows-Gerät durchspielen.
- [ ] Alle Links von Hand im Browser öffnen.
- [ ] Screenshots zu Hause aufnehmen, sobald ein Windows-Rechner bereitsteht (deutsche Oberfläche, Standard Abschnitt 7). Plätze im `index.html` als HTML-Kommentar markiert: `01-claude-upgrade-pro`, `03-mac-terminal-installation`, `04-windows-powershell-installation`, `05-claude-version`, `06-claude-code-anmeldung` (bis vor den letzten Klick), `07-claude-code-erste-antwort`. Ablage `img/`.

**Gegenüber Juni 2026 geändert**

- Node.js entfällt. Der native Installer braucht es auf keinem System.
- Claude Desktop neu als Schritt 3 (Version 0.5.0, 20.11.2026): Das Seminar arbeitet in der Desktop App und im Terminal. Offen: Ob Git for Windows für die Desktop App nötig ist, nennt die Anthropic-Doku nicht; es bleibt wegen des Terminals Pflicht. Screenshot-Platz `02-claude-desktop-code-tab` ist im `index.html` markiert.
- Git for Windows neu als Pflicht auf Windows, damit Claude Code mit Bash arbeitet und sich die Befehle im Kurs auf Mac und Windows gleichen.
- Kein GitHub-Konto: Die Website am zweiten Tag entsteht rein lokal, ohne Veröffentlichung (Entscheid Ralph 14.11.2026, Einsteigerkurs). Obsidian bleibt Voraussetzung.
- Kein Visual Studio Code: Für den Einsteigerkurs nicht nötig (Entscheid Ralph 14.11.2026).
- Laptop-Anforderung mit Mindestversionen der Betriebssysteme.

**Anleitung B (Kurstag)**

Nur anlegen, wenn die Einrichtung vor Ort Schritte braucht. Kandidat: Obsidian-Vault für das Personal OS. Hängt vom Kursablauf aus der courselib ab, siehe Aktualitätsprüfung.

**Veröffentlichung**

- [x] `index.html` im Absender HWZ, aufgebaut nach der Midjourney-Seite (14.11.2026). Bilder aus `img/` fehlen noch.
- [x] Privates Repo `ralphhutter/claude-code` angelegt, Kopie unter https://ralphhutter.github.io/claude-code/ mit `noindex` (14.11.2026). Nach den Screenshots beide Orte nachführen.

**Nach dem Kurs (27.11.2026)**

- [ ] Seite `ralphhutter.github.io/claude-code/` entfernen oder durch Hinweis ersetzen.
- [ ] Teilnehmende an die Kündigung des Abos erinnern (optional).
- [ ] Anleitung nach `_archiv/2026-11-25.claude-code-fuer-einsteiger.hwz/` verschieben.

## Versionsgeschichte

| Version | Datum | Änderung |
|---|---|---|
| 0.1.0 | 2026-11-14 | Erste Fassung nach Standard Vorbereitungsauftrag 0.1.0, Installation nach aktueller Doku von Anthropic |
| 0.2.0 | 2026-11-14 | HTML-Fassung `index.html` im HWZ-CD, Zusatzguthaben als optionaler Punkt |
| 0.3.0 | 2026-11-14 | GitHub-Konto entfällt, Website am zweiten Tag rein lokal |
| 0.4.0 | 2026-11-14 | Visual Studio Code entfällt, Obsidian einziger Editor |
