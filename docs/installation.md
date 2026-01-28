# 🛠️ Installation Guide

This guide covers how to set up the **Bacterial Generation Determination** pipeline. You can choose to run the analysis in the cloud (Google Colab) or on your local machine.

## 🚀 Option 1: Google Colab (Zero Setup)
**Recommended for most users.**

You do not need to install Python or any libraries. The notebook handles the environment setup automatically.

1. **Open the Notebook:**
   Click the **"Open in Colab"** badge in the main README or [click here](https://colab.research.google.com/github/JoeVPhD/TrackMate_CellPose_Bacterial_Generation_Determination/blob/main/TrackMate_CellPose_Bacterial_Generation_Determination.ipynb).

2. **Run the Setup Cell:**
   The very first code cell in the notebook contains a script that detects you are in Colab and runs:
   ```python
   !pip install -q pandas numpy matplotlib seaborn scipy networkx
Connect Data:
The notebook will ask you to mount Google Drive. Ensure your TrackMate .csv files are uploaded to your Drive before starting.

💻 Option 2: Local Computer
Best for heavy processing or users who prefer privacy/offline access.

Prerequisites
Python 3.8 or higher.

Git (to download the repository).

A terminal (Command Prompt, PowerShell, or Terminal).

Step-by-Step Installation
1. Download the Repository
Open your terminal and run:

bash
git clone https://github.com/JoeVPhD/TrackMate_CellPose_Bacterial_Generation_Determination.git
cd TrackMate_CellPose_Bacterial_Generation_Determination
(Alternatively, you can download the ZIP file from GitHub and unzip it.)

2. Set Up a Virtual Environment (Recommended)
It is best practice to isolate this project so it doesn't conflict with other Python tools you use.

Using Conda (Anaconda/Miniconda):

bash
conda create -n bacterial_tracker python=3.10
conda activate bacterial_tracker
Using Standard Python (venv):
Windows:

bash
python -m venv venv
.\venv\Scripts\activate
Mac/Linux:

bash
python3 -m venv venv
source venv/bin/activate
3. Install Dependencies
We provide a requirements.txt file that lists all necessary libraries (Pandas, NetworkX, SciPy, etc.).

bash
pip install -r requirements.txt
4. Launch Jupyter
Start the notebook interface:

bash
jupyter notebook TrackMate_CellPose_Bacterial_Generation_Determination.ipynb
⚠️ Troubleshooting
"ModuleNotFoundError: No module named..."

You likely forgot to run pip install -r requirements.txt.

If you are in Conda, make sure you ran conda activate bacterial_tracker first.

"FileNotFoundError" when loading data

Ensure your input files follow the naming convention:

ExperimentName_spots.csv

ExperimentName_edges.csv

Windows Users: Avoid spaces in your folder paths if possible.

Graphviz / NetworkX Errors

This pipeline uses networkx which is pure Python. You generally do not need to install system-level Graphviz binaries for this specific notebook.

text

***

### Update your main `README.md`
Now, in your main README, simply add a clear, short pointer to this new file.

**Add this to `README.md`:**

```markdown
## 📦 Installation
For detailed instructions on setting up this tool locally or on Google Colab, please see our [Installation Guide](INSTALLATION.md).

**Quick Start:**
- **Cloud:** Click the "Open in Colab" badge above.
- **Local:** `pip install -r requirements.txt`
