# Transformative Gerechtigkeit Website - Anfängerleitfaden

## 📁 Struktur des Projekts

```
docs/
├── index.html                    (Landing Page - Startseite)
├── partnergewalt.html           (Was ist Partnergewalt?)
├── transformative-justice.html  (Was ist Transformative Justice?)
├── unser-prozess.html           (Unser Prozess + Blog + Download)
├── weiterführende-links.html    (Links und Ressourcen)
├── style.css                    (Alle Farben und Styles)
└── assets/
    └── Brief.docx              (Das Dokument zum Herunterladen)
```

---

## 🎨 Farben & Styling anpassen

Alle Farben sind in `style.css` oben definiert. Änderungen dort wirken sich auf **alle** Seiten aus:

```css
:root {
  --primary-purple: #A47FC7;    /* Hauptfarbe (Hintergrund) */
  --dark-purple: #6B4B7A;       /* Dunkles Lila (Überschriften) */
  --text-black: #000000;        /* Schwarze Textfarbe */
  --light-bg: #F9F7FA;          /* Heller Hintergrund für Boxen */
}
```

**Um Farben zu ändern:**
1. Öffne `style.css`
2. Ändere die Hex-Codes oben
3. Speichern → Alle Seiten zeigen die neuen Farben

---

## ✏️ Inhalte bearbeiten

### Text hinzufügen
Jede HTML-Datei hat Kommentare wie:
```html
<!-- BEARBEITE DIESEN TEXT: Füge hier deine Inhalte ein -->
```

Ersetze einfach den "Placeholder Text" darunter mit deinem echten Inhalt.

### Links hinzufügen
Suche nach `<a href="#">` und ersetze `#` durch die echte URL:
```html
<!-- VORHER: -->
<a href="#">Ressource 1 - Link einfügen</a>

<!-- NACHHER: -->
<a href="https://www.example.com">Ressource 1 - Schöner Name</a>
```

### Das Brief.docx hinzufügen
1. Kopiere deine `Brief.docx` in den `assets/` Ordner
2. Der Download-Button funktioniert dann automatisch

### Blog-Beiträge hinzufügen
Die 4 Karten auf `unser-prozess.html` sind Vorlagen. Für weitere Beiträge:
1. Kopiere eine der 4 Karten
2. Ändere den Titel und Text
3. (Optional: Später kannst du separate HTML-Dateien für längere Beiträge erstellen)

---

## 🌐 Auf GitHub Pages hosten

**Was ist GitHub Pages?**
GitHub Pages erlaubt dir, static HTML/CSS/JS kostenlos zu hosten – deine Website wird live im Internet verfügbar!

### Schritt 1: Repository klonen/setup
```
Du hast bereits: https://github.com/Widerstandsplenum/hexenzirkel
```

Wenn du noch nicht geklont hast:
```bash
git clone https://github.com/Widerstandsplenum/hexenzirkel
cd hexenzirkel
```

### Schritt 2: Dateien hochladen
1. **Kopiere die `docs/` Ordner** in dein `hexenzirkel` Repository
2. Nutze Git zu pushen:

```bash
git add .
git commit -m "Add website files"
git push origin main
```

### Schritt 3: GitHub Pages aktivieren
1. Gehe auf GitHub: https://github.com/Widerstandsplenum/hexenzirkel
2. Klick "Settings" (Zahnradsymbol oben rechts)
3. Links im Menü: "Pages"
4. Unter "Source" wähle: `main` branch und `/docs` folder
5. Speichern
6. Nach 1-2 Minuten: Deine Website ist live unter:
   ```
   https://widerstandsplenum.github.io/hexenzirkel/
   ```

---

## 🛠️ Häufige Anfängerfehler vermeiden

| Problem | Lösung |
|---------|--------|
| Bilder werden nicht angezeigt | Bilder in `assets/` Ordner legen, dann `<img src="assets/name.jpg">` |
| Links funktionieren nicht | Relativer Pfad verwenden: `href="partnergewalt.html"` nicht `href="/partnergewalt.html"` |
| CSS sieht anders aus | Cache löschen (Ctrl+Shift+Del) oder mit neuer Datei testen |
| GitHub Page wird nicht aktualisiert | Git Commit + Push machen, warten 2-5 Minuten |

---

## 📝 Bearbeiten ohne Terminal?

Du kannst auch direkt auf GitHub bearbeiten:
1. Gehe auf https://github.com/Widerstandsplenum/hexenzirkel
2. Navigiere zu `docs/` folder
3. Klick auf eine Datei
4. Klick "Edit" (Stift-Icon)
5. Ändere Text
6. "Commit changes" klicken

---

## 🎯 Nächste Schritte

1. **Inhalte füllen**: Ersetze alle "Placeholder Text" Abschnitte mit deinen Inhalten
2. **Links hinzufügen**: Sammle die Ressourcen-Links und trage sie ein
3. **Brief hochladen**: Kopiere `Brief.docx` in den `assets/` Ordner
4. **Bilder/Icons**: Wenn vorhanden, in `assets/` ablegen
5. **Auf GitHub pushen**: Folge Schritt 2-3 oben

---

## ❓ Fragen?

Diese Website nutzt:
- **HTML**: Struktur der Seiten
- **CSS**: Farben und Layout
- **Bootstrap**: Responsive Design (funktioniert auf Handy/Tablet/PC)
- **Vanilla JS**: Minimal – nur für Navigation nötig

Alles ist einfach und anfängerfreundlich gestaltet! 🎉
