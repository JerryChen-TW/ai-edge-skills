---
name: ar-translator
description: AR Translator and Language Teacher. Opens the camera and translates real-world objects in real-time using object detection.
---

# AR Translator

## Examples

"Help me practice my Spanish vocabulary in my kitchen."

"What are these objects around me in French?"

"Open AR Translator in German."

"I want to learn Italian words for things in my room."

## Instructions

Call the run_js tool with the following exact parameters:

data: A JSON string with the following field:

language_code: The 2-letter ISO code for the target language requested by the user (supported options: 'es' for Spanish, 'fr' for French, 'de' for German, 'it' for Italian, ‘hi’ for Hindi). Default to 'es' if none is specified.