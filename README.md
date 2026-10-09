# Audio Prompt Generator — Referenz → Prompt

**DE** · [EN](#english)

Lädt einen Referenztrack, misst Tempo und Tonart lokal im Browser und lässt ein Audio-fähiges Modell über [OpenRouter](https://openrouter.ai) Genre, Instrumentierung, Groove und Produktion beschreiben. Heraus kommt ein fertiger Prompt für **Suno**, **Udio**, **Stable Audio**, **ACE-Step** oder als allgemeiner Fließtext.

- Eine einzelne HTML-Datei (`index.html`), kein Build, kein Server. Läuft lokal oder über GitHub Pages.
- Oberfläche auf Deutsch und Englisch (Umschalter oben rechts, Auswahl wird gemerkt, Direktlink mit `?lang=de` / `?lang=en`).
- Tempo über Spectral-Flux + Kammfilter, Tonart über Chroma + Krumhansl-Profile, inklusive Messsicherheit.
- An das Modell geht nur ein Ausschnitt (15/25/40 s, mono, 16 kHz) plus die Messwerte. BPM und Tonart darf es nicht überschreiben.
- Keine Künstlernamen im Output.

**Benutzung:** `index.html` öffnen, OpenRouter-API-Schlüssel eintragen, Audiodatei hineinziehen, Zielgenerator wählen, „Prompt erzeugen“.

Der Schlüssel wird nur an openrouter.ai gesendet und nur auf Wunsch im `localStorage` des Browsers gespeichert.

---

## English

Load a reference track, measure tempo and key locally in the browser, and let an audio-capable model on [OpenRouter](https://openrouter.ai) describe genre, instrumentation, groove and production. The output is a ready-to-use prompt for **Suno**, **Udio**, **Stable Audio**, **ACE-Step** or as general free text.

- A single HTML file (`index.html`): no build step, no server. Runs locally or on GitHub Pages.
- UI in German and English (switch at the top right, choice is remembered, direct link via `?lang=de` / `?lang=en`).
- Tempo via spectral flux + comb filter, key via chroma + Krumhansl profiles, including measurement confidence.
- Only an excerpt (15/25/40 s, mono, 16 kHz) plus the measurements is sent to the model, which may not override BPM and key.
- No artist names in the output.

**Usage:** open `index.html`, enter your OpenRouter API key, drop in an audio file, pick the target generator, click "Generate prompt".

The key is only sent to openrouter.ai and is only stored in the browser's `localStorage` if you opt in.

## License

Apache 2.0, see [LICENSE](LICENSE).
