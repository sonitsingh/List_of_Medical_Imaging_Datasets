# List_of_Medical_Imaging_Datasets
Partial list of medical imaging datasets

I am maintaining this repo to have list of various datasets on which I aim to work in a single listing. By all means, this is not complete and I do not frequently update this list.

# MEDICAL VISION DATASETS

## ChestX-ray14 Dataset from National Institute of Health (NIH)

Please read the following paper for details:

[1] [ChestX-ray8: Hospital-scale Chest X-ray Database and Benchmarks on Weakly-Supervised Classification and Localization of Common Thorax Diseases](https://arxiv.org/abs/1705.02315)

1. Contains 112,120 frontal-view Chest X-rays of 32,717 unique patients.
2. All images have a resolution of 1024 * 1024 with 8 bits of gray scale.
3. Classsified into 14 diseases namely, Atelectasis, Cardiomegaly, Effusion, Infiltration, Mass, Nodule, Pneumonia, Pneumothorax, Consolidation, Edema, Emphysema, Fibrosis, Pleural Thickening, and Hernia.
4. These labels are not manaully curated, instead NLP based labeler is applied to get these labels from radiology reports.
5. Split by image: The dataset has been split into train, valid and test consisting of 70%, 20%, and 10% of total dataset.
6. Split by patient: The official split by patient is also available [here](https://nihcc.app.box.com/v/ChestXray-NIHCC)
7. The official splits, either by images or by patients ensures no patient overlap in the train and test sets.
8. Number of images per class is given below.

|    Disease        | Train | Test  | Valid |
|-------------------|-------|------ |-------|
|Atelectasis        | 7996  | 2420  | 1119  |
|Cardiomegaly       | 1950  | 582   | 240   |
|Effusion           | 9261  | 2754  | 1292  |
|Infiltration       | 13914 | 3938  | 2018  |
|Mass               | 3988  | 1133  | 625   |
|Nodule             | 4375  | 1335  | 613   |
|Pneumonia          | 978   | 242   | 133   |
|Pneumothorax       | 3705  | 1089  | 504   |
|Consolidation      | 3263  | 957   | 447   |
|Edema              | 1690  | 413   | 200   |
|Emphysema          | 1799  | 509   | 208   |
|Fibrosis           | 1158  | 362   | 166   |
|Hernia             | 144   | 42    |  41   |
|No Findings        | 42404 | 11927 | 6078  |
|**No. of Images**  |**78467**| **22432** | **11218** |

## MIMIC-CXR Dataset

Please read the following paper for more details:

[2] [MIMIC-CXR: A Large publicly available database of labeled Chest Radiographs](https://arxiv.org/pdf/1901.07042.pdf)

1. A large dataset of 371,920 chest X-rays associated with 227,943 imaging studies sourced from the Beth Israel Deaconess Medical Centre between 2011-2016.
2. Each imaging study is most often associated with two images: a frontal view and a lateral view.
3. Images are provided with 14 thoracic disease labels derived by applying NLP tool to corresponding radiology reports.
4. The dataset is de-identified to satisfy the US HIPAA requirements.
5. The pathology labels significantly overlap with those of the NIH ChestX-ray14 dataset.
6. Each chest radiograph was sourced from hospitals' PACS in DICOM format. After de-identification, images were exported in the JPEG standard format having pixel data normalized to the unit interval, and the bit-depth scaled to 8-bit (0-255).
7. Although there are different section in a radiology report such as *comparison*, *Indication*, *findings*, and *impression*, labels for the images are derived from either the *impression* section or the *finding* section if impression is not present. 
8. Of the total 227,943 reports, 82.4% have an impression section, 12.5% have findings sections, and 5.1% do not have an impression or findings section.
9. Labels are determined using the open source CheXpert labeler developed at the Stanford University.
10. CheXpert is a rule based classifier having three stages: 1. extraction, 2. classification, and 3. aggregation. 
11. The curated dataset is publicly available on PhysioNet and is free to all researchers after signing a data use agreement. 
12. In future, authors plan to release the original DICOM files with free-text radiology reports.

### Task List
- [x] NIH ChesX-ray14 Dataset
- [ ] MIMIC-CXR Dataset
- [ ] Chexpert Dataset
- [ ] Indiana University Chest X-ray collection
- [ ] PadChest Dataset
- [ ] Need to finish portfolio 1
