## Overview

This README provides details about the sample data file `untitledDLC_resnet50_sniff_helmet4Jun20shuffle1_75000.csv`, which contains tracking data produced by the DeepLabCut (DLC) model `DLC_resnet50_sniff_helmet4Jun20shuffle1_75000`.

## Data Description

The data file contains information about the coordinates and likelihood of the detected body parts in a series of frames. Below is a description of each column in the dataset:

- **scorer:** The model used to generate the data (`DLC_resnet50_sniff_helmet4Jun20shuffle1_75000`).
- **bodyparts:** The specific body parts being tracked:
  - Nose
  - L_Eye
  - R_Eye
  - L_Ear
  - R_Ear
  - Throat
  - Withers
  - TailSet
  - L_F_Paw
  - R_F_Paw
  - L_F_Wrist
  - R_F_Wrist
  - L_F_Elbow
  - R_F_Elbow
  - L_B_Paw
  - R_B_Paw
  - L_B_Hock
  - R_B_Hock
  - L_B_Stiffle
  - R_B_Stiffle
- **coords:** The type of data being recorded (`x`, `y`, `likelihood`).

### Columns

1. **scorer**: The model used to produce the data.
2. **bodyparts**: The specific body parts being tracked.
3. **coords**: The type of data recorded for each frame.
    - `x`: The x-coordinate of the detected body part.
    - `y`: The y-coordinate of the detected body part.
    - `likelihood`: The likelihood of the detection being correct.

### Sample Data

| scorer                                      | bodyparts | coords     | 0                | 1                |
|---------------------------------------------|-----------|------------|------------------|------------------|
| DLC_resnet50_sniff_helmet4Jun20shuffle1_75000 | Nose      | x          | 820.226867675781 | 345.133819580078 |
| DLC_resnet50_sniff_helmet4Jun20shuffle1_75000 | Nose      | y          | 610.618286132813 | 55.7734107971191 |
| DLC_resnet50_sniff_helmet4Jun20shuffle1_75000 | Nose      | likelihood | 0.0242341384291649 | 0.146951898932457 |

## File Format

The data is stored in a CSV file format, which can be opened using any standard text editor or spreadsheet software such as Microsoft Excel or Google Sheets.

## Usage

This data can be used for analyzing the movement and behavior of the tracked body parts in the recorded frames. It can be imported into various data analysis tools for further processing and visualization.

### Additional Files

- `acc_all_june20th.csv`: Contains data on the acceleration of the same body parts.
- `velocity_all_june20th.csv`: Contains data on the velocity of the same body parts.

EEG Data Sample
Overview
This document provides an overview and description of the EEG data collected in the sample dataset. The dataset includes timestamps, EEG measurements from various electrodes, trial markers indicating different trial states, and additional sensor data including accelerometer, gyroscope, and magnetometer readings.

Data Description
EEG Data
Columns
The EEG dataset contains the following columns:

Timestamp: The time at which the EEG data was recorded.
Fz: EEG data from the Fz electrode.
Cz: EEG data from the Cz electrode.
T3: EEG data from the T3 electrode.
T4: EEG data from the T4 electrode.
P3: EEG data from the P3 electrode.
P4: EEG data from the P4 electrode.
Fp1: EEG data from the Fp1 electrode.
Fp2: EEG data from the Fp2 electrode.
trial_marker: Indicates the trial state. The values in this column can be:
0: No sniff
1: Sniffed control
2: Sniffed target
Sample Data
Timestamp	Fz	Cz	T3	T4	P3	P4	Fp1	Fp2	trial_marker
257312.878	17237.810547	9872.769531	1205.250000	-2459.570068	287.820007	-3004.889893	-2013.020020	-3410.820068	0
257312.879	17254.500000	9836.480469	1177.219971	-2479.510010	265.739990	-3022.479980	-2048.830078	-3447.290039	0
257312.880	17267.369141	9811.209961	1164.869995	-2496.000000	241.089996	-3042.510010	-2071.090088	-3471.800049	0
257312.881	17277.529297	9795.240234	1155.189941	-2505.300049	223.919998	-3057.379883	-2084.300049	-3478.580078	0
257312.882	17288.830078	9780.549805	1147.219971	-2514.459961	213.669998	-3074.739990	-2084.449951	-3493.070068	0
Sensor Data
Columns
The sensor dataset contains the following columns:

Timestamp: The time at which the sensor data was recorded.
Ax: Accelerometer data along the x-axis.
Ay: Accelerometer data along the y-axis.
Az: Accelerometer data along the z-axis.
Gx: Gyroscope data along the x-axis.
Gy: Gyroscope data along the y-axis.
Gz: Gyroscope data along the z-axis.
Mx: Magnetometer data along the x-axis.
My: Magnetometer data along the y-axis.
Mz: Magnetometer data along the z-axis.
Sample Data
Timestamp	Ax	Ay	Az	Gx	Gy	Gz	Mx	My	Mz
257312.958586	129.503006	-524.661011	-652.151001	-58931.25	16563.75	89853.75	287.279999	-218.880005	252.320007
257312.983614	28.792000	-481.106995	-620.552979	-62728.75	22758.75	111545.00	253.839996	-264.480011	243.199997
257313.022463	-6.710000	-361.973999	-643.732971	-32182.50	9336.25	125177.50	247.759995	-300.959991	237.119995
257313.076736	-161.893997	-396.683014	-715.591003	-6440.00	38788.75	133770.00	208.240005	-354.160004	221.919998
257313.100406	3.294000	-381.372009	-706.502014	-6545.00	35306.25	94097.50	158.080002	-398.239990	255.360001
Usage
This dataset can be used to analyze the EEG responses during different trial states as well as to study movement and orientation data recorded simultaneously. The trial_marker column provides context for the EEG readings, indicating whether the subject was not sniffing (0), sniffing a control (1), or sniffing a target (2).

Notes
All timestamps are rounded to three decimal places.
EEG data is provided for eight electrodes: Fz, Cz, T3, T4, P3, P4, Fp1, and Fp2.
Sensor data includes accelerometer, gyroscope, and magnetometer readings.
The trial markers are essential for distinguishing between different trial conditions and should be used accordingly in any analysis.
