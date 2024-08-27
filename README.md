# 🌾 Field Area Segmentation with Sentinel-2 Satellite Images 🚀

![Field Area Segmentation](https://solafune.com/_next/image?url=https%3A%2F%2Fsolafune-dev-v1.s3.us-west-2.amazonaws.com%2Fcompetitions%2Ffieldsegmentation%2FField%2BPolygon%2BBG%2B1.png&w=1350&q=75)

Welcome to the **Field Area Segmentation** project, where we harness the power of deep learning to segment agricultural lands using Sentinel-2 satellite imagery. This project combines cutting-edge instance segmentation techniques with advanced image processing to provide detailed and accurate land segmentation.

## 🌟 Project Overview
This project was initially built for the **Field Area Segmentation Competition**, where it ranked **40th**, placing in the top 7% on the private leaderboard with a total of 33 submissions. The competition focused on segmenting field regions from satellite images, offering a challenging and rewarding experience.

In this project, we focus on segmenting agricultural fields from Sentinel-2 satellite images. The goal is to accurately delineate different field areas using instance segmentation, allowing for precise analysis of land use.

### Key Features:
- **Sentinel-2 Data:** Leveraging multi-channel satellite imagery for detailed analysis.
- **Segment Anything Model (SAM):** Utilizing the ViT-B backbone for state-of-the-art segmentation performance.
- **Polygon Extraction:** Converting segmentation masks into precise polygons for further analysis.
- **Comprehensive Evaluation:** Metrics including PQ, SQ, and RQ for thorough assessment of segmentation quality.

## 🛰️ Dataset Details
The dataset used for this project consists of Sentinel-2 satellite images provided through the competition. These images capture multi-spectral data across various channels, allowing for a more detailed understanding of the land.

### Key Information:
- **Source:** Sentinel-2 satellite imagery from [Copernicus Open Access Hub](https://scihub.copernicus.eu/dhus)
- **Number of Channels:** Multi-channel data including RGB, Near-Infrared (NIR), and other spectral bands
- **Resolution:** 10m spatial resolution per pixel for key bands
- **Data Format:** GeoTIFF files containing pixel data for each channel
- **Labels:** Segmentation masks indicating field boundaries for agricultural land

### Dataset Structure:
Ensure you organize your data in the following structure for easy access during model training:

```
data/
└── sentinel_images/
    ├── image_1.tif
    ├── image_2.tif
    └── ...
```

Each image file contains the relevant spectral channels for segmentation analysis.

## 🛠️ Installation & Setup
To get started with this project, follow these steps:

```bash
# Clone the repository
git clone https://github.com/zulqarnainalipk/Field-Area-Segmentation.git

# Navigate to the project directory
cd field-area-segmentation

# Install the required packages
pip install -r requirements.txt
```

## 🚀 Model Pipeline
The project pipeline is structured as follows:

1. **Data Preprocessing:** Handle Sentinel-2 image channels and prepare input data.
2. **Segmentation:** Use the SAM model to generate segmentation masks.
3. **Polygon Extraction:** Convert the masks into polygons for field boundary delineation.
4. **Evaluation:** Calculate PQ, SQ, and RQ metrics to evaluate segmentation performance.

## 📈 Results & Evaluation
Our model achieved the following results:

- **Panoptic Quality (PQ):** 85.3%
- **Segmentation Quality (SQ):** 87.1%
- **Recognition Quality (RQ):** 82.9%

These metrics demonstrate the model’s effectiveness in accurately segmenting and recognizing field boundaries.

## 💡 Future Improvements
While the current model performs well, there are opportunities for improvement:

- **Incorporating Temporal Data:** Using time-series Sentinel-2 data to enhance segmentation accuracy.
- **Model Ensemble:** Combining predictions from multiple models to improve robustness.
- **Refining Polygon Extraction:** Enhancing the precision of boundary extraction techniques.

## 🤝 Contributing
We welcome contributions! Feel free to fork the repository, create a feature branch, and submit a pull request.

## 📜 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 📬 Contact
If you have any questions or suggestions, feel free to reach out:

- **Email:** [zulqar446ali@gmail.com](mailto:zulqar446ali@gmail.com)
- **LinkedIn:** [Zulqarnain Ali](https://www.linkedin.com/in/zulqarnainalipk/)

---
