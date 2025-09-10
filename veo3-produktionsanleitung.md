# Veo3 Produktionsanleitung: Charakterkonsistente Erklärvideos

## **ÜBERSICHT: Der 4-Phasen-Workflow**

Basierend auf der Forschung zu KI-Videogenerierung und den technischen Beschränkungen von Veo3 (8-Sekunden-Clips) verwenden wir einen **hybriden Ansatz** für maximale Charakterkonsistenz.

---

## **PHASE 1: CHARACTER SHEET ERSTELLEN** 
*[Vorbereitung - ca. 2 Stunden]*

### **Ziel:** Solide visuelle Grundlage für konsistente Charaktere

### **Tools:**
- **Midjourney** (empfohlen) oder Adobe Firefly
- **Alternative:** DALL-E 3, Stable Diffusion

### **Character Sheet Prompts für "Marc" (Zeichentrick-Immobilienmakler):**

```
MASTER PROMPT (für Midjourney):
"2D cartoon character Marc, friendly real estate agent, simple cartoon style like Dropbox explainer videos, clean vector art, 35-40 years old, short dark hair, big expressive eyes, wearing simple white business shirt, mobile-friendly design, character sheet showing front view, side profile, and 3/4 angle, flat colors, white background --style raw --ar 9:16 --v 6 --niji 6"
```

### **Variationen für Character Sheet:**

**1. Basis-Referenzbilder (Zeichentrick):**
```
"2D cartoon Marc, front view, neutral expression, simple vector style like Slack animations, white business shirt, big eyes, mobile-friendly --style raw --ar 9:16 --niji 6"

"2D cartoon Marc, side profile, same cartoon character, consistent flat color style --style raw --ar 9:16 --niji 6"

"2D cartoon Marc, 3/4 angle, slight smile, same vector design, explainer video style --style raw --ar 9:16 --niji 6"
```

**2. Emotionale Varianten (für Mobile lesbar):**
```
"2D cartoon Marc looking shocked and frustrated, sitting at modern desk, exaggerated cartoon expressions, big eyes wide, same character design --style raw --ar 9:16 --niji 6"

"2D cartoon Marc looking tired and overwhelmed, same vector character, droopy cartoon eyes, consistent styling --style raw --ar 9:16 --niji 6"

"2D cartoon Marc happy and celebrating, same character design, big cartoon smile, arms raised triumphantly --style raw --ar 9:16 --niji 6"
```

**3. Situative Posen (9:16 optimiert):**
```
"2D cartoon Marc talking on phone, sitting at desk, phone clearly visible, same vector character design, vertical composition --style raw --ar 9:16 --niji 6"

"2D cartoon Marc driving car, view through windshield, same cartoon character, simple background, mobile-optimized --style raw --ar 9:16 --niji 6"

"2D cartoon Marc shaking hands with cartoon clients, same character design, friendly business scene, vertical frame --style raw --ar 9:16 --niji 6"
```

### **Qualitätskontrolle:**
- **Konsistenz prüfen:** Alle Bilder zeigen identisches Gesicht, Frisur, Kleidung
- **20-30 Bilder sammeln:** Verschiedene Winkel, Emotionen, Situationen
- **Beste 15-20 auswählen:** Hohe Qualität, klare Erkennbarkeit

---

## **PHASE 2: VEO3 PROMPTING-STRATEGIE**
*[Pro Clip - ca. 15 Minuten]*

### **Veo3 Charakterkonsistenz-Hack:**

**Jeder Prompt MUSS folgende Struktur haben:**
1. **Charakter-Beschreibung** (identisch in jedem Prompt!)
2. **Spezifische Aktion** (für diesen Clip)
3. **Setting/Umgebung**
4. **Stil-Anweisungen**
5. **Technische Parameter**

### **UNIVERSELLE CHARAKTER-BESCHREIBUNG (ZEICHENTRICK):**
```
"2D cartoon Marc, friendly real estate agent, simple vector style like Dropbox animations, 35-40 years old, short dark hair, big expressive eyes, white business shirt, clean cartoon design"
```

### **CLIP-SPEZIFISCHE PROMPTS (9:16 + LINKEDIN-OPTIMIERT):**

**Clip 1: LinkedIn-Hook mit ChatGPT-Bezug**
```
"2D cartoon Marc, friendly real estate agent, simple vector style like Dropbox animations, 35-40 years old, short dark hair, big expressive eyes, white business shirt, clean cartoon design, sitting at desk looking curious about ChatGPT on computer screen, 2D explainer video style, mobile-friendly vertical composition, 8 seconds, 1080x1920"
```

**Clip 2: Schockierend niedrige Abschlussquote**
```
"2D cartoon Marc, friendly real estate agent, simple vector style like Dropbox animations, 35-40 years old, short dark hair, big expressive eyes, white business shirt, clean cartoon design, looking shocked at computer showing '12% success rate', exaggerated cartoon expression, same office setting, 2D animation style, large text visible on mobile, 8 seconds"
```

**Clip 3: ChatGPT Interface zeigt niedrige Quote**
```
"2D cartoon style ChatGPT interface showing '12% success rate' with cartoon Marc looking disappointed, simple vector graphics, mobile-readable text, explainer video style, consistent character design as previous clips, vertical 9:16 composition, 6 seconds"
```

### **KONSISTENZ-REGELN FÜR ALLE CLIPS (MOBILE + ZEICHENTRICK):**

1. **NIEMALS die Grundbeschreibung ändern**
2. **Immer "2D cartoon" und "vector style" erwähnen**
3. **Konsistente "big expressive eyes" für mobile Lesbarkeit**
4. **9:16 Format IMMER: "vertical composition, 1080x1920"**
5. **LinkedIn-Context beibehalten wo relevant**
6. **Bei Problemen: Zeichentrick-Referenzbild aus Phase 1 hochladen**

---

## **PHASE 3: CLIP-GENERIERUNG UND QUALITÄTSKONTROLLE**
*[Pro Clip - ca. 20-30 Minuten]*

### **Workflow für jeden der 14 Clips:**

**Schritt 1: Prompt eingeben**
- Exakten Prompt aus Phase 2 verwenden
- Optional: Referenzbild aus Character Sheet hochladen

**Schritt 2: Erste Generation prüfen**
- ✅ **Charakterkonsistenz:** Sieht Marc identisch aus?
- ✅ **Aktion stimmt:** Macht er was gewünscht?
- ✅ **Qualität:** Keine Artefakte, glatte Animation?

**Schritt 3: Bei Inkonsistenz - Re-Roll Strategie**
```
WENN Charakter inkonsistent:
1. Prompt mit zusätzlichen Details anreichern
2. Referenzbild aus Phase 1 hochladen
3. "Consistency: high" oder ähnliches hinzufügen
4. Maximal 3 Versuche pro Clip
```

**Schritt 4: Backup-Strategie bei wiederholtem Versagen**
- **Plan B:** Statisches Keyframe aus Phase 1 + Runway Gen-3 für Animation
- **Plan C:** Midjourney für einzelne Frames + After Effects für Bewegung

---

## **PHASE 4: POST-PRODUCTION ASSEMBLY**
*[Finaler Schnitt - ca. 3-4 Stunden]*

### **Tools:**
- **Primary:** DaVinci Resolve (kostenlos) oder Adobe Premiere Pro
- **Audio:** ElevenLabs für Voice-over
- **Musik:** Beatoven.ai oder Epidemic Sound

### **Assembly-Workflow:**

**1. Clip-Sequencing:**
- 14 Clips in chronologischer Reihenfolge
- Jeweils 6-8 Sekunden (für Pacing-Kontrolle)
- Sanfte Übergänge (0.2s Cross-Fade)

**2. Audio-Layer:**
```
Track 1: Voice-over (ElevenLabs generiert)
Track 2: Hintergrundmusik (Beatoven.ai, 20% Lautstärke)
Track 3: Sound Effects (optional, Freesound.org)
```

**3. Text/Graphics Overlay:**
- Clip 6: "40h" und "€8.700" Animation
- Clip 11: Statistiken als Motion Graphics  
- Clip 13-14: CTA Button und "Nur noch 3 Plätze"

**4. Farbkorrektur:**
- Einheitliche Farbtemperatur über alle Clips
- Leichte Sättigung für professionellen Look
- Konsistente Belichtung

---

## **KONSISTENZ-TIPPS FÜR VEO3**

### **✅ DO's:**

1. **Identische Beschreibung:** Kopiere die Charakter-Beschreibung 1:1 in jeden Prompt
2. **Referenzbilder verwenden:** Upload aus Phase 1 bei kritischen Clips
3. **Sequentielle Generation:** Einen Clip nach dem anderen (nicht parallel)
4. **Konsistenz-Check:** Jeder neue Clip mit vorherigem vergleichen
5. **Backup-Plan:** Alternative Generatoren bereithalten

### **❌ DON'Ts:**

1. **Beschreibung variieren:** Selbst kleine Änderungen können Charakter ändern
2. **Zu komplexe Prompts:** Veo3 bevorzugt klare, strukturierte Anweisungen  
3. **Emotionen im Charakter:** Besser separate "emotion: frustrated" Parameter
4. **Kleidung ändern:** Konstante Kleidung = bessere Erkennbarkeit
5. **Batch-Generation:** Erhöht Inkonsistenz-Risiko

---

## **TROUBLESHOOTING HÄUFIGER PROBLEME**

### **Problem: Gesicht ändert sich zwischen Clips**
**Lösung:**
- Referenzbild aus Phase 1 hochladen
- Prompt um Gesichtsbeschreibung erweitern: "same face as reference image"
- Lighting-Konsistenz prüfen: "consistent lighting"

### **Problem: Kleidung wird anders dargestellt**
**Lösung:**
- Kleidungsbeschreibung detaillierter: "exact same white business shirt, dark formal pants"
- Vollbody-Shots vermeiden, auf Medium-Shots fokussieren

### **Problem: Animation-Stil inkonsistent**
**Lösung:**
- Style-Marker verstärken: "2D animated explainer video style, consistent with previous clips"
- Reference-Style aus erfolgreichem Clip verwenden

### **Problem: Hintergrund/Setting ändert sich**
**Lösung:**
- Setting in jedem Prompt erwähnen
- "Same office/car/location as previous clip" hinzufügen

---

## **QUALITÄTSSICHERUNG CHECKLIST**

### **Vor Abschluss prüfen:**

**Charakterkonsistenz:**
- [ ] Marc sieht in allen 14 Clips identisch aus
- [ ] Kleidung ist konsistent
- [ ] Gesichtszüge bleiben erhalten
- [ ] Alterserscheinung konstant

**Narrative Kohärenz:**
- [ ] Emotionale Journey funktioniert (frustriert → erfolgreich)
- [ ] Alle Szenen des Skripts abgedeckt
- [ ] Timing stimmt (90 Sekunden Gesamtlänge)
- [ ] CTA ist klar und deutlich

**Technische Qualität:**
- [ ] Alle Clips 1920x1080 oder höher
- [ ] Keine sichtbaren Artefakte
- [ ] Audio synchron zu Video
- [ ] Übergänge sind smooth

---

## **MOBILE-FIRST BESONDERHEITEN (LINKEDIN-TRAFFIC)**

### **Kritische Mobile-Optimierungen:**
- **Text-Größe:** Minimum 24px für mobile Lesbarkeit
- **Kontrast:** Hoher Kontrast zwischen Text und Hintergrund
- **Animationsgeschwindigkeit:** Langsamer als Desktop (mobile Verarbeitung)
- **Erste 3 Sekunden:** Hook muss auf 5-Zoll-Screen funktionieren
- **Vertikaler Fokus:** Wichtige Elemente in oberen 2/3 des Frames

### **LinkedIn-Spezifische Anpassungen:**
- **Referenz auf "ChatGPT-Tipps" in ersten 5 Sekunden**
- **CTA zeigt nach unten** (zu Kommentaren/Link)
- **Professioneller Ton** (LinkedIn-Audience)
- **Zahlen groß und prominent** (mobile Sichtbarkeit)

---

## **ERWARTUNGSMANAGEMENT**

### **Realistische Ergebnisse (Mobile + Zeichentrick):**
- **85-95% Charakterkonsistenz** bei Zeichentrick (einfacher als Photorealismus)
- **1-2 Re-Rolls** pro Clip (Cartoon-Stil verzeiht mehr)
- **Gesamtproduktionszeit:** 12-15 Stunden
- **Qualität:** Professionell, Zeichentrick-Stil verschleiert KI-Artefakte

### **Wenn perfekte Konsistenz kritisch ist:**
- **Vorteil Zeichentrick:** Weniger "Uncanny Valley" als Photorealismus
- **Backup:** Statische Zeichentrick-Frames + After Effects Animation
- **Alternative:** Lottie-Files für Web-optimierte Vektoranimationen

---

## **BUDGET & TIMELINE**

### **Kosten-Übersicht:**
- **Midjourney:** ~$30/Monat (Character Sheet)
- **Veo3:** ~$50-100 (14 Clips mit Re-Rolls)
- **ElevenLabs:** ~$22/Monat (Voice-over)
- **Beatoven.ai:** ~$25/Monat (Musik)
- **GESAMT:** ~$150-200

### **Timeline:**
- **Tag 1:** Character Sheet erstellen (2-3h)
- **Tag 2-3:** Clip-Generierung (6-8h)
- **Tag 4:** Post-Production (3-4h)
- **GESAMT:** 4 Tage (bei Vollzeit)

---

Mit diesem Workflow erreichen Sie **professionelle Erklärvideo-Qualität** mit **maximaler Charakterkonsistenz** innerhalb des Veo3-Frameworks. Die Kombination aus strategischem Character Design, präzisem Prompting und sorgfältiger Post-Production überwindet die technischen Limitierungen aktueller KI-Videotools.