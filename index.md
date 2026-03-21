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
</style>

**Interspeech 2025** · [Paper](#) · [Code](#) · [Citation](#citation)

---

We propose **HybridAttentionMapper**, a 21.7M-parameter neural network that re-maps speaker identity embeddings across a static trait boundary (gender) while preserving linguistic content. Below we compare the **ground truth (source)** against our **Hybrid system** across two conversion directions and multiple corpora.

---

## Female → Male

<!-- ### VCTK — British English

| Speaker | Utterance | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|---|
| p268 (F) | 020 | <audio controls><source src="samples/VCTK/p268_020_mic2.flac" type="audio/flac"></audio> | <audio controls><source src="samples/VCTK/p268_020_slt.wav" type="audio/wav"></audio> |
| p268 (F) | 027 | <audio controls><source src="samples/VCTK/p268_027_mic1.flac" type="audio/flac"></audio> | <audio controls><source src="samples/VCTK/p268_027_slt.wav" type="audio/wav"></audio> | -->

### L2-ARTIC — Hindi L2

| Speaker | Utterance | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|---|
| SVBI (F) | arctic-a0120 | <audio controls><source src="samples/l2artic/SVBI_arctic-a0120_source.wav" type="audio/wav"></audio> | <audio controls><source src="samples/l2artic/SVBI_a0120_slt.wav" type="audio/wav"></audio> |
| SVBI (F) | arctic-a0130 | <audio controls><source src="samples/l2artic/SVBI_arctic-a0130_source.wav" type="audio/wav"></audio> | <audio controls><source src="samples/l2artic/SVBI_a0130_slt.wav" type="audio/wav"></audio> |

### LibriTTS — English

| Speaker | Utterance | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|---|
| 3570 (F) | 5695-000000 | <audio controls><source src="samples/libri/3570_5695_000000_000000_source.wav" type="audio/wav"></audio> | <audio controls><source src="samples/libri/3570_5695_000000_000000_slt.wav" type="audio/wav"></audio> |
| 3570 (F) | 5695-000001 | <audio controls><source src="samples/libri/3570_5695_000001_000003_source.wav" type="audio/wav"></audio> | <audio controls><source src="samples/libri/3570_5695_000001_000003_slt.wav" type="audio/wav"></audio> |

### VCC2020 — Studio English

| Speaker | Utterance | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|---|
| SEF2 (F) | E30012 | <audio controls><source src="samples/vcc2020/sef2_E30012_source.wav" type="audio/wav"></audio> | <audio controls><source src="samples/vcc2020/SEF2_E30012_slt.wav" type="audio/wav"></audio> |
| SEF2 (F) | E30019 | <audio controls><source src="samples/vcc2020/sef2_E30019_source.wav" type="audio/wav"></audio> | <audio controls><source src="samples/vcc2020/SEF2_E30019_slt.wav" type="audio/wav"></audio> |

---

## Male → Female

### VCTK — British English

| Speaker | Utterance | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|---|
| p258 (M) | 008 | <audio controls><source src="samples/VCTK/p258_008_mic2.flac" type="audio/flac"></audio> | <audio controls><source src="samples/VCTK/p258_008_slt.wav" type="audio/wav"></audio> |
| p258 (M) | 019 | <audio controls><source src="samples/VCTK/p258_019_mic2.flac" type="audio/flac"></audio> | <audio controls><source src="samples/VCTK/p258_019_slt.wav" type="audio/wav"></audio> |

### L2-ARTIC — Hindi L2

| Speaker | Utterance | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|---|
| ASI (M) | arctic-a0009 | <audio controls><source src="samples/l2artic/ASI_arctic-a0009_source.wav" type="audio/wav"></audio> | <audio controls><source src="samples/l2artic/ASI_a0009_slt.wav" type="audio/wav"></audio> |
| ASI (M) | arctic-a0017 | <audio controls><source src="samples/l2artic/ASI_arctic-a0017_source.wav" type="audio/wav"></audio> | <audio controls><source src="samples/l2artic/ASI_a0017_slt.wav" type="audio/wav"></audio> |

### VCC2020 — Studio English

| Speaker | Utterance | Source (Ground Truth) | Hybrid (Ours) |
|---|---|---|---|
| SEM1 (M) | E30006 | <audio controls><source src="samples/vcc2020/sem1_E30006_source.wav" type="audio/wav"></audio> | <audio controls><source src="samples/vcc2020/SEM1_E30006_slt.wav" type="audio/wav"></audio> |
| SEM1 (M) | E30016 | <audio controls><source src="samples/vcc2020/sem1_E30016_source.wav" type="audio/wav"></audio> | <audio controls><source src="samples/vcc2020/SEM1_E30016_slt.wav" type="audio/wav"></audio> |

---

## Citation

\`\`\`bibtex
@inproceedings{speakershift2025,
  title     = {Embedding-Space Speaker Trait Conversion via Hybrid Attention Mapping},
  author    = {[Authors]},
  booktitle = {Proceedings of Interspeech 2025},
  year      = {2025},
  url       = {https://[username].github.io/speakershift}
}
\`\`\`