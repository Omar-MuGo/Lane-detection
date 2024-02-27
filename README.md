# Lane Detection with CARLA Simulation

[![Lane Detection DEMO](https://github.com/Omar-MuGo/Lane-detection/blob/c3ab1bafd82881c533831197c25b2ba10f250779/Images/thumbnail.png)](https://www.youtube.com/watch?v=Ye1y3uwR9ko))
## Introduction

Lane detection is a crucial aspect of autonomous driving systems, enabling vehicles to understand their environment and navigate safely. This project leverages the CARLA simulation environment and a semantic segmentation algorithm based on UNet to detect left and right lanes in a virtual driving scenario.

## Features

- **Semantic Segmentation**: Utilizes a UNet-based neural network for lane detection.
- **CARLA Integration**: Integrates with the CARLA simulator for training, validation, and real-time testing.
- **Real-time Processing**: Capable of making lane detection predictions in near real-time.

## Installation

1. **CARLA Setup**: Follow the [CARLA installation guide](https://carla.readthedocs.io/en/latest/start_quickstart/) to set up the CARLA simulator.
2. **Dependencies**: Install the required Python dependencies listed in `requirements.txt` using pip:
    ```
    pip install -r requirements.txt
    ```

## Methodology

This project follows a two-stage methodology: data collection and model training, followed by model deployment. Raw camera images and label images are collected within the CARLA simulation environment, which are then used to train a UNet-based neural network. The trained model is subsequently deployed for real-time lane detection.

## Results

The trained model demonstrates promising results in the simulation environment, achieving low loss and high Mean IoU metrics during training. However, there are observed false positives and false negatives in real-time predictions, indicating room for improvement. Further data augmentation, fine-tuning with real-world data, and enhancements to the simulation environment are suggested for future iterations.

## Future Work

- Expand the dataset: Gather more diverse data to improve model generalization.
- Data augmentation: Apply augmentation techniques to increase dataset variability.
- Fine-tuning: Adapt the model with real-world data to enhance performance in real-world scenarios.
- Simulation enhancement: Improve simulation realism to better align with real-world conditions.

## Acknowledgements

- Special thanks to the CARLA development team for providing a powerful simulation platform.
- This project is based on the [course](https://thomasfermi.github.io/Algorithms-for-Automated-Driving/LaneDetection/LaneDetectionOverview.html) by Thomas Fermi. Thanks a lot!
