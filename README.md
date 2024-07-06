# Coarse-to-Fine Deep Learning Method for OC and OD Segmentation in Fundus Eye Images

This project implements a coarse-to-fine deep learning approach for the segmentation of the optic cup (OC) and optic disk (OD) in fundus eye images, specifically for the purpose of glaucoma detection. The method leverages both object annotations and boundary annotations to enhance the accuracy of segmentation. The fundus eye images used in this project are obtained from the publicly available REFUGE dataset.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Methodology](#methodology)
  - [Coarse Segmentation](#coarse-segmentation)
  - [Fine Segmentation](#fine-segmentation)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Acknowledgements](#acknowledgements)

## Introduction

Glaucoma is a severe eye condition that can lead to blindness if not detected and treated early. One of the key indicators of glaucoma is the change in the shape and size of the optic cup (OC) and optic disk (OD) in fundus eye images. This project aims to develop a deep learning model that can accurately segment the OC and OD to assist in the early detection of glaucoma.

## Dataset

The REFUGE (Retinal Fundus Glaucoma Challenge) dataset is used for training and testing the deep learning models. The dataset includes high-quality fundus images along with ground truth annotations for the OC and OD.

- [REFUGE Dataset](https://refuge.grand-challenge.org/)

## Methodology

The segmentation process is divided into two stages: coarse segmentation and fine segmentation.

### Coarse Segmentation

In the first stage, a coarse segmentation model is trained to identify the approximate location and boundaries of the OC and OD. This model uses object annotations to create initial segmentation masks.

### Fine Segmentation

In the second stage, a fine segmentation model is applied to the coarse segmentation results. This model refines the boundaries of the OC and OD using boundary annotations to improve the accuracy of the segmentation.

## Installation

To run this project, you need to have Python and the required libraries installed. You can install the dependencies using the following command:

```bash
pip install -r requirements.txt
