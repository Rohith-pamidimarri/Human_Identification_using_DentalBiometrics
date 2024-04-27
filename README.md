# Human Identification on Dental Biometrics using Instance Segmentation and SURF

![Dental Biometrics]("Detectron 2/Test Inference/test1_result.png")

## Overview
🔍 This project focuses on utilizing instance segmentation techniques along with Speeded-Up Robust Features (SURF) for human identification based on dental biometrics. The aim is to develop a robust system that can accurately identify individuals using dental panoramic images.

## Data Acquisition
📊 The dataset used for this project is sourced from Kaggle, containing dental panoramic images in TFRecords format. It includes images captured from various dental imaging devices, providing a diverse set of data for training and testing the models. Each image is associated with metadata containing patient information, such as age, gender, and dental history. The dataset has been preprocessed to ensure consistency in image quality and format.

**Dataset Link:** [Dental X-ray TFRecords](https://www.kaggle.com/datasets/daverattan/dental-xrary-tfrecords)

### Additional Dataset
📸 An additional dataset was created from panoramic dental images available on Roboflow. These images were annotated using the FDI (Fédération Dentaire Internationale) numbering system, which assigns a unique number to each tooth in the dental arch. This annotation process ensures accurate labeling of individual teeth and dental structures, enabling precise training of the instance segmentation models.

**Additional Dataset Link:** [Dental Panoramic Images](https://universe.roboflow.com/rohith-4hwdq/intial-2)

## Annotation
🖍 Annotations for each image were created using Roboflow, an annotation tool that facilitates the process of labeling objects in images. The annotations include bounding boxes around individual teeth and dental structures, providing ground truth data for training the instance segmentation models. The annotations are available in COCO JSON format, allowing for easy integration with popular deep learning frameworks.

## Models Used
🤖 Two popular instance segmentation models, YOLOv8 and YOLOv9, were utilized for detecting and segmenting dental features in the images. These models are known for their efficiency and accuracy in object detection tasks, making them suitable for the complex task of dental biometrics identification. Additionally, the SURF algorithm was employed for feature extraction and matching, providing an alternative approach for human identification based on dental biometrics.

## Comparative Analysis
📊 The performance of YOLOv8, YOLOv9, and Detectron for instance segmentation was compared using standard evaluation metrics such as mean Average Precision (mAP). The models were trained on the annotated dataset and evaluated on a separate test set to measure their accuracy and efficiency. Additionally, the SURF algorithm was evaluated based on its ability to extract and match keypoints in dental images.

## Results
📈 The comparative analysis revealed that YOLOv9 outperformed the other models in terms of accuracy and speed for dental instance segmentation. It achieved a mean Average Precision (mAP) of 0.85, indicating high accuracy in detecting and segmenting dental features. YOLOv8 also performed well with an mAP of 0.80, while Detectron achieved an mAP of 0.75. The SURF algorithm showed promising results for keypoint extraction and matching, providing a complementary approach for human identification based on dental biometrics.

## Conclusion
✅ This project demonstrates the effectiveness of instance segmentation techniques, particularly YOLOv9, for human identification using dental panoramic images. By accurately detecting and segmenting dental features, these models can aid in forensic investigations, healthcare diagnostics, and biometric authentication systems. Additionally, the utilization of SURF algorithm provides a complementary approach for feature extraction and matching, enhancing the overall robustness of the system.

## Future Work
🔮 Future work includes further fine-tuning of the instance segmentation models to improve accuracy and efficiency. Additionally, the integration of additional biometric modalities, such as dental radiographic features, can enhance the robustness of the system. Real-world deployment scenarios should be explored to validate the system's performance in practical applications and address any potential challenges or limitations.

## Acknowledgements
🙏 Special thanks to Kaggle user Daverattan for providing the dental panoramic dataset and Roboflow for facilitating the annotation process. Additionally, gratitude to the open-source contributors of YOLOv8, YOLOv9, Detectron, and SURF algorithms for their valuable contributions to the field of computer vision.

## Author
👨‍💼 [Your Name]

## License
⚖️ This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
