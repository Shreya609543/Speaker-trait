---
layout: home
title: "SpeakerShift: Embedding-Space Speaker Trait Conversion"
---

<style>
table { width: 100%; border-collapse: collapse; font-size: 0.9em; margin-bottom: 1.5em; }
th { background: #f4f4f4; text-align: center; padding: 0.5em 0.75em; border: 1px solid #ddd; font-weight: 600; }
td { text-align: center; padding: 0.5em 0.75em; border: 1px solid #ddd; vertical-align: middle; }
td:first-child { text-align: left; font-weight: 500; }
audio { width: 200px; }
.section-note { font-size: 0.85em; color: #555; margin: -0.5em 0 1em 0; }
</style>

**Interspeech 2025** · [Paper](#) · [Code](#) · [Citation](#citation)

---

We propose **HybridAttentionMapper**, a 21.7M-parameter neural network that re-maps speaker identity embeddings across a static trait boundary (gender) while preserving linguistic content. Below we compare the **ground truth (source)** against our **Hybrid system** across two conversion directions, four corpora, and both accent groups.

---

## Female → Male

### VCTK — British English

| Speaker | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|
| p268 (F) | <audio controls><source src="samples/vctk/p268_utt01_source.wav"></audio> | <audio controls><source src="samples/vctk/p268_utt01_hybrid.wav"></audio> |
| p268 (F) | <audio controls><source src="samples/vctk/p268_utt02_source.wav"></audio> | <audio controls><source src="samples/vctk/p268_utt02_hybrid.wav"></audio> |
| p268 (F) | <audio controls><source src="samples/vctk/p268_utt03_source.wav"></audio> | <audio controls><source src="samples/vctk/p268_utt03_hybrid.wav"></audio> |

### L2-ARTIC — Hindi L2

| Speaker | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|
| SVBI (F) | <audio controls><source src="samples/l2artic/SVBI_utt01_source.wav"></audio> | <audio controls><source src="samples/l2artic/SVBI_utt01_hybrid.wav"></audio> |
| SVBI (F) | <audio controls><source src="samples/l2artic/SVBI_utt02_source.wav"></audio> | <audio controls><source src="samples/l2artic/SVBI_utt02_hybrid.wav"></audio> |
| SVBI (F) | <audio controls><source src="samples/l2artic/SVBI_utt03_source.wav"></audio> | <audio controls><source src="samples/l2artic/SVBI_utt03_hybrid.wav"></audio> |

### LibriTTS — English

| Speaker | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|
| 1320 | <audio controls><source src="samples/libri/1320_utt01_source.wav"></audio> | <audio controls><source src="samples/libri/1320_utt01_hybrid.wav"></audio> |
| 2961 | <audio controls><source src="samples/libri/2961_utt01_source.wav"></audio> | <audio controls><source src="samples/libri/2961_utt01_hybrid.wav"></audio> |
| 3570 | <audio controls><source src="samples/libri/3570_utt01_source.wav"></audio> | <audio controls><source src="samples/libri/3570_utt01_hybrid.wav"></audio> |

### VCC2020 — Studio English

| Speaker | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|
| SEF1 | <audio controls><source src="samples/vcc2020/SEF1_utt01_source.wav"></audio> | <audio controls><source src="samples/vcc2020/SEF1_utt01_hybrid.wav"></audio> |
| SEF2 | <audio controls><source src="samples/vcc2020/SEF2_utt01_source.wav"></audio> | <audio controls><source src="samples/vcc2020/SEF2_utt01_hybrid.wav"></audio> |

---

## Male → Female

### VCTK — British English

| Speaker | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|
| p258 (M) | <audio controls><source src="samples/vctk/p258_utt01_source.wav"></audio> | <audio controls><source src="samples/vctk/p258_utt01_hybrid.wav"></audio> |
| p258 (M) | <audio controls><source src="samples/vctk/p258_utt02_source.wav"></audio> | <audio controls><source src="samples/vctk/p258_utt02_hybrid.wav"></audio> |
| p258 (M) | <audio controls><source src="samples/vctk/p258_utt03_source.wav"></audio> | <audio controls><source src="samples/vctk/p258_utt03_hybrid.wav"></audio> |

### L2-ARTIC — Hindi L2

| Speaker | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|
| ASI (M) | <audio controls><source src="samples/l2artic/ASI_utt01_source.wav"></audio> | <audio controls><source src="samples/l2artic/ASI_utt01_hybrid.wav"></audio> |
| ASI (M) | <audio controls><source src="samples/l2artic/ASI_utt02_source.wav"></audio> | <audio controls><source src="samples/l2artic/ASI_utt02_hybrid.wav"></audio> |
| ASI (M) | <audio controls><source src="samples/l2artic/ASI_utt03_source.wav"></audio> | <audio controls><source src="samples/l2artic/ASI_utt03_hybrid.wav"></audio> |

### LibriTTS — English

| Speaker | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|
| 4507 | <audio controls><source src="samples/libri/4507_utt01_source.wav"></audio> | <audio controls><source src="samples/libri/4507_utt01_hybrid.wav"></audio> |
| 8230 | <audio controls><source src="samples/libri/8230_utt01_source.wav"></audio> | <audio controls><source src="samples/libri/8230_utt01_hybrid.wav"></audio> |
| SEM1 | <audio controls><source src="samples/vcc2020/SEM1_utt01_source.wav"></audio> | <audio controls><source src="samples/vcc2020/SEM1_utt01_hybrid.wav"></audio> |

### VCC2020 — Studio English

| Speaker | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|
| SEM1 | <audio controls><source src="samples/vcc2020/SEM1_utt01_source.wav"></audio> | <audio controls><source src="samples/vcc2020/SEM1_utt01_hybrid.wav"></audio> |
| SEM2 | <audio controls><source src="samples/vcc2020/SEM2_utt01_source.wav"></audio> | <audio controls><source src="samples/vcc2020/SEM2_utt01_hybrid.wav"></audio> |

---

## Citation

```bibtex
@inproceedings{speakershift2025,
  title     = {Embedding-Space Speaker Trait Conversion via Hybrid Attention Mapping},
  author    = {[Authors]},
  booktitle = {Proceedings of Interspeech 2025},
  year      = {2025},
  url       = {https://[username].github.io/speakershift}
}
```
