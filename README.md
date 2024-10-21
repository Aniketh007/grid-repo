
# FLipkart GRID ROBOTICS CHALLENGE -- QC AUTOMATION

Complete Architecture:

![image](https://github.com/user-attachments/assets/d393e05e-c866-4df0-9bf4-288637c5aa17)


## Testing using Kaggle Notebooks :
(ipynb files)

Final : https://www.kaggle.com/code/rohansai2208/final

Packed unpacked detection : https://www.kaggle.com/code/rohansai2208/packed-unpacked/notebook

QWEN OCR : https://www.kaggle.com/code/rohansai2208/qwen-ocr-01



## Overview

This project is an advanced image analysis system designed to process and classify both single and multiple object images. It utilizes state-of-the-art machine learning models to segment, classify, and extract detailed information from images of packed and unpacked items, with a focus on groceries and household products.

## Key Features

1. **Dual Image Processing**: Analyzes both front and back images of objects.
2. **Single and Multiple Object Handling**: Capable of processing images containing single or multiple objects.
3. **Object Segmentation**: Uses SAM (Segment Anything Model) for precise object detection and segmentation in multi-object images.
4. **Classification**: 
   - Packed vs Unpacked items
   - Fruit and Vegetable classification (54 categories)
   - Fresh vs Rotten for produce items
5. **Detailed Product Information Extraction**: For packed items, extracts product name, expiry date, description, and category.
6. **Output Generation**: Produces CSV files for combined items, packed items, and unpacked items.

## Technologies Used

- Python 3.x
- PyTorch and torchvision
- Ultralytics SAM
- OpenCV
- Pandas
- Pillow (PIL)
- Scikit-learn
- Transformers (Hugging Face)
- Matplotlib

## Models

1. **SAM (Segment Anything Model)**: For object segmentation
2. **EfficientNet-B0**: 
   - Packed/Unpacked classification
   - Fruit/Vegetable classification (54 categories)
   - Fresh/Rotten classification
3. **Qwen2VL**: For extracting detailed product information

## Setup and Installation

1. Clone the repository:
   ```
   git clone [repository-url]
   cd [repository-name]
   ```

2. Install required packages:
   ```
   pip install -r requirements.txt
   ```

3. Ensure you have the following pre-trained model files in the appropriate directory:
   - `sam2_b.pt`
   - `efficientnet_b0_packed_unpacked.pth`
   - `efficientnet_b0_fruit_veg_1.pth`
   - `efficientnet_b0_fruit_veg.pth`

## Usage

The main execution code is contained in `final.ipynb`. To use the system:

1. Open `final.ipynb` in a Jupyter Notebook environment.
2. Run all cells in the notebook.
3. When prompted, specify whether you're processing a single object or multiple objects.
4. Provide the paths to the front and back images when asked.
5. The system will process the images and generate CSV files with the results.

## Output

The script generates three CSV files:
1. `combined_items.csv`: All processed items
2. `packed_items.csv`: Information on packed items
3. `unpacked_items.csv`: Information on unpacked items (fruits, vegetables)

## Project Structure

- `final.ipynb`: Main Jupyter notebook containing all functions and the execution flow
- `requirements.txt`: List of required Python packages
- `README.md`: This file
- Other supporting Python scripts and model files

## Future Improvements

- Implement a graphical user interface for easier interaction
- Enhance object matching between front and back images
- Integrate with a database for persistent storage
- Add support for video processing
- Implement more robust error handling and logging

## Contributors

Aniketh : https://github.com/Aniketh007

## License

[MIT License]

---

This README provides a comprehensive overview of your project, including its features, technologies used, setup instructions, and usage guidelines. It's tailored to the fact that the main execution is in a Jupyter notebook (`final.ipynb`). Users can easily understand how to set up and use your image analysis system based on this documentation.

Citations:
[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/13521434/c8d83959-3b01-4518-ae43-2385fc197b0e/paste.txt
