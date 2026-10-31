# chatpet models

Model files downloaded by [chatpet](https://github.com/reezex0-ux/chatpet-releases) on first run.

**Powered by Kanana**

## kanana2-3b-q5km-v1

`kanana2-3b-q5_k_m.gguf` (2,512,164,736 bytes), split into two parts because GitHub Releases allows at most 2 GiB per file.

| file | bytes | SHA-256 |
| - | - | - |
| kanana2-3b-q5_k_m.gguf.part1 | 1,300,000,000 | ce43c33051ba529815df8bda434af14f1bfd53cb3ba66603510046a3f4342800 |
| kanana2-3b-q5_k_m.gguf.part2 | 1,212,164,736 | 70b087c5c6cd349ca54af777c889b536cb85ee041419365bf6b16aa8df574c22 |
| joined `kanana2-3b-q5_k_m.gguf` | 2,512,164,736 | 7933fa2ab32a1d1cdb143357b6cb49ef52d0d41f56395df00f301b8d71d8d68d |

To join them by hand:

```
copy /b kanana2-3b-q5_k_m.gguf.part1 + kanana2-3b-q5_k_m.gguf.part2 kanana2-3b-q5_k_m.gguf
```

### Source and modification

- Original: [kakaocorp/kanana-2-3b-instruct](https://huggingface.co/kakaocorp/kanana-2-3b-instruct), revision `6a5d7889964c4c590299d16e309eabab1f73f8a9`.
- **Modified**: converted to GGUF (f16) with llama.cpp b11624 `convert_hf_to_gguf.py`, then quantized to Q5_K_M with `llama-quantize`. It is not the original file.

### License

Kanana is licensed in accordance with the Kanana Open License Agreement. Copyright © KAKAO Corp. All Rights Reserved.

The full agreement is in [LICENSE.md](LICENSE.md); notices in [NOTICE.txt](NOTICE.txt). Use of this model and its derivatives must comply with applicable laws and KAKAO's Guidelines For Responsible AI, and these restrictions apply to everyone who receives it (Agreement 2.2, 3.1(i)).
