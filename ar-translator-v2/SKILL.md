---
name: ar-translator-v2
description: AR Translator v2 with higher accuracy model (EfficientDet-Lite2). Opens the camera and translates real-world objects in real-time using on-device object detection.
js:
  path: scripts/index.html
  output_type: webview
---

## Instructions

This skill opens a fullscreen camera view and uses on-device object detection (MediaPipe EfficientDet-Lite2) to identify real-world objects, displaying their translated names as an AR overlay in real-time.

Call the `run_js` tool with the following exact parameters:

- data: A JSON string with the following field:
  - `target_language`: The language code for translation.

### Language code mapping

| User says | `target_language` value |
|-----------|------------------------|
| Spanish / español | `es` |
| French / français | `fr` |
| German / Deutsch | `de` |
| Italian / italiano | `it` |
| Hindi / हिन्दी | `hi` |

If no language is specified, default to `es` (Spanish).

## Examples

- "Open AR Translator in Spanish"
- "What are these objects in French?"
- "Open AR Translator in German"
- "I want to learn Italian words for things in my room"
- "Open AR Translator in Hindi"
