# Tamil ↔ Indian English Interpreter — Free V3.1

V3.1 improves translation without paid APIs.

Primary translation path on supported desktop Chrome:
- Chrome Translator API, on-device.
- Tamil (`ta`) is a supported language.
- No translation text is sent to a paid API once the local model is downloaded.

Fallback:
- Transformers.js + Xenova/nllb-200-distilled-600M runs in the browser.
- The model is downloaded from Hugging Face the first time it is needed and cached by the browser.
- This can be a large download and can use substantial RAM/CPU.

Speech:
- Browser SpeechRecognition: `en-IN` / `ta-IN`
- Browser/device SpeechSynthesis: prefers `en-IN` and `ta-IN`.

No OpenAI API key, paid API, or credit card is required.
