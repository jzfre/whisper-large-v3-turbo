# Whisper and pyannote model files

Public mirror of `config.json` and `model.safetensors` from
[openai/whisper-large-v3-turbo on Hugging Face](https://huggingface.co/openai/whisper-large-v3-turbo).

Upstream revision: `41f01f3fe87f28c78e2fbf8b568835947dd65ed9`.
The files are copied without modification and retain their original names.

## Download

- [config.json](https://github.com/jzfre/whisper-large-v3-turbo/releases/download/hf-41f01f3/config.json)
- [model.safetensors](https://github.com/jzfre/whisper-large-v3-turbo/releases/download/hf-41f01f3/model.safetensors) — 1,617,824,864 bytes
- [SHA256SUMS](https://github.com/jzfre/whisper-large-v3-turbo/releases/download/hf-41f01f3/SHA256SUMS)
- [MIT license](https://github.com/jzfre/whisper-large-v3-turbo/blob/main/LICENSE)

The model weights are hosted as a GitHub Release asset. No authentication is
required to download public release assets. `config.json` is also included
in this repository.

To check downloaded files on macOS:

```sh
shasum -a 256 -c SHA256SUMS
```

The Whisper mirror contains only the two requested model files. A complete local
Transformers inference setup also needs the tokenizer and processor files
from the upstream model repository.

## Attribution

The original model is published by OpenAI under the MIT license. See
[LICENSE](LICENSE). This is an independent mirror, not an official OpenAI repository.

## Pyannote speaker diarization Community-1

- [Download the complete model bundle (ZIP, 31.3 MB)](https://github.com/jzfre/whisper-large-v3-turbo/releases/download/pyannote-community-1-hf-3533c8c/pyannote-speaker-diarization-community-1.zip)
- [Archive SHA256 checksum](https://github.com/jzfre/whisper-large-v3-turbo/releases/download/pyannote-community-1-hf-3533c8c/pyannote-SHA256SUMS)
- [Release and usage notes](https://github.com/jzfre/whisper-large-v3-turbo/releases/tag/pyannote-community-1-hf-3533c8c)

Source: [pyannote/speaker-diarization-community-1](https://huggingface.co/pyannote/speaker-diarization-community-1), revision `3533c8cf8e369892e6b79ff1bf80f7b0286a54ee`.
All 10 upstream files are preserved, including `config.yaml`, segmentation weights,
speaker embedding weights, and PLDA files. Extract the ZIP to preserve their directory structure.

```python
from pyannote.audio import Pipeline
pipeline = Pipeline.from_pretrained("/path/to/pyannote-speaker-diarization-community-1")
```

The config declares `pyannote.audio` 4.0.0. Python dependencies and FFmpeg/TorchCodec
libraries are not included. Archive integrity and upstream file hashes were verified;
inference was not run as part of mirroring.

The pyannote bundle is published by pyannote under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/),
separately from the Whisper MIT license above. Original attribution, model cards,
and citations are included, along with the license text, provenance manifest, and checksums.
The upstream files are unmodified. This is an independent mirror and is not endorsed by pyannote.
