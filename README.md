# 🍛 Bangladeshi Food Dataset

### Overview

The **Bangladeshi Food Dataset** is a curated image collection designed to advance research in **food recognition**, **computer vision**, and **cultural AI**.
It contains **10,000+ high-quality images** across **45 traditional Bangladeshi food categories**, including iconic dishes such as *Biriyani*, *Khichuri*, *Hilsha Fish*, *Roshogolla*, and *Pitha*.

This dataset aims to fill a major gap in current food recognition resources, which are predominantly Western-centric (e.g., Food-101, FoodX-251). The dataset provides a culturally rich, geographically diverse dataset representing authentic Bangladeshi cuisine — an underrepresented domain in global AI research.

---

### ✨ Key Features

* **58 distinct food categories** covering main dishes, sweets, snacks, and beverages
* **7,500+ labeled images** collected from diverse real-world sources (homes, restaurants, markets, and online platforms)
* **High-quality manual verification** to ensure accurate labels and clean data
* **Balanced representation** of urban and regional foods
* **Ready for ML pipelines** — organized in a `class_name/` folder structure compatible with PyTorch, TensorFlow, and Keras

---

### 📂 Dataset Structure

```
/
│
├── Biriyani/
│   ├── img_001.jpg
│   ├── img_002.jpg
│   └── ...
│
├── Hilsha_Fish/
│   ├── img_001.jpg
│   ├── img_002.jpg
│   └── ...
│
└── ... (58 total folders)
```

---

### 📊 Statistics

| Property                 | Value                                   |
| ------------------------ | --------------------------------------- |
| Total Images             | ~10,000                                  |
| Classes                  | 45                                      |
| Average Images per Class | 120–150                                 |
| Format                   | `.jpg`                                  |
| Image Resolution         | 256×256 (approx.)                       |
| Labels                   | Folder names correspond to class labels |

---

### 🧠 Motivation

Most large-scale food datasets (e.g., Food-101, ISIA Food-500) overrepresent Western dishes and underrepresent South Asian cuisines. This limits the performance and fairness of computer vision models across cultures.
**BFD-58** was created to bridge that gap by providing a high-quality, publicly available dataset centered on Bangladeshi culinary diversity — supporting fairer, more inclusive food recognition systems.

---

### 🚀 Usage

You can use this dataset for:

* Food image **classification** and **fine-grained recognition**
* **Transfer learning** and **PEFT** (Parameter-Efficient Fine-Tuning) experiments
* **Cross-cultural dataset comparison** (e.g., training on Food-101 and evaluating on BFD)
* **AI fairness** and **representation** studies in computer vision

Example (PyTorch):

```python
from torchvision import datasets, transforms

data_dir = "path/to/BFD-58"
transform = transforms.Compose([
    transforms.Resize((224, 224)),
    transforms.ToTensor()
])

dataset = datasets.ImageFolder(root=data_dir, transform=transform)
```

---

### 📑 Citation

If you use this dataset in your research, please cite:

```
@dataset{solaiman2025bfd58,
  title     = {A Comprehensive Dataset for Bangladeshi Food Recognition},
  author    = {Solaiman, Ishmam},
  year      = {2025},
  publisher = {GitHub},
  url       = {https://github.com/ishmam97/Bangladeshi-Food-Dataset}
}
```

---

### ⚖️ License

This dataset is released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.
You are free to use, share, and adapt the dataset with proper attribution.

---

### 📬 Contact

For questions, collaborations, or research inquiries:
**Ishmam Solaiman**
🌐 [ishmamsolaiman.com](https://ishmamsolaiman.com)
🔗 [LinkedIn](https://linkedin.com/in/iasolaiman) | [GitHub](https://github.com/ishmam97)
