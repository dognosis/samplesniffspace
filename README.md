## Overview

This README provides details about the sample data file `untitledDLC_resnet50_sniff_helmet4Jun20shuffle1_75000.csv`, which contains tracking data produced by the DeepLabCut (DLC) model `DLC_resnet50_sniff_helmet4Jun20shuffle1_75000`.

## Data Description

The data file contains information about the coordinates and likelihood of the detected body part (Nose) in a series of frames. Below is a description of each column in the dataset:

- **scorer:** The model used to generate the data (`DLC_resnet50_sniff_helmet4Jun20shuffle1_75000`).
- **bodyparts:** The specific body part being tracked (`Nose`).
- **coords:** The type of data being recorded (`x`, `y`, `likelihood`).

### Columns

1. **scorer**: The model used to produce the data.
2. **bodyparts**: The specific body part being tracked.
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

This data can be used for analyzing the movement and behavior of the tracked body part (Nose) in the recorded frames. It can be imported into various data analysis tools for further processing and visualization.

### Additional Files

- `acc_all_june20th.csv`: Contains data on the acceleration of the same body part.
- `velocity_all_june20th.csv`: Contains data on the velocity of the same body part.

### Configuration File

The `config.yaml` file, located at `/home/ashie/DeepLabCut/project_directory/sniff_helmet4-aswin-2024-06-20/config.yaml`, contains the following content:

```yaml
    # Project definitions (do not edit)
Task: sniff_helmet4
scorer: aswin
date: Jun20
multianimalproject: false
identity:

    # Project path (change when moving around)
project_path: /home/ashie/DeepLabCut/project_directory/sniff_helmet4-aswin-2024-06-20

    # Annotation data set configuration (and individual video cropping parameters)
video_sets:
  /home/ashie/DeepLabCut/project_directory/sniff_helmet4-aswin-2024-06-20/videos/untitled.mp4:
    crop: 0, 1920, 0, 1080
bodyparts:
- Nose
- L_Eye
- R_Eye
- L_Ear
- R_Ear
- Throat
- With
update it as for all bodyparts(20) as for exaplme nose is only mentioned here
ChatGPT
Here's the updated README content that includes the detailed information about all 20 body parts as listed in the config.yaml:

python
Copy code
# Create the README content
readme_content = """
# Sample Data README

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
