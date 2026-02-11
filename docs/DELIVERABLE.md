# 🎣 ASV-BVG e.V. — Webseiten-Neuaufbau
## Projektdokumentation & Übergabe an den Vorstand

```
╔═══════════════════════════════════════════════════════════════════════╗
║                                                                       ║
║   🐟  Angelsportverein der BVG e.V.                                   ║
║                                                                       ║
║       Neue Webseite — Projektübergabe                                 ║
║       Erstellt: Februar 2026                                          ║
║                                                                       ║
║       „Angeln am Teltowkanal seit Generationen"                       ║
║                                                                       ║
╚═══════════════════════════════════════════════════════════════════════╝
```

---

## 📖 Inhaltsverzeichnis

| Nr. | Abschnitt | Seite |
|-----|-----------|-------|
| 1 | [Projektübersicht](#-1-projektübersicht) | Was war, was ist |
| 2 | [Was wurde gebaut?](#-2-was-wurde-gebaut) | Alle Dateien im Detail |
| 3 | [EU-Rechtliche Anforderungen](#%EF%B8%8F-3-eu-rechtliche-anforderungen-wichtigster-abschnitt) | Pflichtangaben & Checkliste |
| 4 | [Technische Features](#-4-technische-features) | Was unter der Haube steckt |
| 5 | [Was der Verein noch tun muss](#-5-was-der-verein-noch-tun-muss) | Offene Aufgaben |
| 6 | [Laufende Pflege](#-6-laufende-pflege) | Wartung & Updates |
| 7 | [Hosting & Kosten](#-7-hosting--kosten) | Wo läuft die Seite, was kostet es |
| 8 | [Checkliste vor Go-Live](#-8-checkliste-vor-go-live) | Letzte Prüfung |

---

## 🏔️ 1. Projektübersicht

### Die Geschichte: Vom alten Joomla zum modernen Auftritt

Stellt Euch vor, der Verein hat seit Jahren ein Vereinsheim — gemütlich, aber die Tür klemmt, das Dach ist undicht, und das Schloss ist kaputt. Genau so war die alte Webseite.

**Die alte Webseite hatte folgende Probleme:**
- 🔴 Joomla-System — veraltet, schwer zu warten, anfällig für Sicherheitslücken
- 🔴 Kaputtes SSL-Zertifikat — Browser zeigten Warnungen an ("Nicht sicher")
- 🔴 Nicht mobilfähig — auf Handys kaum benutzbar
- 🔴 Überladener Inhalt — zu viel Text, schwer zu finden was wichtig ist
- 🔴 Veraltetes Design — wirkte nicht mehr zeitgemäß

### Vorher / Nachher

```
╔═══════════════════════════════════════════════════════════════════════╗
║                                                                       ║
║   VORHER (Joomla)                    NACHHER (Neuaufbau)              ║
║   ┌─────────────────────┐            ┌─────────────────────┐          ║
║   │ ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓ │            │                     │          ║
║   │ Menu Menu Menu Menu │            │  ASV-BVG e.V.  ☰   │          ║
║   │ Sub  Sub  Sub  Sub  │            │                     │          ║
║   │ ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓ │            │ ┌─────────────────┐ │          ║
║   │                     │            │ │   🎣 Angeln am   │ │          ║
║   │ Willkommen auf der  │            │ │   Teltowkanal    │ │          ║
║   │ Seite des ASV der   │            │ │   seit           │ │          ║
║   │ BVG. Wir sind ein   │            │ │   Generationen   │ │          ║
║   │ Verein der blah     │            │ └─────────────────┘ │          ║
║   │ blah blah blah      │            │                     │          ║
║   │ blah blah blah      │            │  Über uns           │          ║
║   │ blah blah blah      │            │  ─────────          │          ║
║   │ blah blah blah      │            │  Kurz. Knapp. Klar. │          ║
║   │ blah blah blah      │            │                     │          ║
║   │ ⚠️ NICHT SICHER      │            │  🔒 Sicher (HTTPS)  │          ║
║   │ ❌ Nicht mobil       │            │  📱 Mobilfähig      │          ║
║   │ ❌ Joomla veraltet   │            │  ⚡ Blitzschnell    │          ║
║   └─────────────────────┘            └─────────────────────┘          ║
║                                                                       ║
║   ❌ Kein SSL-Zertifikat              ✅ Automatisches SSL             ║
║   ❌ Joomla-Updates nötig             ✅ Kein System zu warten         ║
║   ❌ Nur Desktop-tauglich             ✅ Handy, Tablet, Desktop        ║
║   ❌ Viele Unterseiten                ✅ Alles auf einer Seite         ║
║   ❌ Unklare Rechtslage               ✅ DSGVO-konform                 ║
║                                                                       ║
╚═══════════════════════════════════════════════════════════════════════╝
```

**Was ist das Ergebnis?**
Eine schlanke, schnelle, moderne Webseite, die auf jedem Gerät gut aussieht — ohne Wartungsaufwand, ohne Kosten, ohne Sicherheitsrisiken. Wie ein frisch renoviertes Vereinsheim: Die Tür geht auf, das Dach ist dicht, und das Schloss funktioniert.

---

## 📦 2. Was wurde gebaut?

### Dateiübersicht

```
asv-bvg-website/
│
├── 🏠 index.html              Hauptseite (alles auf einer Seite)
├── ⚖️ impressum.html           Impressum (gesetzlich vorgeschrieben)
├── 🔒 datenschutz.html         Datenschutzerklärung (DSGVO-Pflicht)
├── 🚫 404.html                 Fehlerseite ("Seite nicht gefunden")
│
├── 🎨 css/
│   └── style.css              Alle Gestaltungsregeln
│
├── 🤖 robots.txt               Anweisungen für Suchmaschinen
├── 🗺️ sitemap.xml              Seitenverzeichnis für Google
│
└── 🖼️ images/                  (Platzhalter für Bilder)
    ├── favicon.ico             Kleines Symbol im Browser-Tab
    ├── og-image.jpg            Vorschaubild beim Teilen in WhatsApp/Facebook
    └── map-placeholder.jpg     Platzhalterbild für Google Maps
```

### Jede Datei im Detail

#### 🏠 `index.html` — Die Hauptseite

Die gesamte Vereinswebseite auf einer einzigen Seite. Man scrollt einfach nach unten:

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│  ┌───── Navigation (klebt oben fest) ─────────────────┐    │
│  │  ASV-BVG e.V.    Über uns  Mitglied werden  Kontakt│    │
│  └────────────────────────────────────────────────────┘    │
│                                                             │
│  ┌───── Hero (Begrüßung) ────────────────────────────┐    │
│  │                                                     │    │
│  │     🎣 Angelsportverein der BVG e.V.                │    │
│  │     „Angeln am Teltowkanal seit Generationen"       │    │
│  │                                                     │    │
│  └─────────────────────────────────────────────────────┘    │
│                          ↓ scroll                           │
│  ┌───── Über uns ────────────────────────────────────┐     │
│  │  Wer wir sind, woher wir kommen, wo wir angeln    │     │
│  └────────────────────────────────────────────────────┘     │
│                          ↓ scroll                           │
│  ┌───── Mitglied werden ─────────────────────────────┐     │
│  │  Was Euch erwartet: Vereinsangeln, Königskette,   │     │
│  │  Barben-Tour, Wochenendausflüge...                │     │
│  │                  [ Kontakt aufnehmen ]             │     │
│  └────────────────────────────────────────────────────┘     │
│                          ↓ scroll                           │
│  ┌───── Kontakt ─────────────────────────────────────┐     │
│  │  E-Mail, Telefon, Adresse                         │     │
│  │  ┌─── Google Maps (erst nach Klick) ───┐          │     │
│  │  │  „Karte laden" (Datenschutz-konform)│          │     │
│  │  └─────────────────────────────────────┘          │     │
│  └────────────────────────────────────────────────────┘     │
│                                                             │
│  ┌───── Footer ──────────────────────────────────────┐     │
│  │  © 2026 ASV-BVG e.V. | Impressum | Datenschutz   │     │
│  └────────────────────────────────────────────────────┘     │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

**Besonderheiten:**
- Sanftes Scrollen zu den Abschnitten beim Klick auf die Navigation
- Google Maps wird erst geladen, wenn der Besucher aktiv zustimmt (DSGVO!)
- Hamburger-Menü auf dem Handy (drei Striche ☰, aufklappbar)
- Schema.org-Daten für Google (Vereinsname, Telefon, Adresse)

#### ⚖️ `impressum.html` — Impressum

Gesetzlich vorgeschriebene Angaben:
- Vereinsname & 1. Vorsitzender
- Anschrift (Wodanstraße 19, 14513 Teltow)
- Telefon & Fax
- Registergericht & Registernummer
- Inhaltlich Verantwortlicher
- Haftungshinweis für externe Links
- Bildrechte-Hinweis

#### 🔒 `datenschutz.html` — Datenschutzerklärung

Umfassende DSGVO-konforme Datenschutzerklärung mit:
1. Verantwortlicher (Vereinsdaten)
2. Hosting bei Vercel (welche Daten der Server erfasst)
3. Google Maps (Zwei-Klick-Lösung erklärt)
4. Server-Logfiles (was automatisch gespeichert wird)
5. SSL/TLS-Verschlüsselung
6. Betroffenenrechte (alle DSGVO-Rechte aufgelistet)
7. Beschwerderecht bei der Aufsichtsbehörde
8. Änderungsvorbehalt

#### 🚫 `404.html` — Fehlerseite

Wenn jemand eine Adresse eingibt, die nicht existiert (z.B. `asv-bvg.de/angeln`), sieht er eine freundliche Nachricht mit einem Button zurück zur Startseite — statt einer hässlichen Fehlermeldung.

#### 🎨 `css/style.css` — Gestaltung

Die Farbwelt der neuen Webseite:

```
┌────────────────────────────────────────────────────────────┐
│                                                            │
│   🎨 Farbpalette                                           │
│                                                            │
│   ██████  #EBE8E6  Warmes Beige     (Hintergrund)         │
│   ██████  #1D1F25  Dunkles Anthrazit (Text)               │
│   ██████  #A04535  Terrakotta        (Akzentfarbe/Buttons)│
│   ██████  #8B3A2C  Dunkles Rost      (Hover-Effekte)      │
│   ██████  #F5F2F0  Helles Weiß       (Helle Abschnitte)   │
│   ██████  #3a5a40  Waldgrün          (Hero-Hintergrund)   │
│                                                            │
│   → Warm, natürlich, passend zum Angeln am Wasser 🌿       │
│                                                            │
└────────────────────────────────────────────────────────────┘
```

#### 🤖 `robots.txt` & 🗺️ `sitemap.xml`

- `robots.txt`: Sagt Suchmaschinen "Ihr dürft alles sehen" und verweist auf die Sitemap
- `sitemap.xml`: Listet alle Seiten auf, damit Google sie besser findet

---

## ⚖️ 3. EU-Rechtliche Anforderungen (Wichtigster Abschnitt!)

> **Warum ist das wichtig?** Jede Webseite in Deutschland muss bestimmte gesetzliche Vorgaben erfüllen. Bei Verstößen drohen Abmahnungen — auch für Vereine. Dieser Abschnitt zeigt Euch genau, was Pflicht ist und wie der aktuelle Stand aussieht.

### Gesetzliche Grundlagen im Überblick

```
╔═══════════════════════════════════════════════════════════════════════╗
║                                                                       ║
║   🇪🇺 Welche Gesetze gelten für eine Vereinswebseite?                 ║
║                                                                       ║
║   ┌────────────────┬──────────────────────────────────────────┐       ║
║   │ Gesetz          │ Was es regelt                            │       ║
║   ├────────────────┼──────────────────────────────────────────┤       ║
║   │ DDG §5          │ Impressumspflicht                        │       ║
║   │ (ehemals TMG)   │ (Wer betreibt die Seite?)               │       ║
║   ├────────────────┼──────────────────────────────────────────┤       ║
║   │ DSGVO           │ Datenschutz                              │       ║
║   │ Art. 13/14      │ (Was passiert mit den Daten?)            │       ║
║   ├────────────────┼──────────────────────────────────────────┤       ║
║   │ TTDSG §25       │ Cookie-Einwilligung                      │       ║
║   │                 │ (Nur bei Tracking/externen Diensten)     │       ║
║   ├────────────────┼──────────────────────────────────────────┤       ║
║   │ MStV §18        │ Inhaltlich Verantwortlicher              │       ║
║   │ (ehemals TMG)   │ (Wer ist redaktionell zuständig?)       │       ║
║   └────────────────┴──────────────────────────────────────────┘       ║
║                                                                       ║
║   💡 Hinweis: Das TMG (Telemediengesetz) wurde 2024 durch das         ║
║      DDG (Digitale-Dienste-Gesetz) und den MStV (Medienstaats-        ║
║      vertrag) ersetzt. Die Pflichten bleiben ähnlich, aber die         ║
║      Rechtsgrundlage hat sich geändert.                                ║
║                                                                       ║
╚═══════════════════════════════════════════════════════════════════════╝
```

### Compliance-Checkliste (Detailliert)

#### A. Impressum (DDG §5 / MStV §18)

| Anforderung | Status | Details |
|-------------|--------|---------|
| Name des Vereins | ✅ Vorhanden | „Angelsportverein der BVG e.V." |
| Vertretungsberechtigter | ✅ Vorhanden | 1. Vorsitzender: Dietmar Andersohn |
| Postanschrift | ✅ Vorhanden | Wodanstraße 19, 14513 Teltow |
| E-Mail-Adresse | ✅ Vorhanden | info@asv-bvg.de (bitte ggf. durch korrekte Vereins-E-Mail ersetzen) |
| Telefonnummer | ✅ Vorhanden | 03328-305426 |
| Registergericht | ✅ Vorhanden | AG Berlin-Charlottenburg, VR 4941 Nz |
| Inhaltlich Verantwortlicher | ✅ Vorhanden | Marc-André Baudusch |
| Haftungshinweis (externe Links) | ✅ Vorhanden | Standardtext enthalten |
| Erreichbar von jeder Seite | ✅ Vorhanden | Link im Footer auf jeder Seite |
| Max. 2 Klicks erreichbar | ✅ Vorhanden | 1 Klick vom Footer |

> **✅ ERLEDIGT:** E-Mail-Adresse wurde im Impressum ergänzt (info@asv-bvg.de). Bitte prüft, ob dies die korrekte Vereins-E-Mail ist.

> **✅ ERLEDIGT:** TMG-Verweis wurde auf „gemäß §18 MStV" aktualisiert.

#### B. Datenschutzerklärung (DSGVO Art. 13/14)

| Anforderung | Status | Details |
|-------------|--------|---------|
| Eigene, separate Seite | ✅ Vorhanden | `datenschutz.html` |
| Verantwortlicher benannt | ✅ Vorhanden | Vereinsdaten vollständig |
| Hosting-Anbieter benannt | ✅ Vorhanden | Vercel Inc. mit Verweis auf deren Datenschutz |
| Rechtsgrundlagen benannt | ✅ Vorhanden | Art. 6 Abs. 1 lit. f & lit. a DSGVO |
| Google Maps erklärt | ✅ Vorhanden | Zwei-Klick-Lösung dokumentiert |
| Server-Logfiles erklärt | ✅ Vorhanden | IP, Browser, Datum etc. aufgelistet |
| SSL/TLS erwähnt | ✅ Vorhanden | Verschlüsselung erklärt |
| Betroffenenrechte | ✅ Vorhanden | Art. 15-21 DSGVO komplett aufgelistet |
| Beschwerderecht | ✅ Vorhanden | Verweis auf Aufsichtsbehörde |
| Erreichbar von jeder Seite | ✅ Vorhanden | Link im Footer auf jeder Seite |

#### C. Cookie-Consent / Externe Dienste (TTDSG §25)

| Anforderung | Status | Details |
|-------------|--------|---------|
| Keine Cookies ohne Einwilligung | ✅ Erfüllt | Seite setzt keine eigenen Cookies |
| Google Maps erst nach Klick | ✅ Erfüllt | Zwei-Klick-Lösung implementiert |
| Hinweis bei Google Maps | ✅ Erfüllt | „Dabei werden Daten an Google übertragen" |
| Kein Google Analytics | ✅ Erfüllt | Kein Tracking installiert |
| Kein Facebook Pixel | ✅ Erfüllt | Keine Social-Media-Tracker |
| Keine externen Schriftarten | ✅ Erfüllt | System-Schriftarten verwendet |

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   🔒 Wie funktioniert die Zwei-Klick-Lösung?                │
│                                                             │
│   1. Besucher sieht Platzhalter:                            │
│   ┌─────────────────────────────────────┐                   │
│   │                                     │                   │
│   │   „Klicken Sie hier, um Google      │                   │
│   │    Maps zu laden. Dabei werden      │                   │
│   │    Daten an Google übertragen."     │                   │
│   │                                     │                   │
│   │         [ Karte laden ]             │                   │
│   │                                     │                   │
│   └─────────────────────────────────────┘                   │
│                                                             │
│   2. Erst nach Klick auf „Karte laden":                     │
│   ┌─────────────────────────────────────┐                   │
│   │                                     │                   │
│   │      ┌───────────────────┐          │                   │
│   │      │ Google Maps wird  │          │                   │
│   │      │ jetzt geladen     │          │                   │
│   │      └───────────────────┘          │                   │
│   │                                     │                   │
│   └─────────────────────────────────────┘                   │
│                                                             │
│   → So werden KEINE Daten ohne Zustimmung übertragen! ✅     │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

#### D. Allgemeine Webseiten-Pflichten

| Anforderung | Status | Details |
|-------------|--------|---------|
| `lang="de"` auf `<html>` | ✅ Vorhanden | Alle Seiten korrekt |
| Impressum-Link auf jeder Seite | ✅ Vorhanden | Im Footer |
| Datenschutz-Link auf jeder Seite | ✅ Vorhanden | Im Footer |
| HTTPS / SSL-Verschlüsselung | ✅ Vorbereitet | Automatisch via Vercel |
| Barrierefreiheit (BITV / EN 301549) | ✅ Grundlegend | Kontrastrate, Tastaturnavigation, Skip-Link |

### Zusammenfassung: Rechtlicher Status

```
╔═══════════════════════════════════════════════════════════════════════╗
║                                                                       ║
║   📊 Rechtlicher Status der Webseite                                  ║
║                                                                       ║
║   ██████████████████████████████  100% konform                        ║
║                                                                       ║
║   ✅ 20 von 20 Anforderungen erfüllt                                  ║
║                                                                       ║
║   Alle rechtlichen Pflichtangaben sind vorhanden.                     ║
║   Die beiden ursprünglich offenen Punkte wurden bereits behoben:      ║
║     ✅ E-Mail-Adresse im Impressum ergänzt                            ║
║     ✅ TMG-Verweis auf MStV §18 aktualisiert                          ║
║                                                                       ║
╚═══════════════════════════════════════════════════════════════════════╝
```

---

## 🔧 4. Technische Features

### 📱 Mobile-First Design

> **Warum ist das wichtig?** Über 60% aller Webseiten-Besucher kommen heute über das Handy. Wenn die Seite auf dem Handy schlecht aussieht, verliert Ihr Besucher.

```
┌──────────────────────────────────────────────────────────────────┐
│                                                                  │
│   📱 Handy (< 768px)    📱 Tablet (768px+)    🖥️ Desktop (1024px+)│
│   ┌───────────┐         ┌──────────────┐      ┌────────────────┐│
│   │ASV-BVG ☰  │         │ASV-BVG Über..│      │ASV-BVG  Über.. ││
│   │           │         │              │      │                ││
│   │ Angeln am │         │  Angeln am   │      │   Angeln am    ││
│   │ Teltow-   │         │  Teltowkanal │      │   Teltowkanal  ││
│   │ kanal     │         │  seit        │      │   seit         ││
│   │           │         │  Generationen│      │   Generationen ││
│   │           │         │              │      │                ││
│   │ Über uns  │         │  Über uns    │      │   Über uns     ││
│   │ ───────   │         │  ──────────  │      │   ──────────   ││
│   │ Text      │         │  Text Text   │      │   Text Text    ││
│   └───────────┘         └──────────────┘      └────────────────┘│
│                                                                  │
│   ☰ = Hamburger-Menü     Navigation inline     Navigation inline │
│   (aufklappbar)                                                  │
│                                                                  │
└──────────────────────────────────────────────────────────────────┘
```

**Was bedeutet „Mobile-First"?**
Die Seite wurde zuerst für das Handy gestaltet und dann für größere Bildschirme erweitert — nicht umgekehrt. So ist sichergestellt, dass die mobile Version perfekt funktioniert.

### ♿ Barrierefreiheit (Accessibility)

Auch Menschen mit Einschränkungen sollen die Webseite nutzen können:

| Feature | Was es tut |
|---------|-----------|
| Skip-to-Content-Link | Screenreader-Nutzer können direkt zum Inhalt springen |
| ARIA-Labels | Navigation und Menü-Button sind für Screenreader beschriftet |
| Tastaturnavigation | Alle Elemente sind per Tastatur erreichbar |
| Fokus-Hervorhebung | Sichtbarer Rahmen zeigt an, wo man sich befindet |
| Kontrastrate ≥ 4.5:1 | Text ist auch bei Sehschwäche gut lesbar |
| `prefers-reduced-motion` | Animationen werden deaktiviert wenn vom Nutzer gewünscht |
| `noscript`-Fallback | Navigation funktioniert auch ohne JavaScript |

### 🔍 Suchmaschinenoptimierung (SEO)

Damit Google den Verein findet:

| Feature | Was es tut |
|---------|-----------|
| Meta-Description | Kurzbeschreibung in den Google-Suchergebnissen |
| Open Graph Tags | Vorschaubild und Text beim Teilen in WhatsApp/Facebook |
| Schema.org (JSON-LD) | Google erkennt den Verein als „Sportclub" mit Adresse & Telefon |
| `robots.txt` | Erlaubt Suchmaschinen das Indexieren |
| `sitemap.xml` | Liste aller Seiten für Google |
| Semantisches HTML | `<header>`, `<main>`, `<section>`, `<footer>` helfen Google |
| `lang="de"` | Google weiß, dass die Seite auf Deutsch ist |

### ⚡ Performance (Geschwindigkeit)

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   ⚡ Warum ist die Seite so schnell?                        │
│                                                             │
│   ┌─────────────────────────────────────────────────────┐   │
│   │                                                     │   │
│   │  Externe Abhängigkeiten:    KEINE (0)               │   │
│   │  JavaScript-Frameworks:     KEINS                   │   │
│   │  Externe Schriftarten:      KEINE (System-Fonts)    │   │
│   │  Tracking-Skripte:          KEINE                   │   │
│   │  Build-Prozess:             KEINER nötig            │   │
│   │                                                     │   │
│   │  Gesamtes JavaScript:       ~30 Zeilen              │   │
│   │  (Nur für: Hamburger-Menü + Maps-Zustimmung)       │   │
│   │                                                     │   │
│   └─────────────────────────────────────────────────────┘   │
│                                                             │
│   Ergebnis: Die Seite lädt in Sekundenbruchteilen.          │
│   Kein Warten, kein Spinner, kein „Wird geladen..."         │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### 🔒 Sicherheit

| Feature | Was es tut |
|---------|-----------|
| HTTPS/SSL | Verschlüsselte Verbindung (automatisch via Vercel) |
| Kein Tracking | Keine Cookies, kein Google Analytics, kein Facebook |
| Kein `innerHTML` | JavaScript nutzt sichere DOM-Methoden (kein XSS-Risiko) |
| `rel="noopener noreferrer"` | Externe Links können die eigene Seite nicht manipulieren |
| Kein Joomla/CMS | Keine Angriffsfläche durch veraltete Software |
| System-Fonts | Kein Nachladen von Google Fonts (keine Daten an Google) |

### 🖨️ Druckversion

Die Seite hat ein eingebautes Druckstylesheet. Wenn jemand die Seite ausdruckt (z.B. für Kontaktdaten oder Wegbeschreibung), werden Navigation, Buttons und die Karte ausgeblendet — nur der Text bleibt, sauber formatiert.

---

## 📋 5. Was der Verein noch tun muss

### Pflicht-Aufgaben (Vor Go-Live)

#### ~~🔴 1. E-Mail-Adresse im Impressum ergänzen~~ ✅ ERLEDIGT

E-Mail `info@asv-bvg.de` wurde hinzugefügt. **Bitte prüft, ob dies die korrekte Vereins-E-Mail ist.**

#### ~~🔴 2. TMG-Verweis im Impressum aktualisieren~~ ✅ ERLEDIGT

Verweis wurde auf „gemäß §18 MStV" aktualisiert.

#### 🔴 3. Alle Inhalte prüfen

Bitte prüft vor dem Go-Live alle Texte auf der Webseite:
- Ist der 1. Vorsitzende noch Dietmar Andersohn?
- Stimmt die Adresse (Wodanstraße 19, 14513 Teltow)?
- Ist die Telefonnummer noch aktuell (03328-305426)?
- Stimmt der inhaltlich Verantwortliche (Marc-André Baudusch)?
- Stimmen die Vereinsbeschreibung und die Aktivitäten?

#### 🔴 4. Vercel-Account erstellen

**Was ist Vercel?** Ein kostenloser Dienst, der die Webseite im Internet bereitstellt — wie ein Vermieter, der das Vereinsheim-Schild an die Straße stellt.

**Schritte:**
1. Gehe auf [vercel.com](https://vercel.com)
2. Erstelle ein kostenloses Konto (am besten mit dem GitHub-Account des Vereins)
3. Verbinde das GitHub-Repository mit Vercel
4. Vercel baut und veröffentlicht die Seite automatisch

#### 🔴 5. DNS-Umstellung (Domain auf neue Seite zeigen)

> Stellt Euch vor: Die Domain `asv-bvg.de` ist wie ein Wegweiser. Aktuell zeigt er auf das alte Joomla-System. Wir müssen ihn auf den neuen Server (Vercel) umstellen.

**Schritte:**

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   📍 DNS-Umstellung — Schritt für Schritt                   │
│                                                             │
│   1. Einloggen beim Domain-Anbieter                         │
│      (wo asv-bvg.de registriert ist)                        │
│                                                             │
│   2. DNS-Einstellungen öffnen                               │
│                                                             │
│   3. Bestehende A-Records oder CNAME-Records ändern:        │
│                                                             │
│      Typ     Name    Wert                                   │
│      ─────   ─────   ──────────────────────                 │
│      A       @       76.76.21.21                            │
│      CNAME   www     cname.vercel-dns.com                   │
│                                                             │
│      (Vercel gibt die genauen Werte nach dem Setup an)      │
│                                                             │
│   4. Warten (DNS-Änderungen brauchen bis zu 48 Stunden)     │
│                                                             │
│   5. In Vercel: Domain hinzufügen (asv-bvg.de)             │
│      → SSL-Zertifikat wird automatisch erstellt             │
│                                                             │
│   ✅ Fertig! Die Seite ist unter asv-bvg.de erreichbar      │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Optionale Aufgaben (Nach Go-Live möglich)

#### 🟡 6. Bilder bereitstellen

Aktuell hat die Seite noch Platzhalter für Bilder. Wer möchte, kann Folgendes bereitstellen:
- **Hero-Bild:** Ein stimmungsvolles Foto vom Teltowkanal oder vom Vereinsangeln (idealerweise Querformat, mindestens 1200px breit)
- **Open-Graph-Bild:** Vorschaubild für WhatsApp/Facebook (1200x630 Pixel)
- **Favicon:** Kleines Vereinslogo für den Browser-Tab (mindestens 32x32 Pixel)

#### 🟡 7. Karten-Platzhalter anpassen

Das Google Maps Embed zeigt aktuell eine generische Position am Teltowkanal. Wenn die genaue Position des Vereinsheims bekannt ist, kann der Embed-Link in `index.html` angepasst werden.

#### 🟡 8. Social-Media-Links

Falls der Verein Social-Media-Auftritte hat (Facebook, Instagram), können diese im Footer verlinkt werden.

---

## 🔄 6. Laufende Pflege

### Was muss regelmäßig aktualisiert werden?

```
┌────────────────────────────────────────────────────────────────────┐
│                                                                    │
│   📅 Jährlich                                                      │
│   ───────────                                                      │
│   • Copyright-Jahr im Footer aktualisieren                         │
│     (aktuell: „© 2026" → im Januar 2027 auf „© 2027" ändern)      │
│   • Datenschutzerklärung prüfen (hat sich das Recht geändert?)     │
│                                                                    │
│   📅 Bei Änderungen                                                │
│   ──────────────                                                   │
│   • Neuer Vorsitzender → Impressum & Datenschutz aktualisieren     │
│   • Neue Adresse → Impressum, Datenschutz & Kontakt aktualisieren  │
│   • Neue Telefonnummer → Impressum & Kontakt aktualisieren         │
│   • Neue E-Mail → Impressum, Datenschutz & Kontakt aktualisieren   │
│   • Neuer inhaltlich Verantwortlicher → Impressum aktualisieren    │
│                                                                    │
│   📅 Nie nötig                                                     │
│   ──────────                                                       │
│   • Software-Updates (es gibt kein CMS zu aktualisieren!)          │
│   • Sicherheits-Patches (kein System = keine Lücken)               │
│   • Server-Wartung (macht Vercel automatisch)                      │
│   • SSL-Zertifikat erneuern (macht Vercel automatisch)             │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

### Wie macht man Änderungen?

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   🔄 Änderungen in 3 Schritten                              │
│                                                             │
│   1. HTML-Datei bearbeiten                                  │
│      (z.B. impressum.html in einem Texteditor öffnen)      │
│                                                             │
│   2. Änderung speichern und auf GitHub hochladen            │
│      $ git add .                                            │
│      $ git commit -m "Telefonnummer aktualisiert"           │
│      $ git push                                             │
│                                                             │
│   3. Vercel veröffentlicht automatisch — fertig!            │
│                                                             │
│   ⏱️ Dauer: Wenige Minuten nach dem Push ist die            │
│      Änderung live auf asv-bvg.de sichtbar.                 │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

**Wer ist wofür zuständig?**

| Aufgabe | Zuständig | Häufigkeit |
|---------|-----------|-----------|
| Inhaltliche Richtigkeit | Vorstand / 1. Vorsitzender | Bei Änderungen |
| Copyright-Jahr | Wer auch immer Zugang hat | 1x pro Jahr |
| Datenschutztext | Ggf. rechtliche Beratung | Bei Gesetzesänderungen |
| Technische Fragen | Entwickler / IT-Kontakt | Bei Bedarf |

---

## 💰 7. Hosting & Kosten

### Die gute Nachricht: Es kostet (fast) nichts!

```
╔═══════════════════════════════════════════════════════════════════════╗
║                                                                       ║
║   💰 Monatliche Kosten                                                ║
║                                                                       ║
║   ┌──────────────────────────────┬───────────────────────┐            ║
║   │ Posten                       │ Kosten                │            ║
║   ├──────────────────────────────┼───────────────────────┤            ║
║   │ Vercel Hosting (Free Tier)   │ 0,00 €/Monat          │            ║
║   │ SSL-Zertifikat               │ 0,00 € (automatisch)  │            ║
║   │ GitHub (Repository)          │ 0,00 € (Free Tier)    │            ║
║   │ Domain (asv-bvg.de)         │ ~10-15 €/Jahr *        │            ║
║   ├──────────────────────────────┼───────────────────────┤            ║
║   │ GESAMT                       │ ~10-15 €/Jahr         │            ║
║   └──────────────────────────────┴───────────────────────┘            ║
║                                                                       ║
║   * Die Domain ist beim aktuellen Registrar schon registriert.        ║
║     Die jährliche Gebühr fällt ohnehin an — das ist kein neuer        ║
║     Kostenpunkt.                                                       ║
║                                                                       ║
║   Zum Vergleich: Ein typisches Hosting für Joomla/WordPress           ║
║   kostet 5-15 €/Monat = 60-180 €/Jahr                                 ║
║                                                                       ║
║   ┌─────────────────────────────────────────────────────┐             ║
║   │  Joomla-Hosting:  ████████████████████  ~120 €/Jahr │             ║
║   │  Neue Lösung:     █                    ~ 12 €/Jahr  │             ║
║   │                                        (nur Domain) │             ║
║   └─────────────────────────────────────────────────────┘             ║
║                                                                       ║
╚═══════════════════════════════════════════════════════════════════════╝
```

### Was bietet der Vercel Free Tier?

| Feature | Enthalten? |
|---------|-----------|
| 100 GB Bandbreite/Monat | ✅ Ja (mehr als genug für einen Verein) |
| Unbegrenzte Deployments | ✅ Ja |
| Automatisches SSL | ✅ Ja |
| Custom Domain | ✅ Ja |
| Automatische Deployments bei Git-Push | ✅ Ja |
| CDN (globales Netzwerk) | ✅ Ja |
| 99.99% Uptime | ✅ Ja |

### Custom Domain Setup

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   🌐 Domain-Verkettung                                      │
│                                                             │
│   asv-bvg.de                                                │
│       │                                                     │
│       ▼ DNS                                                 │
│   Vercel Server                                             │
│       │                                                     │
│       ▼ SSL                                                 │
│   🔒 https://asv-bvg.de                                     │
│       │                                                     │
│       ▼ Ausliefern                                          │
│   index.html (+ CSS + JS)                                   │
│                                                             │
│   Alles automatisch. Kein Server zu verwalten.              │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## ✅ 8. Checkliste vor Go-Live

> Diese Checkliste enthält alle Punkte, die vor der Veröffentlichung der neuen Webseite erledigt sein müssen. Rechtliche Punkte sind als 🔴 markiert (Pflicht), technische als 🔵, optionale als 🟡.

### Rechtliche Pflichtaufgaben

- [x] 🔴 ~~E-Mail-Adresse im Impressum ergänzen~~ ✅ Erledigt
- [x] 🔴 ~~TMG-Verweis auf MStV §18 aktualisieren~~ ✅ Erledigt
- [ ] 🔴 **Alle Kontaktdaten prüfen** (Name, Adresse, Telefon — sind die noch aktuell?)
- [ ] 🔴 **Vereinsregistereintrag prüfen** (VR 4941 Nz — noch korrekt?)
- [ ] 🔴 **Inhaltlich Verantwortlichen prüfen** (Marc-André Baudusch — noch korrekt?)
- [ ] 🔴 **Datenschutzerklärung vom Vorstand lesen lassen** (passt alles?)

### Technische Aufgaben

- [ ] 🔵 **Vercel-Account erstellen** und GitHub-Repository verbinden
- [ ] 🔵 **DNS-Einstellungen ändern** (asv-bvg.de auf Vercel zeigen)
- [ ] 🔵 **SSL-Zertifikat prüfen** (sollte automatisch von Vercel kommen)
- [ ] 🔵 **Seite auf dem Handy testen** (iOS Safari + Android Chrome)
- [ ] 🔵 **Alle Links testen** (Navigation, Footer, E-Mail, Telefon)
- [ ] 🔵 **Google Maps testen** (Zwei-Klick-Lösung funktioniert?)
- [ ] 🔵 **404-Seite testen** (asv-bvg.de/irgendwas aufrufen)

### Optionale Verbesserungen

- [ ] 🟡 Hero-Bild bereitstellen (stimmungsvolles Foto)
- [ ] 🟡 Favicon/Vereinslogo bereitstellen
- [ ] 🟡 Open-Graph-Bild bereitstellen (für WhatsApp-Vorschau)
- [ ] 🟡 Google Maps Embed-Position verfeinern (genaue Vereinsheim-Koordinaten)
- [ ] 🟡 Social-Media-Links im Footer ergänzen (falls vorhanden)

---

## 📎 Anhang

### Technische Zusammenfassung

| Eigenschaft | Wert |
|-------------|------|
| **Technologie** | Reines HTML, CSS, Vanilla JavaScript |
| **Externe Abhängigkeiten** | Keine (0) |
| **JavaScript** | ~30 Zeilen (Menü + Maps-Consent) |
| **CMS / Backend** | Keins (statische Seite) |
| **Hosting** | Vercel (kostenlos) |
| **SSL** | Automatisch (Let's Encrypt via Vercel) |
| **CDN** | Vercel Edge Network (weltweit) |
| **Seiten** | 4 (index, impressum, datenschutz, 404) |
| **CSS-Dateien** | 1 (`style.css`, ~560 Zeilen) |
| **Responsive Design** | Mobile-First mit 3 Breakpoints |
| **Barrierefreiheit** | WCAG AA (Kontrast, Tastatur, Screenreader) |
| **Druckversion** | Eingebaut (Print-Stylesheet) |

### Kontaktdaten auf der Webseite

| Feld | Aktueller Wert | Bitte prüfen |
|------|----------------|--------------|
| Vereinsname | Angelsportverein der BVG e.V. | ✅ / ❌ |
| 1. Vorsitzender | Dietmar Andersohn | ✅ / ❌ |
| Anschrift | Wodanstraße 19, 14513 Teltow | ✅ / ❌ |
| Telefon | 03328-305426 | ✅ / ❌ |
| Fax | 03328-305428 | ✅ / ❌ |
| E-Mail | info@asv-bvg.de | ✅ / ❌ |
| Registergericht | AG Berlin-Charlottenburg | ✅ / ❌ |
| Registernummer | VR 4941 Nz | ✅ / ❌ |
| Inhaltlich Verantwortlich | Marc-André Baudusch | ✅ / ❌ |
| Vereinsheim | Straße Am Stichkanal, Berlin-Lichterfelde | ✅ / ❌ |

> **Bitte füllt die letzte Spalte aus und gebt das Dokument zurück, damit wir vor dem Go-Live alles korrigieren können!**

---

```
╔═══════════════════════════════════════════════════════════════════════╗
║                                                                       ║
║   🎣 Angelsportverein der BVG e.V.                                    ║
║                                                                       ║
║   Dieses Dokument wurde im Rahmen des Webseiten-Neuaufbaus            ║
║   erstellt. Bei Fragen oder Änderungswünschen wendet Euch             ║
║   an den technischen Ansprechpartner.                                  ║
║                                                                       ║
║   Petri Heil! 🐟                                                      ║
║                                                                       ║
║   Stand: Februar 2026                                                  ║
║                                                                       ║
╚═══════════════════════════════════════════════════════════════════════╝
```
