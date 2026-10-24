## High-Fidelity Underwater Image Enhancement using A Multi-Branch Fusion Framework

| Humphrey Oboso Menge
| Vishnukumar S.

Implementation of the paper: *[High-fidelity underwater image enhancement using a multi-branch fusion framework](https://www.sciencedirect.com/science/article/pii/S0143816626005865)*

### Introduction
In this paper, we propose a novel underwater image enhancement method that separately enhances the contrast, reduces noise, and dehazes underwater images and subsequently, leverages the strengths of multi-exposure fusion to generate a high-fidelity image.


### Dependencies
- Windows MATLAB Runtime R2025a (25.1)

### Usage

Download UIEB, LSUI, and EUVP datasets from the below links:
```
UIEB: https://li-chongyi.github.io/proj_benchmark.html
LSUI: https://lintaopeng.github.io/_pages/UIE%20Project%20Page.html
EUVP: https://www.kaggle.com/datasets/pamuduranasinghe/euvp-dataset
```

1. Download and install the Windows MATLAB Runtime R2025a (25.1) from:
```
https://www.mathworks.com/products/compiler/runtime.html
```

2. Download the program from the below link:
```
https://drive.google.com/file/d/1KPYkC3yBcPYYc6JLjzeUWUxT3VwVuGpO/view?usp=sharing
```

3. Run the program

Example:
```
./interim_matlab.exe --raw "./UIEB_Best" --output_folder "./UIEB_Output"
```

### Citation
If you find our work useful, please consider citing the paper.

```
@article{MENGE2027110182,
title = {High-fidelity underwater image enhancement using a multi-branch fusion framework},
journal = {Optics and Lasers in Engineering},
volume = {208},
pages = {110182},
year = {2027},
issn = {0143-8166},
doi = {https://doi.org/10.1016/j.optlaseng.2026.110182},
url = {https://www.sciencedirect.com/science/article/pii/S0143816626005865},
author = {Humphrey Oboso Menge and Vishnukumar S․},
keywords = {Underwater image enhancement (UIE), Multi-exposure fusion (MEF), Contrast enhancement, Transmission map estimation, Image dehazing, Saliency detection},
abstract = {Recently, increased aquatic activities have necessitated the acquisition of clear underwater images worldwide. Underwater image enhancement (UIE) is an image processing approach that restores the quality of degraded aquatic images. Wavelength attenuation, light absorption, and light scattering significantly diminish captured underwater image clarity. Past studies introduce artifacts and color distortion and may not remove noise, which greatly affects image quality and clarity. This work proposes an underwater image enhancement method that generates a high-quality image by performing Multi-Exposure Fusion (MEF) on four enhanced versions of the input image, which have different features. The method first generates a color-corrected image from a distorted input image through color correction. Secondly, the color-corrected image is converted into the HSV color format, and then CLAHE is applied separately on the S and V channels to produce two contrast-enhanced images. Meanwhile, the Non-Local Means Filter and Unsharp Masking denoise and sharpen the color-corrected image to output a denoised-sharpened image. Concurrently, ambient light and transmission map estimates derived from the color-corrected image are utilized in generating four dehazed and restored images, and the best dehazed and restored image is selected using the NIQE metric. Subsequently, the four variably-enhanced images are used to generate four refined weight maps. Afterwards, the four refined weight maps and corresponding images are collapsed to output a final enhanced underwater image. Extensive evaluation results demonstrate that the proposed work outperforms existing methods in qualitative and quantitative assessments across three datasets. Substantive ablation studies validate the efficacy of each method component. https://github.com/humstack/high-fidelity.}
}
```