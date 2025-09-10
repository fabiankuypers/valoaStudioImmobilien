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

### **Character Sheet Prompts für "Marc" (Immobilienmakler):**

```
MASTER PROMPT (für Midjourney):
"Professional real estate agent Marc, 35-40 years old, short dark hair with slight gray temples, friendly face, wearing white business shirt and dark pants, clean modern style, character sheet showing front view, side profile, and 3/4 angle, consistent lighting, white background --style raw --ar 16:9 --v 6"
```

### **Variationen für Character Sheet:**

**1. Basis-Referenzbilder:**
```
"Marc the real estate agent, front view, neutral expression, white business shirt, dark pants --style raw --ar 1:1"

"Marc the real estate agent, side profile, same clothing, consistent style --style raw --ar 1:1"

"Marc the real estate agent, 3/4 angle, slight smile, same styling --style raw --ar 1:1"
```

**2. Emotionale Varianten:**
```
"Marc looking frustrated and stressed, sitting at desk, same character design --style raw --ar 16:9"

"Marc looking tired and overwhelmed, same character, consistent styling --style raw --ar 16:9"

"Marc happy and confident, same character design, triumphant expression --style raw --ar 16:9"
```

**3. Situative Posen:**
```
"Marc talking on phone, professional posture, same character design --style raw --ar 16:9"

"Marc in car driving, same character, through windshield view --style raw --ar 16:9"

"Marc shaking hands with clients, same character design --style raw --ar 16:9"
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

### **UNIVERSELLE CHARAKTER-BESCHREIBUNG:**
```
"Marc, professional real estate agent, 35-40 years old, short dark hair with gray temples, friendly face, white business shirt, dark pants"
```

### **CLIP-SPEZIFISCHE PROMPTS:**

**Clip 1: Gestresster Marc am Schreibtisch**
```
"Marc, professional real estate agent, 35-40 years old, short dark hair with gray temples, friendly face, white business shirt, dark pants, sitting frustrated at modern office desk with computer and ringing phone, stress visible on face, 2D animation style, clean modern office background, smooth camera movement, 8 seconds, 1920x1080"
```

**Clip 2: Marc bei Telefonaten**
```
"Marc, professional real estate agent, 35-40 years old, short dark hair with gray temples, friendly face, white business shirt, dark pants, talking on phone while taking notes, looking increasingly tired, same office setting as previous clip, 2D animation style, consistent lighting, 8 seconds"
```

**Clip 3: Marc beim Autofahren**
```
"Marc, professional real estate agent, 35-40 years old, short dark hair with gray temples, friendly face, white business shirt, dark pants, driving car between different house viewings, view from passenger seat showing his profile, multiple houses in background, 2D animation style, daytime lighting, 8 seconds"
```

### **KONSISTENZ-REGELN FÜR ALLE CLIPS:**

1. **NIEMALS die Grundbeschreibung ändern**
2. **Identische Kleidung in jedem Prompt**
3. **Konsistente Alters- und Aussehen-Beschreibung**
4. **Gleicher Stil-Marker: "2D animation style"**
5. **Bei Problemen: Referenzbild aus Phase 1 hochladen**

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

## **ERWARTUNGSMANAGEMENT**

### **Realistische Ergebnisse:**
- **80-90% Charakterkonsistenz** bei sorgfältiger Umsetzung
- **2-3 Re-Rolls** pro Clip normal
- **Gesamtproduktionszeit:** 15-20 Stunden
- **Qualität:** Professionell, aber erkennbar KI-generiert

### **Wenn perfekte Konsistenz kritisch ist:**
- **Hybrid-Ansatz:** Beste Clips aus Veo3 + manuelle Touch-ups
- **Alternative:** RunwayML Act-Two für kritische Szenen
- **Budget-Option:** Statische Frames + einfache Animation

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