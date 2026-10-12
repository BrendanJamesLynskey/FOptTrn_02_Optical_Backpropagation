# Fourier Optics for Training 02 — Optical Backpropagation and In-Situ Training

How optical hardware is itself trained, and what that teaches about putting optics in an LLM training loop: in-silico training of diffractive networks and the reality gap, in-situ backpropagation by the adjoint method, physics-aware training, direct feedback alignment on a photonic co-processor, forward-only methods, zero-mean against biased analogue error, the ADC precision BF16 and FP8 formats ask for, a comparison of the methods, and a live in-browser experiment that trains one distorted convolution three ways (in-silico, physics-aware, in-situ). The conclusion: for an LLM-scale transform engine these methods calibrate the engine's own parameters; they do not train the LLM.

Topics: Reality gap, Adjoint method, Physics-aware training, DFA, Forward-only, FP8 gradients.

**Live site:** https://brendanjameslynskey.github.io/FOptTrn_02_Optical_Backpropagation/

Part of the [Fourier Optics for Training series](https://github.com/BrendanJamesLynskey/LLM_Hub_Fourier_Optics_Training). Every number comes from [analysis/results.md](https://github.com/BrendanJamesLynskey/LLM_Hub_Fourier_Optics_Training/blob/main/analysis/results.md), written by [analysis/train_flop_share.py](https://github.com/BrendanJamesLynskey/LLM_Hub_Fourier_Optics_Training/blob/main/analysis/train_flop_share.py), from a cited paper, or from the slide's live computation; the experiment is an illustrative toy and labelled as such. Every concept used here is explained, with links, in the [series glossary](https://brendanjameslynskey.github.io/LLM_Hub_Fourier_Optics_Training/#glossary). Sister series: [Fourier Optics for Inference](https://github.com/BrendanJamesLynskey/LLM_Hub_Fourier_Optics_Inference), [Compute in Transit](https://github.com/BrendanJamesLynskey/LLM_Hub_Compute_in_Transit), [FHE Accelerator Simulators](https://github.com/BrendanJamesLynskey/FHE_Hub_Accelerator_Simulators).

Licence: CC BY 4.0.
