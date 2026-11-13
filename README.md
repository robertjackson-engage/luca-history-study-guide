# Factory Tycoon — Luca's Unit 3 (Industrial Revolution)

History study game for Luca's Unit 3 test. Open `index.html` or visit the Pages URL.

Seven zones built from the Unit 3 study guide (all 20 terms, cause-and-effect chains, early vs later changes, working and living conditions, positive and negative effects, social classes, the big ideas, and a long answer workshop) plus a Boss Test that generates a fresh multiple-choice practice test.

## Updating

Edit `index.html`, then:

```bash
git commit -am "update" && git push
```

## Audio

Clips in `audio/` were pre-generated with ElevenLabs by `tools/gen_audio.py`; the site is static and contains no API key. To regenerate, put `ELEVENLABS_API_KEY=...` in a local gitignored `.env`, save `AUDIO_TEXTS()` from the browser console to `texts.json`, and run:

```bash
set -a && source .env && set +a && python3 tools/gen_audio.py texts.json
```
