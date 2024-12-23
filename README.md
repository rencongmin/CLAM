# CLASI: Combined Learning for Augmented Super-Resolution Imaging

CLAM is a two-stage deep learning framework designed to reconstruct high-resolution super-resolution (SR) images from low signal-to-noise ratio (SNR), diffraction-limited wide-field (WF) microscopy images. CLAM integrates the high-fidelity restoration capabilities of supervised deep learning (SDL) models with the ultra-fine structure generation strengths of generative deep learning (GDL) models, which provides robust and high-fidelity SR reconstructions, enabling researchers to visualize intricate subcellular structures and dynamic interactions.

## **Characrization of CLAM**

- High-fidelity SR reconstruction under low SNR conditions.

![Fig1.png](figs/Fig1.png)

- Supports various microscopy modalities and subcellular structures.

![fig5.tif](https://prod-files-secure.s3.us-west-2.amazonaws.com/349f2e03-5eed-45b5-85a1-60407647e51f/5b53de70-f71c-4b81-988e-b17f77e28101/fig5.tif)

- CLAM enables researchers to observe interactions between organelles with high resolution and high signal-to-noise ratio.

![ER+Mito.tif](https://prod-files-secure.s3.us-west-2.amazonaws.com/349f2e03-5eed-45b5-85a1-60407647e51f/a8bdb97b-e113-4719-bb75-bfd6fb635e43/ERMito.tif)

![MT+Lyso.tif](https://prod-files-secure.s3.us-west-2.amazonaws.com/349f2e03-5eed-45b5-85a1-60407647e51f/53bb95fb-a4fe-4869-a988-429f61dda18a/MTLyso.tif)

## Installation

### Prerequisites

- Python ==3.10.13
- torch==1.13.1+cu116

### Installation Steps

1. Clone the CLAM repository from GitHub.
    
    ```bash
    git clone <https://github.com/your-repo/CLAM.git>
    cd CLAM
    ```
    
2. Create a virtual environment and install PyTorch and other dependencies.
    
    ```bash
    conda create -n CLAM python=3.10.13
    conda activate CLAM
    ```
    
3. Install the required dependencies.
    
    ```bash
    pip install -r requirements.txt
    ```
    
4. Install the CLAM napari plugin.
    
    ```bash
    pip install CLAM.whl
    ```
    

## Usage

### Launching the Plugin

1. Open napari:
    
    ```bash
    napari
    ```
    
2. Load the CLAM plugin by navigating to the `Plugins` menu and selecting `CLAM`.

### Step-by-Step Guide

### Step 1: Load an Image

- Click the **"Select Image"** button to choose a WF microscopy image for processing.

### Step 2: Select Parameters

- Choose the subcellular structure type from the dropdown menu (e.g., CCPs, ER, MTs, or F-actin).
- Select the microscopy modality (WF, TIRF, or Confocal).

### Step 3: Apply Super-Resolution

- Click the **"Apply Super-Resolution"** button to start the reconstruction process.
- Once completed, the processed SR image will be displayed in napari.

### Step 4: Save the Results

- Click the **"Save Image"** button to export the SR image to your desired directory.

## Example Data

To test the functionality of CLAM, example datasets are available in the `example_data/` directory of the GitHub repository.
