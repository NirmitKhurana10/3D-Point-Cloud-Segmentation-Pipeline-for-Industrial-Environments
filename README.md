# 🏗️ 3D Point Cloud Segmentation Pipeline – S3DIS (Preprocessed)

This repository contains a full pipeline for preprocessing and segmenting 3D point cloud data from the [S3DIS dataset](http://buildingparser.stanford.edu/dataset.html), tailored for indoor industrial environments like offices, conference rooms, and hallways.

The project focuses on:
- 🧹 Cleaning and merging raw `.txt` point cloud files
- 🧠 Applying models like PointNet++, RandLA-Net, and KPConv
- 🏷️ Producing labeled 3D segments (e.g., walls, floors, chairs, tables)

---

## 📦 Preprocessed Dataset (4GB)

To avoid pushing large `.npy` files to GitHub, the full preprocessed dataset is hosted externally.

👉 **[Download Preprocessed S3DIS Data (Google Drive)](https://drive.google.com/drive/folders/1VxGy2V-jhwcDfsBCOza0n9ijOpg8BryP?usp=share_link)**  

### After downloading:
1. Unzip the folder.
2. Place it in the project root as:

/processed_dataset/

---

## 📂 Project Structure

📁 processed_dataset/         ← Place your downloaded data here


        ├── Area_1/
                ├── conferenceroom1
                        ├── color.npy
                        ├── coord.npy
                        ├── instance.npy
                        ├── segment.npy
                ...
        ...

📁 notebooks/                 ← Jupyter notebooks for preprocessing/modeling
📁 models/                    ← Pretrained model wrappers or configs
📁 utils/                     ← Helper functions
📄 README.md

---

## 🛠️ Getting Started

### 🔧 Create Python Environment
```bash
conda create -n pointcloud python=3.10
conda activate pointcloud
pip install -r requirements.txt

📗 Run Notebook

jupyter notebook
# Open and run any notebook under /notebooks/


⸻

🚫 .gitignore Note

This repo is set up to ignore .npy, .ply, and other large files using .gitignore.
Make sure you download the preprocessed dataset manually to run the code.

⸻

📬 Contact

If you have questions or need help, feel free to open an issue or contact:

Nirmit Khurana
📧 nirmitkhurana82@gmail.com
🖇️ LinkedIn : Khurananirmit10

⸻

📄 Citation

Armeni et al., “3D Semantic Parsing of Large-Scale Indoor Spaces”, CVPR 2016
Dataset Website

---
