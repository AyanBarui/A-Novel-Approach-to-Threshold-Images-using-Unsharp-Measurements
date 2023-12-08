# **A Novel Approach to Threshold Images using Unsharp Measurements**

### January 23rd, 2021

**Main author:** [Ayan Barui](https://www.linkedin.com/in/ayan-barui-4540b7247/)

**Co-authors:** [Mayukha Pal](https://scholar.google.co.in/citations?user=2VW0NvcAAAAJ&hl=en), [Prasanta K. Panigrahi](https://scholar.google.co.in/citations?user=sNq6fwwAAAAJ&hl=en)

The project [report](https://github.com/SoumikSamanta10/Simulation-QKD-protocols/tree/main/results) in the folder `Report'.

## **Project Description:**

We propose a hybrid quantum approach to threshold and binarize a grayscale image through unsharp measurements (UM), which depends only on the image’s histogram, maintaining secrecy among parties. An image histogram is generally characterized by multiple overlapping normal distributions, which are centered around objects or image features with small but significant overlaps, making it difficult to establish suitable thresholds. The proposed method is based on an overcomplete basis that separates important image features by mapping normal distribution into the Dirac delta function, thereby converting Mahalanobis distance into regular Euclidean distance. This process is iteratively repeated to get more thresholds, which are applied to get high-contrast images, resulting in comparable peak signal-to-noise ratio and structural similarity index measure values. The same is implemented in the space of qubits and experimentally demonstrated in Qiskit using the AerSimulator. The obtained thresholds are used to binarize a grayscale image by using novel enhanced quantum image representation integrated with a threshold encoder and an efficient quantum comparator (QC). The output result depicts the whole binarized picture with just one measured state representing the binary intensity value with its corresponding position pixel. This approach significantly reduces the complexity of the proposed QC when compared to earlier models. 

## **Key Results:**
1) Demonstrated a semi-automatic hybrid quantum thresholding scheme relying on unsharp measurement to give an overcomplete basis.
2) Extracted feature separation realized by Mahalanobis distance into Euclidean distance based on the conversion of normal distributions into the Dirac delta function.
3) This process is iteratively repeated to get more thresholds, which are applied to get high-contrast images, result-ing in comparable PSNR and SSIM values and implemented in the space of qubits.
4) Obtained thresholds are used to binarize a grayscale image by using novel enhanced quantum image represent-tation (NEQR) integrated with a threshold encoder and an efficient quantum comparator. 
5) Reduced the complexity of the proposed QC when compared to its earlier models. 

## **Code Repo Descriptions:**
1) Folder overlap_vs_HS_cost has code for the comparision between the optimization of the Hilbert-Schmidt cost function and the optimization of the overlap. These codes are used in the analysis presented in Sec. (III) of the report.
2) Folder random_embedding_circuits has code for the random variational embedding circuits that we have presented in Sec. (IV) of the report. These codes are used to generate the plots shown in Fig. (3) and Fig. (4) of the report.
3) Folder risk_function/2d_data has code for the analysis of the risk function presented in Sec. (II) of the report. There is also a code for generating a data set shown in Fig. (1) of the report. 
4) Folder Fourier_analysis/1d-QAOA-Fourier has code for performing a Pauli decomposition of the output of a single-wire embedded circuit. See, for e.g., Eqs. (2.3) and (2.4) of the report. 
5) Folder Simulation_of_Variational_Circuits has code for implementing and comparing different variational circuit structures, varying in types of gates, circuit depth, number of qubits, as an embedding circuit for data classification problem.

## Environment Setup before running the code:

1. Clone the repository.
```git clone https://github.com/SoumikSamanta10/Simulation-QKD-protocols.git```

2. Open the terminal and navigate to the directory.
```cd Simulation-QKD-protocols```

3. Install virtual environment package.
```pip install virtualenv```

4. make a virtual environment.
```virtualenv venv```

5. Activate the virtual environment.
Windows: ```./venv/Scripts/activate```
Linux: ```source venv/bin/activate```

6. Install the dependencies.
```pip install -r requirements.txt```

7. Run the codes as you want.

## **Paper Link:**

[1] Ayan Barui, Mayukha Pal, Prasanta K. Panigrahi, [“A Novel Approach to Threshold Images using Unsharp Measurements”](https://scholar.google.co.in/citations?view_op=view_citation&hl=en&user=sNq6fwwAAAAJ&sortby=pubdate&citation_for_view=sNq6fwwAAAAJ:xpOcSxJuMv8C) arXiv preprint, arXiv:2310.10753 (2023)
