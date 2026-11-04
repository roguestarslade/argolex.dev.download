# Argolex model downloads

Release `v1.0` (release/1.0): the model files the Argolex app downloads at first run.

**These files are fetched by the Argolex app, not cloned.** The models are Release assets only; this repository holds just `manifest.json` (path, asset name, bytes, sha256 and URL for every file), the licences and this readme. Do not commit model files here.

67 files, 1.3 GB (1,385,852,670 bytes) in all.

## Licences

| Model | Licence | Licence file |
|---|---|---|
| Kokoro-82M | Apache-2.0 | `LICENSES/kokoro/` |
| Qwen3.5 | Apache-2.0 | `LICENSES/qwen3.5/` |
| Moonshine | MIT | `LICENSES/moonshine/` |
| Silero VAD | MIT | `LICENSES/silero-vad/` |

### Licence file missing

None. Every model has a licence file under `LICENSES/`:

- Kokoro-82M: the upstream model card (`license: apache-2.0`), copied from the local model folder; the upstream licence field on https://huggingface.co/hexgrad/Kokoro-82M also reads apache-2.0 (checked 2026-11-03).
- Qwen3.5: no licence file in the local model folder; the upstream licence field on https://huggingface.co/Qwen/Qwen3.5-0.8B reads apache-2.0 (checked 2026-11-03), so `LICENSES/qwen3.5/LICENSE` is the canonical Apache License 2.0 text (source in `LICENSES/qwen3.5/SOURCE.md`).
- Moonshine and Silero VAD: the LICENSE files shipped next to the models.

## Files

| File | What it is | Size | Licence |
|---|---|---|---|
| `kokoro/config.json` | Kokoro-82M model config (phoneme vocabulary, hyperparameters) | 2.3 KB | Apache-2.0 |
| `kokoro/onnx/model_fp16_nanfix_emo.onnx` | Kokoro-82M TTS, ONNX fp16 (NaN-fixed, emotion inputs) | 155.7 MB | Apache-2.0 |
| `kokoro/onnx/model_emo.onnx` | Kokoro-82M TTS, ONNX fp32 (emotion inputs) | 310.5 MB | Apache-2.0 |
| `kokoro/voices/af_alloy.bin` | Kokoro voice `af_alloy` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/af_aoede.bin` | Kokoro voice `af_aoede` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/af_bella.bin` | Kokoro voice `af_bella` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/af_heart.bin` | Kokoro voice `af_heart` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/af_jessica.bin` | Kokoro voice `af_jessica` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/af_kore.bin` | Kokoro voice `af_kore` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/af_nicole.bin` | Kokoro voice `af_nicole` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/af_nova.bin` | Kokoro voice `af_nova` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/af_river.bin` | Kokoro voice `af_river` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/af_sarah.bin` | Kokoro voice `af_sarah` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/af_sky.bin` | Kokoro voice `af_sky` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/am_adam.bin` | Kokoro voice `am_adam` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/am_echo.bin` | Kokoro voice `am_echo` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/am_eric.bin` | Kokoro voice `am_eric` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/am_fenrir.bin` | Kokoro voice `am_fenrir` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/am_liam.bin` | Kokoro voice `am_liam` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/am_michael.bin` | Kokoro voice `am_michael` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/am_onyx.bin` | Kokoro voice `am_onyx` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/am_puck.bin` | Kokoro voice `am_puck` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/am_santa.bin` | Kokoro voice `am_santa` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/bf_alice.bin` | Kokoro voice `bf_alice` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/bf_emma.bin` | Kokoro voice `bf_emma` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/bf_isabella.bin` | Kokoro voice `bf_isabella` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/bf_lily.bin` | Kokoro voice `bf_lily` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/bm_daniel.bin` | Kokoro voice `bm_daniel` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/bm_fable.bin` | Kokoro voice `bm_fable` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/bm_george.bin` | Kokoro voice `bm_george` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/bm_lewis.bin` | Kokoro voice `bm_lewis` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/ef_dora.bin` | Kokoro voice `ef_dora` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/em_alex.bin` | Kokoro voice `em_alex` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/em_santa.bin` | Kokoro voice `em_santa` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/ff_siwis.bin` | Kokoro voice `ff_siwis` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/hf_alpha.bin` | Kokoro voice `hf_alpha` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/hf_beta.bin` | Kokoro voice `hf_beta` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/hm_omega.bin` | Kokoro voice `hm_omega` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/hm_psi.bin` | Kokoro voice `hm_psi` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/if_sara.bin` | Kokoro voice `if_sara` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/im_nicola.bin` | Kokoro voice `im_nicola` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/jf_alpha.bin` | Kokoro voice `jf_alpha` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/jf_gongitsune.bin` | Kokoro voice `jf_gongitsune` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/jf_nezumi.bin` | Kokoro voice `jf_nezumi` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/jf_tebukuro.bin` | Kokoro voice `jf_tebukuro` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/jm_kumo.bin` | Kokoro voice `jm_kumo` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/pf_dora.bin` | Kokoro voice `pf_dora` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/pm_alex.bin` | Kokoro voice `pm_alex` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/pm_santa.bin` | Kokoro voice `pm_santa` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/zf_xiaobei.bin` | Kokoro voice `zf_xiaobei` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/zf_xiaoni.bin` | Kokoro voice `zf_xiaoni` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/zf_xiaoxiao.bin` | Kokoro voice `zf_xiaoxiao` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/zf_xiaoyi.bin` | Kokoro voice `zf_xiaoyi` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/zm_yunjian.bin` | Kokoro voice `zm_yunjian` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/zm_yunxi.bin` | Kokoro voice `zm_yunxi` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/zm_yunxia.bin` | Kokoro voice `zm_yunxia` (style vectors) | 510.0 KB | Apache-2.0 |
| `kokoro/voices/zm_yunyang.bin` | Kokoro voice `zm_yunyang` (style vectors) | 510.0 KB | Apache-2.0 |
| `qwen3.5-gguf/Qwen_Qwen3.5-0.8B-Q4_K_M.gguf` | Qwen3.5 0.8B LLM, GGUF Q4_K_M (llama.cpp) | 552.8 MB | Apache-2.0 |
| `moonshine/base-en-int8/LICENSE` | Moonshine licence (MIT) | 1.0 KB | MIT |
| `moonshine/base-en-int8/README.md` | Moonshine folder readme (upstream source and licence link) | 175 B | MIT |
| `moonshine/base-en-int8/SOURCE.txt` | Moonshine provenance notes | 2.0 KB | MIT |
| `moonshine/base-en-int8/cached_decode.int8.onnx` | Moonshine base (English) speech-to-text: decoder with KV cache, int8 | 95.4 MB | MIT |
| `moonshine/base-en-int8/encode.int8.onnx` | Moonshine base (English) speech-to-text: encoder, int8 | 48.0 MB | MIT |
| `moonshine/base-en-int8/preprocess.onnx` | Moonshine base (English) speech-to-text: audio preprocessor | 13.4 MB | MIT |
| `moonshine/base-en-int8/tokens.txt` | Moonshine tokenizer vocabulary | 426.5 KB | MIT |
| `moonshine/base-en-int8/uncached_decode.int8.onnx` | Moonshine base (English) speech-to-text: first-step decoder, int8 | 116.5 MB | MIT |
| `silero-vad/silero_vad.onnx` | Silero VAD voice-activity detector, ONNX | 2.2 MB | MIT |

Asset names are the path with `/` replaced by `--`, e.g. `kokoro--voices--af_heart.bin`; download URLs are `https://github.com/roguestarslade/argolex.dev.download/releases/download/v1.0/<asset>`.
