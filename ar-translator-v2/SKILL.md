---
name: ar-translator-v2
description: AR Translator v2 with higher accuracy model (EfficientDet-Lite2). Opens the camera and translates real-world objects in real-time using on-device object detection.
---

## Instructions

This skill opens a fullscreen camera view and uses on-device object detection (MediaPipe EfficientDet-Lite2) to identify real-world objects, displaying their translated names as an AR overlay in real-time. Higher accuracy than v1.

### How to open

When invoked, open the webview at `assets/webview.html` and **always append the correct `?lang=` query parameter** based on the user's requested language. Do NOT open without the `?lang=` parameter.

### Language parameter mapping

Detect the target language from the user's message and use the corresponding code:

| User says | Lang code | Open URL |
|-----------|-----------|----------|
| Spanish / español | `es` | `assets/webview.html?lang=es` |
| French / français | `fr` | `assets/webview.html?lang=fr` |
| German / Deutsch | `de` | `assets/webview.html?lang=de` |
| Italian / italiano | `it` | `assets/webview.html?lang=it` |
| Hindi / हिन्दी | `hi` | `assets/webview.html?lang=hi` |

If no language is specified, default to Spanish: `assets/webview.html?lang=es`

### Example prompts and expected behavior

- "Open AR Translator in Spanish" → open `assets/webview.html?lang=es`
- "What are these objects in French?" → open `assets/webview.html?lang=fr`
- "Open AR Translator in German" → open `assets/webview.html?lang=de`
- "I want to learn Italian words for things in my room" → open `assets/webview.html?lang=it`
- "Open AR Translator in Hindi" → open `assets/webview.html?lang=hi`
