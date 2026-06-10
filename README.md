# 🟢 Limevate KI-Akademie

Interaktives Lernportal für das Limevate-Gründerteam (Josh, Marv, Co-Chef) rund um KI-Management, Prompt Engineering, Automatisierung und deutsches KI-Recht.

## 🚀 Schnellstart

```bash
# Repository klonen
git clone https://github.com/DEIN-USERNAME/limevate-ki-akademie.git
cd limevate-ki-akademie

# Einfach index.html im Browser öffnen – kein Server nötig!
open index.html
```

Oder direkt auf GitHub Pages deployen (kostenlos):
1. Repo auf GitHub hochladen
2. Settings → Pages → Branch: main → Speichern
3. Fertig – unter `https://DEIN-USERNAME.github.io/limevate-ki-akademie` erreichbar

## 📁 Projektstruktur

```
limevate-ki-akademie/
├── index.html          # Hauptseite
├── assets/
│   └── styles.css      # Alle Styles (Light & Dark Mode)
├── src/
│   ├── data.js         # Alle Inhalte: Module, Tools, Recht, Quiz
│   └── app.js          # Anwendungslogik
└── README.md
```

## 📚 Inhalte

### 5 Lernmodule
| Modul | Level | Dauer |
|-------|-------|-------|
| Modul 1 – KI-Grundlagen | Einsteiger | 45 Min |
| Modul 2 – Prompt Engineering | Mittelstufe | 60 Min |
| Modul 3 – KI-Strategie im Unternehmen | Fortgeschritten | 75 Min |
| Modul 4 – KI-Agenten & Automatisierung | Fortgeschritten | 90 Min |
| Modul 5 – KI-Schulungen verkaufen | Business | 60 Min |

### Weitere Tabs
- **Team** – Profile für Josh, Marv und Co-Chef mit personalisierten Lernpfaden
- **KI-Tools** – 16 Tools in 4 Kategorien mit Empfehlungen
- **Recht** – EU AI Act, DSGVO, Haftung, Gründung (Deutschland)
- **Quiz** – 13 Fragen in 5 Kategorien mit sofortigem Feedback

## ✏️ Inhalte anpassen

Alle Lerninhalte, Quiz-Fragen und Rechtstexte befinden sich in `src/data.js`.

### Neue Quiz-Frage hinzufügen
```js
// In src/data.js → allQ Array
{ 
  l: 'mittel',           // 'einsteiger' | 'mittel' | 'profi' | 'recht' | 'business'
  q: "Deine Frage?", 
  opts: ["Option A", "Option B", "Option C", "Option D"], 
  c: 1,                  // Index der richtigen Antwort (0-3)
  e: "Erklärung warum die Antwort richtig ist." 
}
```

### Neues Modul hinzufügen
Neues Objekt in das `modules`-Array in `src/data.js` einfügen – der Rest wird automatisch gerendert.

## 🔗 Integration mit Claude

Die Buttons "Tiefer lernen" und "Lernplan erstellen" öffnen direkt Claude.ai mit vorausgefülltem Kontext. Zum Anpassen der Prompts: `openClaude(...)` Aufrufe in `index.html` und `src/app.js` bearbeiten.

## 🛠️ Technologie

- **Vanilla HTML/CSS/JS** – kein Framework, kein Build-Tool nötig
- **Tabler Icons** – via CDN (https://tabler.io/icons)
- **Dark Mode** – automatisch via `prefers-color-scheme`
- **Responsive** – funktioniert auf Mobile und Desktop

## 📜 Lizenz

MIT – frei nutzbar und anpassbar für Limevate und alle zukünftigen Kunden.

---

Made with ❤️ für das Limevate-Team · Josh · Marv · Co-Chef
