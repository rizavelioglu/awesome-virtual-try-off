# 🌟 A Curated List of Awesome Virtual Try-Off (VTOFF) Research 🌟

Virtual Try-Off (VTOFF) is a novel computer vision task that extracts standardized, canonical garment images from single photos of clothed individuals, moving beyond traditional virtual try-on techniques by focusing on precise garment reconstruction rather than model dressing. The task was introduced in [TryOffDiff: Virtual-Try-Off via High-Fidelity Garment Reconstruction using Diffusion Models](https://rizavelioglu.github.io/tryoffdiff).

### Papers
May'20, **_TileGAN: category-oriented attention-based high-quality tiled clothes generation from dressed person_**\
<sub>
  [[paper]](https://yuan-gao.net/pdf/NCA2020%20-%20TileGAN.pdf) 
  targeted vtoff task with a two-stage method.
</sub>

Apr'24, **_FLDM-VTON: Faithful Latent Diffusion Model for Virtual Try-on_**\
<sub>
  [[paper]](https://arxiv.org/abs/2404.14162) 
  [[code]](https://github.com/xiangji-ai/fldm-vton) 
  vtoff task is included in the loss function for training a vton model, vtoff was not the focus of the paper, nor was a stand-alone task introduced.
</sub>

Nov'24, **_TryOffDiff: Virtual-Try-Off via High-Fidelity Garment Reconstruction using Diffusion Models_**\
<sub>
  [[paper]](https://huggingface.co/papers/2411.18350)
  [[project]](https://rizavelioglu.github.io/tryoffdiff)
  [[code]](https://github.com/rizavelioglu/tryoffdiff/)
  coined the term Virtual Try-Off (VTOFF), formally introduced the task and introduced the baselines.
</sub>

Nov'24, **_RAGDiffusion: Faithful Cloth Generation via External Knowledge Assimilation_**\
<sub>
  [[paper]](https://arxiv.org/abs/2411.19528)
</sub>

Dec'24, **_TryOffAnyone: Tiled Cloth Generation from a Dressed Person_**\
<sub>
  [[paper]](https://arxiv.org/abs/2412.08573)
  [[code]](https://github.com/ixarchakos/try-off-anyone)
</sub>

### Datasets
- 2021, [VITON-HD](https://paperswithcode.com/dataset/viton-hd)
- 2022, [DressCode](https://paperswithcode.com/dataset/dress-code)

### Demos
- [[🤗 Space]](https://huggingface.co/spaces/rizavelioglu/tryoffdiff) finetuned Stable Diffusion-v1.4 for VTOFF and introduced `TryOffDiff`.
- [[🤗 Space]](https://huggingface.co/spaces/ginipick/FitGen) uses `FLUX.1-dev` and the LoRA `"prithivMLmods/Canopus-Clothing-Flux-LoRA"` to generate clothes from text.
- [[🤗 Space]](https://huggingface.co/spaces/xiaozaa/cat-try-off-flux) trained a new model "cat-try-off-flux" based on `FLUX.1-dev` and `CatVTON`.
