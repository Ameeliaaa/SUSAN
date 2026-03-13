# SUSAN
# Bridging Seasons and Continents for Land Cover Mapping of Circumpolar Cities: A High-resolution Dataset with 1.5-modality Learning

Yongqi Sun, Anzhu Yu, Chenguang Dai, Yu Su, Meilin Li, Yujun Quan, Yinhe Liu, Yanfei Zhong  

_Submitted to Remote Sensing of Environment_

---

## Abstract

Accurate land cover information is fundamental to urban planning and environmental monitoring. The circumpolar region poses two challenges for land cover mapping: seasonal variations altering spectral appearance between winter and other seasons, and continental differences in urban morphology between European and North American cities. Existing circumpolar studies rely on medium-to-coarse resolution imagery lacking high-resolution annotations for Arctic cities. To bridge these gaps, we present SUSAN (Spaceborne circUmpolar urban SemAntic segmeNtation), a high-resolution dataset derived from JL-1 satellite imagery at 0.5 m and 0.75 m resolutions, covering 17 European and 14 North American cities across all seasons. SUSAN provides 8 coarse-grained and 11 fine-grained land cover categories with annotations, and includes relative depth maps derived from optical imagery as domain-invariant representations. We further propose a 1.5-modality learning paradigm that treats relative depth as a 0.5-modality representation to introduce depth continuity and relief as prior information. Experiments on cross-continent validation, cross-season analysis, and city-scale mapping demonstrate SUSAN's validity and the 1.5-modality effectiveness. The 1.5-modality paradigm improves segmentation accuracy in winter and other seasons compared to single-modality baselines, with gains in season-sensitive categories whose optical signatures are disrupted by snow. In cross-continent validation, our method improves accuracy over single-modality baselines and achieves results comparable to existing unsupervised domain adaptation methods. These results establish SUSAN as a benchmark for circumpolar urban land cover research and the 1.5-modality framework as a broadly applicable methodology for cross-domain semantic segmentation, directly improving the reliability of high-resolution land cover maps under cross-season and cross-continent shifts.

---

## SUSAN Dataset and Code

This repository provides:

- SUSAN: a high-resolution, multi-season land cover dataset for 31 circumpolar cities (17 in Europe, 14 in North America), including:
  - JL-1 optical imagery at 0.5–0.75 m
  - Relative depth (rDepth) maps derived from a vision foundation model
  - Multi-grained labels with 8 coarse-grained and 11 fine-grained land cover categories
- Reference implementations of the 1.5-modality learning framework for RGB–rDepth semantic segmentation under domain generalization (DG) and unsupervised domain adaptation (UDA) settings.

**A subset of the code and data will be released after the paper is accepted.** Please see the code and `docs/` (if provided) for details on data format, training scripts, and evaluation protocols.

---

## Citation

If you find SUSAN or the 1.5-modality framework useful in your research, please cite:

Sun, Y., Yu, A., Dai, C., Su, Y., Li, M., Quan, Y., Liu, Y., Zhong, Y., 2026. Bridging seasons and continents for land cover mapping of circumpolar cities: A high-resolution dataset with 1.5-modality learning. _Remote Sensing of Environment_, under review.

You can also use the following BibTeX entry:

```bibtex
@article{susan_1p5modality_rse2026,
  title   = {Bridging Seasons and Continents for Land Cover Mapping of Circumpolar Cities: A High-resolution Dataset with 1.5-modality Learning},
  author  = {Sun, Yongqi and Yu, Anzhu and Dai, Chenguang and Su, Yu and Li, Meilin and Quan, Yujun and Liu, Yinhe and Zhong, Yanfei},
  journal = {Remote Sensing of Environment},
  year    = {2026},
  note    = {under review}
}
```

---

## Contact

For questions about the dataset or code, please contact:

- Yongqi Sun: `sunyq2002@163.com`  
- Anzhu Yu (corresponding author): `anzhu_yu@126.com`

