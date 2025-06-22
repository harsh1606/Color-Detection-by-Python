# 🎨 Color Detection with OpenCV

## 📌 Overview
This interactive project detects colors in an image using **Python** and **OpenCV**. Just double-click anywhere on the image, and the tool will display the closest matching color name using a reference dataset. It's perfect for developers, designers, and learners working with image data or visual aesthetics.

---

## ✨ Features
✅ Click on any pixel to identify its color name  
✅ Matches RGB values against a rich color dataset (`colors.csv`)  
✅ Displays real-time color names and overlays them on the image  
✅ Automatically adjusts font color for optimal readability

---

## ⚙️ How It Works
1. Load an image by entering its path.
2. Double-click any pixel — the program captures its RGB values.
3. Finds the closest match in the color dataset.
4. Displays a rectangle with the color name on the image.

---

## 📁 Project Files
- **`Color_detection.ipynb`** — Full implementation notebook  
- **`colors.csv`** — Color dataset (with color names, hex codes, RGB values)

---

## 🧠 Sample Code
```python
# Function to return the closest color name
def Color_Name(R, G, B):
    minimum = 9999
    for i in range(len(file)):
        d = abs(R - int(file.loc[i,"R"])) + abs(G - int(file.loc[i,"G"])) + abs(B - int(file.loc[i,"B"]))
        if d <= minimum:
            minimum = d
            color_name = file.loc[i,"color_name"]
    return color_name
```

---

## 🚀 How to Run
1. Install the required libraries:
```bash
pip install numpy pandas opencv-python
```

2. Launch the notebook or run the script:
```bash
python Color_detection.ipynb
```

3. Input the path to your image file when prompted.  
4. Double-click anywhere on the image window to detect the color.

---

## 📦 Requirements
- Python 3.x  
- OpenCV  
- NumPy  
- Pandas

---

## 💡 Use Cases
- 🖌️ Graphic & Web Design Color Picking  
- 📷 Color Analysis in Photography  
- 🧪 Educational Demos in Computer Vision

---

## 👤 Author
**Harsh Kumar Tyagi**  
📧 [harshtyagi022@gmail.com](mailto:harshtyagi022@gmail.com)  
🪪 License: MIT
