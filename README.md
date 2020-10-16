# Detection of abnormal activity using a wearable biosensor

## Background
In the last few decades, the miniaturization of wearable sensors and improvement of data transmission technologies allowed for collecting medically relevant data called digital biomarkers. This data is revolutionising our modern Medicine by offering new perspectives to better understand human physiology and develop personalized medicine. Therefore, new methods for digital biomarker data analysis, leveraging the power of Artificial Intelligence, are needed to characterise health status, detect disease progression steps or consolidate medical diagnostics.

In this project, we will use a publicly available dataset for wearable stress and affect detection (WESAD). 17 participants were submitted to a study protocol designed to elicit three different affective states (neutral, stress, amusement), while wearing two devices collecting physiological data (chest-worn and wrist-worn device). In order to validate the study protocol, each participant filled self-reports to characterise their stress status, that could be used as Ground Truth data.

## Project Goals:

The first goal of this project is to integrate the sensor data into one or several outcome measures, which meaningfully recapitulate the stress status of the subject. The second challenge would be to provide an analysis method allowing for the earliest (using the minimal amount of data) and most reliable detection of change in stress status.


## Milestones:

 Milestones 1: Structure and normalize the data. Identify patterns and characterise stress-related status.
 Milestones 2: Detect early change in stress data. Demonstrate the trade-off between early and reliable detection methods.


## Data:

Please find below a brief description from the [WESAD repository webpage](https://archive.ics.uci.edu/ml/datasets/WESAD+%28Wearable+Stress+and+Affect+Detection%29):

* Raw sensor data was recorded with two devices: a chest-worn device (RespiBAN) and a wrist-worn device (Empatica E4).
* The RespiBAN device provides the following sensor data: electrocardiogram (ECG), electrodermal activity (EDA), electromyogram (EMG), respiration, body temperature, and three-axis acceleration. All signals are sampled at 700 Hz.
* The Empatica E4 device provides the following sensor data: blood volume pulse (BVP, 64 Hz), electrodermal activity (EDA, 4 Hz), body temperature (4 Hz), and three-axis acceleration (32 Hz).

The [dataset's readme-file](wesad_readme.pdf) contains all further details with respect to the dataset structure, data format (RespiBAN device, Empatica E4 device, synchronised data), study protocol, and the self-report questionnaires.

## Approach
**Skills**: Time-series analysis of data.

**Output**: Analysis report of activity. Dashboard for a patient-specific overview

**Value Proposition**: Tells the medical staff any stress-related physiological change.

**Integration**: Dashboard accessible through a web interface to be developed on Streamlit

**Customers**: Medical staff

**Cost**: Written acknowldegement.

**Revenue**: Stress detection may lower medical cost by enabling early detection of stress-related health issues. 

### Code structure

**`1_exploration`**: first handling of the data. Plotting time-series to find the relevant duration and amplitude of patterns. Data interpretation on a few examples.

**`2_forecasting`**: Anomaly detection using time-series forecasting using Prophet from facebook

**`3_dashboard`**:  Web interface dedicated to the caregivers to inform and alert on the patient activities.

Reference
Philip Schmidt, Attila Reiss, Robert Duerichen, Claus Marberger and Kristof Van Laerhoven. 2018. Introducing WESAD, a multimodal dataset for Wearable Stress and Affect Detection. In 2018 International Conference on Multimodal Interaction (ICMI ’18), October 16–20, 2018, Boulder, CO, USA. ACM, New York, NY, USA, 9 pages. https://doi.org/10.1145/3242969.3242985

> Questions:
> Contact Guillaume Azarias at guillaume.azarias@hotmail.com
