# Indoor Air Quality Predicitons And Monitoring Project

Indoor air quality directly affects the quality of life for everyone. The most advanced systems for monitoring air quality rely on automation, which processes data in real-time and responds accordingly. However, these systems also have potential issues that can negatively impact the user experience:

- Incorrect data readings due to sensor malfunctions,

- The system's inability to adapt to short-term changes in user preferences,

- Lack of foresight in case of potential disasters.

In this study, I aim to improve the predictability of automation systems by using deep neural networks to forecast future behaviors. By doing so, we expect to address some of these problems and make the system more adaptable and foresightful.

## CN-OBEE Dataset

The CN-OBEE dataset encompasses one year of data from a Chinese household. This dataset includes data that affect the air quality of six different rooms. Additionally, it provides access to weather information outside the house. Moreover, the power file contains data on the energy consumption of electrical appliances used within the household.

## Indoor Air Quality Predictor
The `Air_Quality_Prediction.ipynb` file utilizes an RNN named GRU and LSTM to generate 44 days of prediction data using this information. These prediction data cover temperature, pressure, and relative humidity. Prediction data are stored in the `predictions.csv` file.

## SmartAir Controller
The `Smart-Air.py` file is a web application written with **Streamlit**. This application allows users to view prediction data and provides information on when the automation system will operate. Furthermore, users can suspend or schedule the system's future operations before they occur if desired.

<p align="center">
  <img src="1.png" alt="Image 1" width="800"/>
  <img src="2.png" alt="Image 2" width="800"/>
</p>

## Contents
`demo.pdf`: This file provides a demonstration of how the Air-Smart-Controller works.

`Air-Smart-Controller-Report.pdf`: This document offers a detailed analysis of the literature and provides in-depth information about the project.

## Usage
To use the Air-Smart-Controller project, follow these steps:

- Clone the repository to your local machine.
- Refer to the demo.pdf for a demonstration of the project's functionality.
- For a deeper understanding of the project and its background, consult the Air-Smart-Controller-Report.pdf and Air-Smart-Controller-Paper.pdf.
- Explore the codebase to view implementation details and make any necessary modifications.
