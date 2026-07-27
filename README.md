# SUSAN
# Mapping Land Cover in Circumpolar Cities Across Seasons and Continents: A Sub-Meter 1.5-Modality Benchmark with Relative Depth

Yongqi Sun, Anzhu Yu, Chenguang Dai, Yu Su, Meilin Li, Yujun Quan, Yinhe Liu and Yanfei Zhong

Information Engineering University, Zhengzhou, 450001, China

Wuhan University, Wuhan 430079

_Submitted to IEEE Transcations on Geoscience and Remote Sensing_

---

## Abstract

Accurate land cover information for circumpolar cities is essential for urban planning, infrastructure management, and climate adaptation, yet existing circumpolar products lack the spatial resolution and thematic detail required for city-scale mapping under strong seasonal and illumination changes. We present SUSAN, to our knowledge the first cross-season and cross-continent sub-meter land cover dataset designed for circumpolar urban environments. SUSAN contains 3685 optical image patches from 31 cities across Europe and North America at 0.5--0.75 m resolution, with aligned relative depth (rDepth) maps and annotations for 8 coarse-grained and 11 fine-grained categories. The rDepth maps are derived from the optical images and evaluated as a supplementary structural representation using a reference 1.5-modality learning architecture, without additional sensor acquisition. Across three matched model pairs and four cross-continent evaluation settings, incorporating rDepth improves mF$_1$ in most cases, with an average gain of 1.83 percentage points and a maximum gain of 7.15 percentage points in fine-grained transfer. The gains are concentrated in buildings, airport roads, and ice, whereas snow shows marginal or negative changes and pooled road accuracy is nearly unchanged. Domain-generalization models with rDepth also remain competitive with unsupervised domain-adaptation methods that use unlabeled target images. Case studies in city-scale mapping, road extraction, cultivated land analysis, and ice-snow discrimination further illustrate the scope of the dataset. SUSAN provides a multi-grained resource and reproducible benchmark for all-season urban land cover mapping at high latitudes.

---

## Highlights

- First cross-season and cross-continent sub-meter urban land cover dataset
- 8 coarse and 11 fine land cover categories for multi-grained analysis
- Co-registered relative depth provided without additional data acquisition
- Benchmark gains concentrate in buildings, airport roads and ice
- Case studies: roads, cultivated land and ice-snow mapping in circumpolar cities

---

## SUSAN Dataset and Code

This repository provides:

- **SUSAN**: a high-resolution, multi-season land cover dataset for 31 circumpolar cities (17 in Europe, 14 in North America), including:
  - JL-1 optical imagery at 0.5--0.75 m
  - Relative depth (rDepth) maps derived from a vision foundation model
  - Multi-grained labels with 8 coarse-grained and 11 fine-grained land cover categories
- Reference implementations of the 1.5-modality learning framework for RGB--rDepth semantic segmentation under domain generalization (DG) and unsupervised domain adaptation (UDA) settings.

**A subset of the code and data will be released after the paper is accepted.** Please see the code and `docs/` (if provided) for details on data format, training scripts, and evaluation protocols.

---

## Keywords

Land cover mapping; Circumpolar cities; Benchmark dataset; High-resolution imagery; Multi-season mapping; Relative depth

---

## Citation

If you find SUSAN or the 1.5-modality framework useful in your research, please cite:

Sun, Y., Yu, A., Dai, C., Su, Y., Li, M., Quan, Y., Liu Y. and Zhong Y. 2026. Mapping land cover in circumpolar cities across seasons and continents: A sub-meter 1.5-modality benchmark with relative depth. _IEEE Transcations on Geoscience and Remote Sensing_, under review.

You can also use the following BibTeX entry:

```bibtex
@article{susan_1p5modality_TGRS2026,
  title   = {Mapping Land Cover in Circumpolar Cities Across Seasons and Continents: A Sub-Meter 1.5-Modality Benchmark with Relative Depth},
  author  = {Yongqi Sun, Anzhu Yu, Chenguang Dai, Yu Su, Meilin Li, Yujun Quan, Yinhe Liu and Yanfei Zhong},
  journal = {IEEE Transcations on Geoscience and Remote Sensing},
  year    = {2026},
  note    = {under review}
}
```

---

## Contact

For questions about the dataset or code, please contact:

- Yongqi Sun: `sunyq2002@163.com`  
- Anzhu Yu (corresponding author): `anzhu_yu@126.com`
