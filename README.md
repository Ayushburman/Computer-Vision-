# Computer-Vision
# Display Images in Various Formats Using Different Color Models

## 📌 Aim

To display and analyze images in different color models such as **RGB, Grayscale, HSV, and Lab** using **OpenCV** and **Matplotlib** in Python.

---

# 📖 Description

This experiment demonstrates how digital images can be represented and visualized using different color spaces.
Different color models are useful for image processing, computer vision, segmentation, enhancement, and analysis.

---

# 🧠 Step 1: Introduction to Image Formats and Color Models

## 🖼️ Common Image Formats

| Format   | Description             | Advantages           | Use Cases         |
| -------- | ----------------------- | -------------------- | ----------------- |
| JPG/JPEG | Compressed image format | Small file size      | Photography       |
| PNG      | Lossless compression    | Transparency support | Web graphics      |
| BMP      | Bitmap image format     | High quality         | Raw image storage |

---

## 🌈 Color Models

| Color Model | Description                | Applications          |
| ----------- | -------------------------- | --------------------- |
| RGB         | Red, Green, Blue channels  | Digital displays      |
| Grayscale   | Black & white intensity    | Simplified processing |
| HSV         | Hue, Saturation, Value     | Color detection       |
| Lab         | Lightness + color channels | Color correction      |

---

# ⚙️ Step 2: Setup and Installation

## Install Required Libraries

### Using pip

```bash
pip install opencv-python matplotlib
```

### Using conda

```bash
conda install opencv matplotlib
```

---

# 🖼️ Step 3: Image Acquisition

* Choose or download sample images.
* Use images with different colors and textures for better visualization.
* Supported formats:

  * `.jpg`
  * `.png`
  * `.bmp`

---

# 📥 Step 4: Reading Images

Use OpenCV to load an image.

```python
import cv2

image = cv2.imread("image.jpg")
```

### Explanation

* `cv2.imread()` reads the image from disk.
* Returns image as NumPy array.
* Default format in OpenCV → **BGR**

---

# 🔄 Step 5: Conversion to Different Color Models

## 🔴 RGB Model

```python
rgb = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
```

### Purpose

Represents image using:

* Red
* Green
* Blue channels

---

## ⚫ Grayscale Conversion

```python
gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
```

### Benefits

* Reduced complexity
* Faster processing
* Useful in edge detection

---

## 🌈 HSV Conversion

```python
hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)
```

### Components

* Hue
* Saturation
* Value

### Applications

* Color segmentation
* Object tracking

---

## 🎨 Lab Conversion

```python
lab = cv2.cvtColor(image, cv2.COLOR_BGR2LAB)
```

### Applications

* Color balancing
* Perceptual color analysis

---

# 📊 Step 6: Visualization with Matplotlib

```python
import matplotlib.pyplot as plt

plt.imshow(rgb)
plt.show()
```

### Purpose

* Display images
* Compare different color spaces
* Visualize transformations

---

# 💾 Step 7: Saving Processed Images

```python
cv2.imwrite("gray.jpg", gray)
```

### Supported Formats

* JPG
* PNG
* BMP

---

# 🧪 Complete Python Program

```python
import cv2
import matplotlib.pyplot as plt

# Read image
image = cv2.imread("image.jpg")

# Convert image
rgb = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)
lab = cv2.cvtColor(image, cv2.COLOR_BGR2LAB)

# Display images
plt.figure(figsize=(10,8))

plt.subplot(2,2,1)
plt.imshow(rgb)
plt.title("RGB")

plt.subplot(2,2,2)
plt.imshow(gray, cmap='gray')
plt.title("Grayscale")

plt.subplot(2,2,3)
plt.imshow(hsv)
plt.title("HSV")

plt.subplot(2,2,4)
plt.imshow(lab)
plt.title("Lab")

plt.tight_layout()
plt.show()
```

---

# 📌 Output

| RGB                        | Grayscale                      |
| -------------------------- | ------------------------------ |
| Color image representation | Black and white representation |

| HSV                      | Lab                             |
| ------------------------ | ------------------------------- |
| Hue-based representation | Perceptual color representation |

---

# ✅ Result

Successfully displayed images in multiple color models:

* RGB
* Grayscale
* HSV
* Lab

using **OpenCV** and **Matplotlib**.

---

# 📚 Applications

* Computer Vision
* Medical Imaging
* Face Detection
* Object Tracking
* Image Segmentation
* AI & Deep Learning

---

# 🎯 Conclusion

This experiment helped understand:

* Different image formats
* Various color models
* Image conversion techniques
* Visualization using Python libraries

It also demonstrated how different color spaces are useful for specific image processing tasks.

---

# 🚀 Future Scope

* Real-time video processing
* Face recognition systems
* Object detection
* Deep learning image pipelines
* Advanced color segmentation




----------------------------------------------------------------------
# Exp 1.2 
## Aim-Convert color images into monochrome images and demonstrate image color conversion techniques.
**Description**

![image](https://github.com/user-attachments/assets/d275a51a-f110-4790-8ddd-78df5a5b4532)

![image](https://github.com/user-attachments/assets/612501f1-ffe9-431a-b8dd-69c2e6bebcdf)

![image](https://github.com/user-attachments/assets/b63ebcbb-d338-4c21-925f-324ec60f9c4d)

![image](https://github.com/user-attachments/assets/b5238e1f-7377-49ed-bcd0-4f6b992aabd6)

**Output**

![image](https://github.com/user-attachments/assets/6059ee65-d390-4daa-b141-0960a75f1406)

**Explaination**

![image](https://github.com/user-attachments/assets/edb7f42a-ea50-441e-95de-b67153ae303c)

**Learning Outcome**

![image](https://github.com/user-attachments/assets/72a1a511-68f2-4ff8-86f2-bfcf91b4443b)




----------------------------------------------------------------------
# Exp 1.3 
## Aim-Apply image enhancement techniques using grey level transformations.
**Description**

![image](https://github.com/user-attachments/assets/0544460d-1bed-4c6f-9db6-a8c49b20d28b)

![image](https://github.com/user-attachments/assets/11871ab6-5905-4a65-bc23-2126ed301453)

![image](https://github.com/user-attachments/assets/361d7071-561c-407d-9eee-fa5720e111bc)

![image](https://github.com/user-attachments/assets/d297b23b-4924-4eb6-9286-f44924172f31)

![image](https://github.com/user-attachments/assets/8576801b-f339-43a2-8665-fb17df141cd0)


**Output**

![image](https://github.com/user-attachments/assets/c8ce3478-4b06-4d3b-8638-51818ddd793c) ,  ![image](https://github.com/user-attachments/assets/e921a539-89d6-4bb0-a2f8-e21ee994e6f1) , ![image](https://github.com/user-attachments/assets/262015a6-fafe-4818-a84a-69117e627fb1) , ![image](https://github.com/user-attachments/assets/50cc071f-3606-465b-b768-7de7112f179e) , ![image](https://github.com/user-attachments/assets/571d791e-0318-4149-b461-12db806da858) , ![image](https://github.com/user-attachments/assets/32bbd4f3-769d-42bc-9f8a-68982d109b08)


**Explaination**

![image](https://github.com/user-attachments/assets/f81c17cc-6ccd-4865-8311-6fd7b266d74f)

**Learning Outcome**

![image](https://github.com/user-attachments/assets/c94ef46a-f4e6-48ac-a7bb-7040c0fe6868)





----------------------------------------------------------------------
# Exp 1.4 
## Aim-Perform histogram matching and specification on images.

**Description**

![image](https://github.com/user-attachments/assets/e57247fe-1ff7-47f2-974c-1c07766c727b)


**Output**

![image](https://github.com/user-attachments/assets/73858f47-e158-4763-99fc-d120c3c700fa)

![image](https://github.com/user-attachments/assets/9c3df8a9-420d-4f5b-962a-0e2eb63e4674)



**Explaination**

![image](https://github.com/user-attachments/assets/c9ada243-a00b-45e4-bc6b-a8f6cf0e302e)

![image](https://github.com/user-attachments/assets/bad5e914-da83-42de-80a7-c9684cfee379)

![image](https://github.com/user-attachments/assets/7b5c99a4-9d11-450c-9290-225756eaa0a0)

![image](https://github.com/user-attachments/assets/5844b677-627a-4039-954d-81e1e7dfc8cc)

**Learning Outcome**

![image](https://github.com/user-attachments/assets/aa344223-ac0f-4a32-848f-f70cb564caac)

----------------------------------------------------------------------
# Exp 2.1 
## Aim-Display images in various formats using different color models.

**Description**

![image](https://github.com/user-attachments/assets/3267df32-9eea-4106-8180-9b5dec5a1c31)


**Output**

![image](https://github.com/user-attachments/assets/56d89573-5a7e-421a-a1d3-2ebf0c4526a6)

![image](https://github.com/user-attachments/assets/38d44503-3be4-495f-9b7b-df7e5422e9e6)

**Explaination**

![image](https://github.com/user-attachments/assets/0692cf93-8c66-4ca4-9aa0-d84ddac6b5eb)

![image](https://github.com/user-attachments/assets/a9f5500e-3151-414a-b2ed-aba7e1ac4c89)


**Learning Outcome**

![image](https://github.com/user-attachments/assets/8b5e7027-1725-4101-b2fe-16534735d63d)

----------------------------------------------------------------------
# Exp 2.2
## Aim-Remove noise from images and apply inverse filtering.

**Description**

![image](https://github.com/user-attachments/assets/f4a3010f-4b83-4752-8459-d57132763697)

**Output**

**Explaination**

![image](https://github.com/user-attachments/assets/90643ec8-d138-461f-92eb-56c4d2d1c0e4)

![image](https://github.com/user-attachments/assets/f6ebc0ba-925c-4bd5-bb6f-13ce71ab0a11)

**Output**
![image](https://github.com/user-attachments/assets/f201a029-ba5a-4965-9d8c-ac4b041b563c)


**Learning Outcome**

![image](https://github.com/user-attachments/assets/262d5bab-0d85-4a04-a2d8-79e791d87c69)

----------------------------------------------------------------------
# Exp 2.3 
## Aim-Conduct image morphological operations.

**Description**

![image](https://github.com/user-attachments/assets/66d4749e-9e1a-4546-a471-dcc70c183b11)


**Output**

![image](https://github.com/user-attachments/assets/c7ca9880-26ec-41fc-bcd7-f6c73ac9a72d)


**Explaination**

![image](https://github.com/user-attachments/assets/1d2ccab4-4425-4000-b0d0-4d39f6d92e0e)

![image](https://github.com/user-attachments/assets/690ec8e1-75d4-4be0-bfd9-0794b26a293c)

![image](https://github.com/user-attachments/assets/ca396ff3-9d5a-4548-8ce7-3c2c66bfae0f)


**Learning Outcome**

![image](https://github.com/user-attachments/assets/2b710ffd-d3b6-4467-b75d-01b5833253ae)

----------------------------------------------------------------------
# Exp 3.1 
## Aim-Detect points, lines, edges, and boundaries in images.

**Description**

![image](https://github.com/user-attachments/assets/335725d4-ee60-4c13-b45e-f1c4052088c0)


**Output**

![image](https://github.com/user-attachments/assets/86d664a4-aac2-4bc7-8ebd-1f7cb80c912c)

**Explaination**

![image](https://github.com/user-attachments/assets/b63ddf26-c41d-4ea3-844f-227dc8bb4673)

![image](https://github.com/user-attachments/assets/f19bb3b2-c3db-4038-a54f-930c9dc94aa0)


**Learning Outcome**

![image](https://github.com/user-attachments/assets/3119efc7-99c8-401e-8cb1-4cf6dce90f20)

----------------------------------------------------------------------
# Exp 3.2
## Aim-Implement boundary linking, representation, and description  techniques on images.


**Description**

![image](https://github.com/user-attachments/assets/985daa53-8558-4751-bfa7-60eae9424a31)

![image](https://github.com/user-attachments/assets/911cf987-2c08-443f-80ec-f6f366ee21aa)


**Output**

![image](https://github.com/user-attachments/assets/b7e7631a-320f-45ac-8758-9003e519e5a3)


**Explaination**

![image](https://github.com/user-attachments/assets/24f5ff40-5a3e-4bef-bcb7-5f6d98e71706)

![image](https://github.com/user-attachments/assets/1db44bc2-04f8-4a54-97d3-d8982bfa702d)

**Learning Outcome**

![image](https://github.com/user-attachments/assets/825cd73d-6c0e-4953-9c55-84818bc3a9b5)

----------------------------------------------------------------------
# Exp 3.3 
## Aim-Develop an application of computer vision using a convolutional neural network.

**Description**

![image](https://github.com/user-attachments/assets/ac209401-f807-4883-b13b-523de81689de)

![image](https://github.com/user-attachments/assets/fcf7ed0d-27a0-4e07-acd1-36caba05fc6a)


**Output**

![image](https://github.com/user-attachments/assets/5fbab602-65fc-46c5-84c0-66b2fabc3ff1)

![image](https://github.com/user-attachments/assets/8dad408b-487d-4712-9b9b-dcbcfdde0882)

![image](https://github.com/user-attachments/assets/2ba9902d-bcca-4cd6-a034-2794fb0957ef)


**Explaination**

![image](https://github.com/user-attachments/assets/3ca554d3-8366-422b-8ae9-dcd6e607801f)

![image](https://github.com/user-attachments/assets/cd0b8375-1997-4cce-ad74-b04d72d68440)

**Learning Outcome**

![image](https://github.com/user-attachments/assets/b6a5f0ed-bb3c-4c2c-bcf0-5598b28d57d6)

![image](https://github.com/user-attachments/assets/a9c379f1-b369-4706-93ff-30ecae5f0b31)

----------------------------------------------------------------------
