# Whisper large-v3-turbo model files

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

This mirror contains only the two requested model files. A complete local
Transformers inference setup also needs the tokenizer and processor files
from the upstream model repository.

## Attribution

The original model is published by OpenAI under the MIT license. See
[LICENSE](LICENSE). This is an independent mirror, not an official OpenAI repository.
