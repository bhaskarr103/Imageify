
# Notion-Style Illustrations SaaS

A SaaS application that transforms text descriptions into Notion-style illustrations, allowing users to create beautiful visuals effortlessly. Built using **React**, **ShadCN UI**, **Node.js**, **Express.js**, and other modern technologies.

![Notion-Style Illustrations SaaS](https://github.com/user-attachments/assets/826e09bf-315c-4487-89cb-7039d3e18dbb)

This project is mainly inspired by the [Generative Adversarial Text-to-Image Synthesis paper](<https://arxiv.org/abs/1605.05396>). We implemented this model using PyTorch. In this model, we train a conditional generative adversarial network, conditioned on text captions, to generate images that correspond to the captions. The network architecture is shown below. This architecture is based on DCGAN.

### DCGAN Network Architecture

![DCGAN Network Architecture](https://github.com/Rakshith-Manandi/text-to-image-using-GAN/blob/master/images/dcgan_network.png)

The architecture used for the GAN model.



## Features

- **Text to Image Conversion**: Converts user-provided text into beautiful Notion-style illustrations.
- **Responsive Design**: Built using React and ShadCN UI for a seamless experience across devices.
- **Express Backend**: Utilizes Node.js and Express.js for handling API requests and managing image processing.
- **Search Functionality**: Users can search for illustrations based on categories or descriptions.
- **User Authentication**: (Optional) Allows users to create accounts, save favorites, and manage their creations.

---

## **Text to Image Synthesis using Generative Adversarial Networks**

### Introduction

This project is inspired by the paper *Generative Adversarial Text-to-Image Synthesis* [1]. We implemented the model using **PyTorch**. It uses a conditional generative adversarial network (GAN), trained on text captions to generate images that correspond to the captions. The architecture is based on **DCGAN**.

### Datasets

We used datasets in **HDF5** format, which were converted from the **Caltech-UCSD Birds 200** and **Oxford Flowers** datasets. Text embeddings were sourced from the original paper authors ([1]).

### Requirements

- **PyTorch**
- **h5py**
- **EasyDict**
- **PIL**
- **Numpy**

**Note**: This implementation requires GPU support. To install dependencies, use:

```bash
pip install -r requirements.txt
```

### Training

To train the model:

1. Clone the repository:
   ```bash
   git clone https://github.com/Shivam-fibo/Imageify.git
   ```
 
2. Start the training process:
   ```bash
   python -u runtime.py
   ```

**Inputs for Training/Prediction**:
- `dataset`: The dataset to use (`birds | flowers`).
- `split`: Split of data (0: train | 1: valid | 2: test).
- `save_path`: Directory for saving models and results.
- `pre_trained_disc`: Path to pre-trained discriminator model.
- `pre_trained_gen`: Path to pre-trained generator model.
- `cls`: Boolean flag to use classification algorithms.

### Demo

To see a demo of the results, follow these steps:

1. Install dependencies and ensure you have GPU access.
2. Run the demo:


### Results

Here are a few examples of images generated by the model (examples to be added):

---

## Technologies Used

- **Frontend**: 
  - React.js 
  - ShadCN UI
  - Tailwind CSS

- **Backend**:
  - Node.js
  - Express.js

---

## Getting Started

### Prerequisites

To run this project, you’ll need **Node.js** and **npm** installed on your machine.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Shivam-fibo/Imageify.git
   ```
2. Navigate to the project directory:
   ```bash
   cd your-repo-name
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the backend server:
   ```bash
   npm run dev
   ```
5. Navigate to the frontend directory and start the React app:
   ```bash
   cd frontend
   npm start
   ```

### Usage

1. Open the app in your browser at `http://localhost:3000`.
2. Input a description to generate a Notion-style illustration.
3. Explore illustrations and manage your profile.

---

## Project Structure

```bash
.
├── backend                 # Backend Node.js server
├── frontend                # React.js frontend
├── public                  # Public assets like images and icons
├── README.md               # Documentation
├── package.json            # Backend dependencies and scripts
└── ...
```

---

## Contributing

Feel free to open an issue or submit a pull request if you have any ideas or improvements.

---

## License

This project is licensed under the ISC License.

---

### References

1. Generative Adversarial Text-to-Image Synthesis: https://arxiv.org/abs/1605.05396
2. Original Implementation by the Authors: https://github.com/reedscot/icml2016

---

Let me know if you need any more adjustments!
---
**Author**: Prince Pal
