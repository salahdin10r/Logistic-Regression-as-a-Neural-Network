# Logistic-Regression-as-a-Neural-Network
This project implements a **Logistic Regression model** from scratch using a neural network perspective to classify images as **cat 🐱 or non-cat 🚫🐱**.

---

## 📌 Overview

- Build a binary image classifier using **logistic regression**
- Treat logistic regression as a **single-layer neural network**
- Train and evaluate the model on a labeled dataset of images

---

## 🧰 Tech Stack

- Python
- NumPy
- Matplotlib
- h5py
- SciPy
- Pillow (PIL)

Install dependencies:

```bash
pip install numpy matplotlib h5py scipy pillow
````

---

## 📊 Dataset

The dataset contains:

* **Training set**: 209 images
* **Test set**: 50 images
* Image size: **64 × 64 × 3 (RGB)**

Each image is labeled:

* `1` → Cat 🐱
* `0` → Non-cat

---

## ⚙️ Project Pipeline

### 1. Data Preprocessing

* Flatten images into vectors
* Normalize pixel values (divide by 255)

### 2. Model Architecture

Logistic Regression (as a Neural Network):

[
z = w^T x + b
]
[
a = sigmoid(z)
]

### 3. Key Functions Implemented

* `sigmoid()` → activation function
* `initialize_with_zeros()` → initialize parameters
* `propagate()` → forward + backward propagation
* `optimize()` → gradient descent
* `predict()` → make predictions
* `model()` → full pipeline

---

## 📈 Results

* **Training Accuracy**: ~91%
* **Test Accuracy**: ~34%

⚠️ The model shows **overfitting** due to:

* Small dataset
* Linear model limitations

---

## 📉 Learning Curve

The cost decreases over iterations, showing the model is learning:

```python
plt.plot(costs)
```

---

## 🧪 Experiments

Tested different learning rates:

| Learning Rate | Train Accuracy | Test Accuracy |
| ------------- | -------------- | ------------- |
| 0.01          | 71%            | 34%           |
| 0.001         | 74%            | 34%           |
| 0.0001        | 66%            | 34%           |

---

## 🖼️ Custom Image Prediction

You can test your own image:

1. Add image to `images/` folder
2. Update filename in code
3. Run prediction

---

## 📚 Key Takeaways

* Data preprocessing is critical
* Logistic regression can be viewed as a neural network
* Hyperparameters (like learning rate) matter a lot
* Overfitting is common with small datasets

---

## 🚀 Future Improvements

* Add regularization to reduce overfitting
* Use a deeper neural network
* Increase dataset size
* Try CNNs for better image performance

---

## 📖 References

* [http://www.wildml.com/2015/09/implementing-a-neural-network-from-scratch/](http://www.wildml.com/2015/09/implementing-a-neural-network-from-scratch/)
* [https://stats.stackexchange.com/](https://stats.stackexchange.com/)

---

## 👨‍💻 Author

* GitHub: [https://github.com/salahdin10r](https://github.com/salahdin10r)

````

---

## 🧠 Extra (makes you look pro)

After creating it:

```bash
touch README.md
````

Paste content → then:

```bash
git add README.md
git commit -m "Add README"
git push
```

