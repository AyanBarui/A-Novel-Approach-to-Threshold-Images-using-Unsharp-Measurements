# **A Novel Approach to Threshold Images using Unsharp Measurements**

### December 8th, 2023

**Main author:** [Ayan Barui](https://www.linkedin.com/in/ayan-barui-4540b7247/)

**Co-authors:** [Mayukha Pal](https://scholar.google.co.in/citations?user=2VW0NvcAAAAJ&hl=en), [Prasanta K. Panigrahi](https://scholar.google.co.in/citations?user=sNq6fwwAAAAJ&hl=en)

The project [report](https://github.com/SoumikSamanta10/Simulation-QKD-protocols/tree/main/results) in the folder `Report'.

## **Project Description:**

We propose a hybrid quantum approach to threshold and binarize a grayscale image through unsharp measurements (UM) relying on image histogram. Generally, the histograms are characterized by multiple overlapping normal distributions corresponding to objects, or image features with small but significant overlaps, making it challenging to establish suitable thresholds. The proposed methodology uses peaks of the overlapping Gaussians and the distance between neighboring local minima as the variance, based on which the UM parameters are chosen, that maps the normal distribution into a localized delta function.
To demonstrate its efficacy, subsequent implementation is done on noisy quantum environments in Qiskit. This process is iteratively repeated for a multimodal histogram to obtain more thresholds, which are then applied to various life-like pictures to get high-contrast images, resulting in comparable peak signal-to-noise
ratio and structural similarity index measure values. The obtained thresholds are used to binarize a grayscale image by using novel enhanced quantum image representation integrated with a threshold encoder and an efficient quantum comparator (QC) that depicts the whole binarized picture. This approach significantly reduces the complexity of the proposed QC and of the whole algorithm when compared to earlier models.


## **Paper Link:**

[1] Ayan Barui, Mayukha Pal, Prasanta K. Panigrahi, [“A Novel Approach to Threshold Images using Unsharp Measurements”](https://scholar.google.co.in/citations?view_op=view_citation&hl=en&user=sNq6fwwAAAAJ&sortby=pubdate&citation_for_view=sNq6fwwAAAAJ:xpOcSxJuMv8C) arXiv preprint, arXiv:2310.10753 (2023)
