# Benchmarking GEMM, Winograd, and FFT Convolution Algorithms

## About

This repository contains the source code, experimental notebook, results, and research paper for our study on the performance of **GEMM, Winograd, and FFT-based convolution algorithms using NVIDIA cuDNN**.

The experiments were performed on a GPU-based environment to compare the behavior of different convolution implementations under various configurations.

The detailed methodology, experimental results, analysis, and conclusions are presented in the research paper included in this repository.

---

## Repository Contents

```text
.
├── Code.ipynb    # Google Colab/Jupyter notebook
├── Paper.pdf                     # Research paper
└── README.md                      # Project documentation
```

## Hardware Requirements

The experiments were conducted using:

* NVIDIA GPU with CUDA support
* NVIDIA Tesla T4 GPU used for the original experiments
* Sufficient GPU memory for the selected convolution configurations

The notebook can be run on **Google Colab** by selecting a GPU runtime.

---

## Software Requirements

The original experiments used:

* Python 3.x
* PyTorch 2.11.0
* CUDA 12.8
* cuDNN 9.1.9
* NumPy
* Matplotlib
* Pandas

The exact environment information is also available in the notebook.

---

## Running the Notebook

### Option 1: Google Colab

1. Open the `.ipynb` notebook from this repository.

2. Open it using Google Colab.

3. Select:

   **Runtime → Change runtime type → GPU**

4. Verify that a GPU is available.

5. Run the notebook cells sequentially.

The notebook performs the convolution benchmarks and generates the measurements and visualizations used in the analysis.

### Option 2: Local Environment

Clone the repository:

```bash
git clone https://github.com/<your-username>/<your-repository>.git
```

Move into the repository:

```bash
cd <your-repository>
```

Install the required Python packages:

```bash
pip install torch torchvision numpy pandas matplotlib
```

Open the notebook:

```bash
jupyter notebook
```

Then run:

```text
convolution_benchmark.ipynb
```

> For GPU-based experiments, the local system must have a compatible NVIDIA GPU, CUDA, and cuDNN installation.

---

## Experimental Configuration

The benchmark configuration used in the original experiments is defined inside the notebook.

The main parameters include:

* Input channels
* Output channels
* Input spatial dimensions
* Batch size
* Convolution kernel size
* Data type
* GPU device

To reproduce the reported results as closely as possible, use the same hardware and software environment described in the paper.

---

## Output

Running the notebook produces benchmark results and visualizations for:

* Execution time
* GPU memory usage
* Numerical stability

These results can be used to reproduce the figures and tables presented in the research paper.

---

## Research Paper

The complete research paper containing the methodology, detailed experimental setup, results, discussion, and conclusion is available in:

```text
Paper.pdf
```

---

## Authors

**Prabin Karki**

[Add other authors here]

## License

This project is intended for **academic and research purposes**.
