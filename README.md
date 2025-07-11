
Pothole Detection using YOLOv8

This project presents a computer vision solution for detecting potholes on roads using the YOLOv8 object detection model. It was built in Google Colab using Python and trained on a custom-labeled dataset. The goal is to identify road hazards automatically and contribute to safer transportation systems, especially in areas prone to infrastructure damage.

---

Technologies Used

* YOLOv8 by Ultralytics
* Google Colab
* Python
* OpenCV
* Custom dataset in YOLO format

---

 Dataset

The dataset includes road images containing potholes, annotated using the YOLO format. It is stored as a zipped file on Google Drive and accompanied by a configuration file (`data.yaml`) required for training the model.

 Project Workflow

1. Required libraries are installed and the dataset is mounted from Google Drive into the Colab environment.
2. The YOLOv8 model (nano version) is used as the base model.
3. The model is trained over 20 epochs on the custom pothole dataset.
4. Once trained, the model is used to make predictions on new images.
5. The output images with bounding boxes around detected potholes are generated and saved for review.
6. pothole-detection-yolov8/

   Dataset and project Format:
│
├── 📁 dataset/
│   ├── images/
│   │   ├── train/
│   │   └── val/
│   ├── labels/
│   │   ├── train/
│   │   └── val/
│   └── data.yaml
│
├── pothole.zip                  # Zipped dataset (for Drive upload)
├── yolov8n.pt                   # Pre-trained YOLOv8n model
├── notebook.ipynb               # Main Colab notebook
├── README.md                    # Project documentation
└── 📁 runs/                      # YOLO output directory
    └── detect/
        └── train/               # Training weights, results, and logs
        └── predict*/            # Prediction output images


 Results

* The trained model successfully detects potholes in road images with good accuracy.
* The output images highlight potholes using bounding boxes.
* Results are stored in automatically created folders within the Colab environment for each prediction run.



Author

Malaika Shoukat
Email: [malaikashoukat594@gmail.com](mailto:malaikashoukat594@gmail.com)
LinkedIn: [linkedin.com/in/malaika-shoukat](https://www.linkedin.com/in/malaika-shoukat)


