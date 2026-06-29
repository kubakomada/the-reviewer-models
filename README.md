# the-reviewer-models

Static hosting (via jsDelivr) of the on-device speech-to-text model used by
**The Reviewer**'s recorded-interview practice. The model runs entirely in the
user's browser; this repo just serves the weights from a CORS-enabled CDN that
isn't blocked by VPNs/ad-blockers the way huggingface.co can be.

- `whisper-tiny.en/` — OpenAI Whisper tiny (English), ONNX, quantized (q8).
  Mirrored from [Xenova/whisper-tiny.en](https://huggingface.co/Xenova/whisper-tiny.en)
  (Apache-2.0). Only the q8 weights + tokenizer/config files are included.

Served at: `https://cdn.jsdelivr.net/gh/kubakomada/the-reviewer-models@v1/`
