# 🌟 A Curated List of Awesome Virtual Try-Off (VTOFF) Research 🌟

Virtual Try-Off (VTOFF) is a novel computer vision task that extracts standardized, canonical images of garments from single photos of clothed individuals, moving beyond traditional virtual try-on techniques by focusing on precise garment reconstruction rather than model dressing. The task was introduced and the term coined in [TryOffDiff: Virtual-Try-Off via High-Fidelity Garment Reconstruction using Diffusion Models](https://rizavelioglu.github.io/tryoffdiff).


### Demos
- [[🤗 Space]](https://huggingface.co/spaces/rizavelioglu/tryoffdiff) finetuned Stable Diffusion-v1.4 for VTOFF and introduced `TryOffDiff`.
- [[🤗 Space]](https://huggingface.co/spaces/ginipick/FitGen) uses `FLUX.1-dev` and the LoRA `"prithivMLmods/Canopus-Clothing-Flux-LoRA"` to generate clothes from text.
- [[🤗 Space]](https://huggingface.co/spaces/xiaozaa/cat-try-off-flux) trained a new model "cat-try-off-flux" based on `FLUX.1-dev` and `CatVTON`.
- [[🤗 Space]](https://huggingface.co/spaces/multimodalart/flux-style-shaping) uses `FLUX.1-dev-Redux` + `FLUX.1-dev-Depth`. Set mask as 'structure' and model image as 'style' for targeting VTOFF.


### Datasets
- 2021, [VITON-HD](https://paperswithcode.com/dataset/viton-hd)
- 2022, [Dress Code](https://paperswithcode.com/dataset/dress-code)
- 2024, [IGPair](https://huggingface.co/datasets/IMAGDressing/IGPair)
- 2025, [LAION-Garment](https://huggingface.co/datasets/loooooong/LAION-Garment)


### Papers
<sup>[2020-05-08]</sup> 
***TileGAN: category-oriented attention-based high-quality tiled clothes generation from dressed person***\
<sup>
  [[paper]](https://yuan-gao.net/pdf/NCA2020%20-%20TileGAN.pdf) 
  targeted vtoff task with a two-stage method.
</sup>

<sup>[2021-08-08]</sup> 
***ViTon-GUN: Person-to-Person Virtual Try-on via Garment Unwrapping***\
<sup>
  [[paper]](https://ieeexplore.ieee.org/abstract/document/10944549) 
  targeted p2p-vton task: run vtoff first, then vton.
</sup>

<sup>[2022-08-11]</sup> 
***ARMANI: Part-level Garment-Text Alignment for Unified Cross-Modal Fashion Design***\
<sup>
  [[paper]](https://arxiv.org/abs/2208.05621) 
  text-to-garment generation.
</sup>

<sup>[2023-08-15]</sup> 
***SGDiff: A Style Guided Diffusion Model for Fashion Synthesis***\
<sup>
  [[paper]](https://arxiv.org/abs/2308.07605)
  finetuned GLIDE to generate garment images from "text" (garment attributes) + "style image".
</sup>

<sup>[2023-08-22]</sup> 
***DiffCloth: Diffusion Based Garment Synthesis and Manipulation via Structural Cross-modal Semantic Alignment***\
<sup>
  [[paper]](https://arxiv.org/abs/2308.11206) 
  finetuned StableDiffusion for targeting garment synthesis and manipulation.
</sup>

<sup>[2024-01-29]</sup> 
***DressCode: Autoregressively Sewing and Generating Garments from Text Guidance***\
<sup>
  [[paper]](https://arxiv.org/abs/2401.16465)
  [[project]](https://ihe-kaii.github.io/DressCode/)
  [[code]](https://github.com/IHe-KaiI/DressCode)
  text-to-3dGarment with 2 branches: text-to-sewing-patterns with SewingGPT (3d garment) and text-to-texture with finetuned StableDiffusion.
</sup>

<sup>[2024-04-22]</sup>
***FLDM-VTON: Faithful Latent Diffusion Model for Virtual Try-on***\
<sup>
  [[paper]](https://arxiv.org/abs/2404.14162) 
  [[code]](https://github.com/xiangji-ai/fldm-vton) 
  vtoff task is included in the loss function for training a vton model, vtoff was not the focus of the paper, nor was a stand-alone task introduced.
</sup>

<sup>[2024-04-26]</sup>
***FashionSD-X: Multimodal Fashion Garment Synthesis using Latent Diffusion***\
<sup>
  [[paper]](https://arxiv.org/abs/2404.18591v1)
  finetuned SD-v1.5 with ControlNet to generate garments from text + sketch image.
</sup>

<sup>[2024-11-25]</sup>
***Controllable Human Image Generation with Personalized Multi-Garments***\
<sup>
  [[paper]](https://arxiv.org/abs/2411.16801)
  [[project]](https://omnious.github.io/BootComp/)
  [[code]](https://github.com/omnious/BootComp)
  generated garment images from segmented garments—extracted from reference images—to construct a dataset for training a multi-garment VTON model.
</sup>

<sup>[2024-11-27]</sup>
***TryOffDiff: Virtual-Try-Off via High-Fidelity Garment Reconstruction using Diffusion Models***\
<sup>
  [[paper]](https://huggingface.co/papers/2411.18350)
  [[project]](https://rizavelioglu.github.io/tryoffdiff)
  [[code]](https://github.com/rizavelioglu/tryoffdiff/)
  coined the term Virtual Try-Off (VTOFF), formally introduced the task and introduced the baselines.
</sup>

<sup>[2024-11-29]</sup>
***RAGDiffusion: Faithful Cloth Generation via External Knowledge Assimilation***\
<sup>
  [[paper]](https://arxiv.org/abs/2411.19528)
</sup>

<sup>[2024-12-11]</sup>
***TryOffAnyone: Tiled Cloth Generation from a Dressed Person***\
<sup>
  [[paper]](https://arxiv.org/abs/2412.08573)
  [[code]](https://github.com/ixarchakos/try-off-anyone)
  finetuned Stable Diffusion-v1.5-inpainting for vtoff in CatVTON-style.
</sup>

<sup>[2024-12-16]</sup>
***IGR: Improving Diffusion Model for Garment Restoration from Person Image***\
<sup>
  [[paper]](https://arxiv.org/abs/2412.11513)
  finetuned Stable Diffusion-v1.5 for vtoff using 2 UNets (Reference and Denoiser).
</sup>

<sup>[2025-01-08]</sup>
***Enhancing Virtual Try-On with Synthetic Pairs and Error-Aware Noise Scheduling***\
<sup>
  [[paper]](https://arxiv.org/abs/2501.04666)
  used VTOFF to generate synthetic pairs to enrich VTON training dataset. Trained a U-Net model for warping latent features.
</sup>

<sup>[2025-01-27]</sup>
***Any2AnyTryon: Leveraging Adaptive Position Embeddings for Versatile Virtual Clothing Tasks***\
<sup>
  [[paper]](https://arxiv.org/abs/2501.15891)
  [[project]](https://logn-2024.github.io/Any2anyTryonProjectPage/)
  [[code]](https://github.com/logn-2024/Any2anyTryon)
  1st unified model targeting both VTON and VTOFF. 
</sup>

<sup>[2025-03-07]</sup>
***DiffDesign: A diffusion model using garment Knowledge-Enhanced for Fashion Design Synthesis***\
<sup>
  [[paper]](https://ieeexplore.ieee.org/document/10889966)
  trained a WURSTCHEN-based model for text-to-garment task.
</sup>

<sup>[2025-04-17]</sup>
***MGT: Extending Virtual Try-Off to Multi-Garment Scenarios***\
<sup>
  [[paper]](https://arxiv.org/abs/2504.13078)
  [[project]](https://rizavelioglu.github.io/tryoffdiff)
  [[code]](https://github.com/rizavelioglu/tryoffdiff/)
  1st VTOFF model supporting multiple garment reconstruction. Finetuned StableDiffusion-v1.4 (similar to TryOffDiff) and trained a class embedding for multi-garment support.
</sup>

<sup>[2025-04-17]</sup>
***IMAGGarment-1: Fine-Grained Garment Generation for Controllable Fashion Design***\
<sup>
  [[paper]](https://arxiv.org/abs/2504.13176)
  [[project]](https://revive234.github.io/imaggarment.github.io/)
  [[code]](https://github.com/muzishen/IMAGGarment-1)
garment synthesis with precise control over silhouette, color, and logo placement (3 inputs). Incorporates a tower architecure with SD-1.5 for coarse generation followed by a fine-grained approach utilizing SD-1.5-inpaint.
</sup>

<sup>[2025-05-26]</sup>
***ImgEdit: A Unified Image Editing Dataset and Benchmark***\
<sup>
  [[paper]](https://arxiv.org/abs/2505.20275)
  [[code]](https://github.com/PKU-YuanGroup/ImgEdit)
  trained an image editing model using Vision-Language Model to process a reference image and editing prompt, targeting multiple tasks including VTOFF.
</sup>

<sup>[2025-05-27]</sup>
***Inverse Virtual Try-On: Generating Multi-Category Product-Style Images from Clothed Individuals***\
<sup>
  [[paper]](https://arxiv.org/abs/2505.21062)
  [[project]](https://temu-vtoff-page.github.io/)
  [[code]](https://github.com/davidelobba/TEMU-VTOFF)
  1st dual-DiT model for VTOFF with multi-garment support, built on a finetuned StableDiffusion-v3 with modified attention. It accepts images, text, or masks as input, enabling multi-category garment handling.
</sup>

<sup>[2025-08-06]</sup>
***Two-Way Garment Transfer: Unified Diffusion Framework for Dressing and Undressing Synthesis***\
<sup>
  [[paper]](https://arxiv.org/abs/2508.04551)
  unified framework (TWGTM) targeting both VTON & VTOFF.
</sup>

<sup>[2025-08-06]</sup>
***One Model For All: Partial Diffusion for Unified Try-On and Try-Off in Any Pose***\
<sup>
  [[paper]](https://arxiv.org/abs/2508.04559)
  [[project]](https://onemodelforall.github.io/)
  unified framework (OMFA) targeting both VTON & VTOFF.
</sup>

<sup>[2025-08-06]</sup>
***Voost: A Unified and Scalable Diffusion Transformer for Bidirectional Virtual Try-On and Try-Off***\
<sup>
  [[paper]](https://arxiv.org/abs/2508.04825)
  [[project]](https://nxnai.github.io/Voost/)
  unified framework (Voost) targeting both VTON & VTOFF.
</sup>
