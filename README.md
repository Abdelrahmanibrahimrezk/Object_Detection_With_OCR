# Object_Detection_With_OCR

<!-- ABOUT THE PROJECT -->
## About The Project

![out](https://user-images.githubusercontent.com/89320483/156454303-b6106985-f2d0-40ab-a2cc-be8de00b07f8.jpg)

I used the MobileNet SSD + deep neural network (dnn ) module in OpenCV to build our object detector.
Then i Compined it with OCR model.

## Getting Started

Here we will use Google colab and there is some specification to run it.

### Installation

  ```sh
  !sudo apt update

  !sudo apt install tesseract-ocr

  !sudo apt install libtesseract-dev

  !pip install pytesseract

  !pip uninstall -y Pillow
  # install the new one
  !pip install Pillow==5.3.0
  ```
  
### Run

  ```sh
  !python Image_object_detection.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel --image aa.jpg
  ```
  
### Display Output

  ```sh
  from google.colab.patches import cv2_imshow
  import cv2
  img = cv2.imread('out.jpg')
  cv2_imshow(img)
  ```
