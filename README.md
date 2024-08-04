# DeepSand-Bulldozer
The main idea of the DeepSand project is the development of an autonomous bulldozer robot capable of grading sand terrain using advanced deep learning techniques. 
# Deepsand: Autonomous Bulldozer Robot

The Deepsand project addresses the challenge of manipulating a continuously deformable environment like sand, which has significant implications for construction, agriculture, and planetary exploration. The ability to autonomously grade and shape sand can lead to advancements in earth-moving machinery, autonomous farming equipment, and robotic systems for extraterrestrial terrain navigation, improving efficiency, accuracy, and safety in these fields.

## Novelty

The novelty in this research lies in its approach to dealing with the complexities of sand interaction. Unlike general Sim2Real problems, modeling sand interaction is highly difficult and computationally expensive. This research proposes innovative techniques to solve the problem effectively.

## Approaches

1. **Traditional Reinforcement Learning (RL):**
   - Utilize reward calculations based on point cloud loss functions like Chamfer distance loss and Earth mover’s distance.

2. **Learning World Model and Formulate as Online RL:**
   - Reference: [Daydreamer](https://arxiv.org/abs/2005.04126)

3. **Predict Robot-Sand Interaction Behavior using Generative Models like GAN:**
   - Reference: [Deep-sand scape](https://arxiv.org/abs/1805.11014)

## Current Implementation

### Data Collection and Localization

- Mapped joystick inputs and developed localization scripts using AprilTag and overhead camera data, enabling manual control and precise localization of the autonomous bulldozer robot.
- Engineered a comprehensive dataset collection system, capturing RGB images, point cloud data, and robot commands, with synchronization through ROS Bag and CSV for post-processing and analysis.

### Initial Model

- Implemented a simple classification model using only RGB images.

### Advanced Model

- Implemented a CNN + LSTM model using PointNet and ResNet-18 to process multimodal data, improving the robot's ability to autonomously identify and fill holes in the terrain.

### Enhanced Techniques

- Progressed to using Action Chunking with Transformers (ACT) techniques, inspired by the paper ['Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware'](https://arxiv.org/abs/2008.06038), to enhance task precision and efficiency in the robot's terrain manipulation tasks.

## Future Work

The research aims to further explore and refine these techniques to improve the robot's capabilities in manipulating sand and similar deformable environments. By leveraging advanced deep learning models and reinforcement learning strategies, the project seeks to achieve higher levels of autonomy and precision in robotic earth-moving tasks.

![Environment Setup](https://github.com/anarbhagat/DeepSand-Bulldozer/blob/main/IMG_20240729_142707330%20(1).jpg?raw=true)

## Contact

For more information, please contact:
- Anar Raghinkumar Bhagat
- Email: [ab11262@nyu.edu](mailto:ab11262@nyu.edu)
- LinkedIn: [Anar Bhagat](https://www.linkedin.com/in/anarbhagat)
