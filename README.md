# PlateSniper

**PlateSniper** is an advanced object detection project leveraging YOLOv10 to accurately identify and extract car license plates from images and videos in real-time. Designed for high precision and speed, PlateSniper is ideal for applications in traffic monitoring and automated vehicle identification.

## Features

- **High Accuracy**: Utilizes the YOLOv10 architecture for real-time object detection.
- **License Plate Detection**: Specifically optimized to detect and identify car license plates.
- **Custom Dataset**: Includes a curated dataset for training and testing.
- **Video Processing**: Capable of detecting license plates in video streams.

## Installation

1. Clone the YOLOv10 repository:

   ```bash
   git clone https://github.com/THU-MIG/yolov10.git
   ```

2. Clone this repository:

   ```bash
   git clone https://github.com/SachinMhetre678/PlateSniper.git
   cd PlateSniper
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Run the Jupyter notebook or script to perform object detection:

   ```bash
   jupyter notebook Object_Detection_Yolov10.ipynb
   ```

## Dataset

This repository includes a custom dataset specifically designed for car license plate detection. The dataset contains labeled images of vehicles with corresponding annotations for license plates.

- **Dataset Structure**:
  - `images/`: Contains all the images used for training and testing.
  - `labels/`: Contains the annotations for each image in YOLO format.

Make sure to check the `data.yaml` file to ensure that all paths to your dataset are correctly set. This file contains the paths to your training, validation, and testing data, and it is crucial for the model to locate and use the data properly.

## Usage

### Image Detection

To detect license plates in an image:

```python
!python detect.py --weights yolov10.pt --source data/images
```

### Video Detection

To detect license plates in a video:

```python
!python detect.py --weights yolov10.pt --source data/videos
```

## Results

### Example Detection on Video

Below are two videos demonstrating license plate detection using YOLOv10:

#### Video 1

![Video 1](https://github.com/user-attachments/assets/1b6442a8-0482-481c-afb5-54efe63a17ac)

#### Video 2

![Video 2](https://github.com/user-attachments/assets/4ae2ff96-3aa8-4cae-91ba-124ca037e47f)

## Contributing

Feel free to contribute to this project by submitting a pull request or reporting any issues.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
