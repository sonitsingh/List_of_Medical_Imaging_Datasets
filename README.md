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
|-------------------|-------|-------|-------|
|No. of Images      | 78467 | 22432 | 11218 |
---------------------------------------------

|                   |[1]    |[1]    |[2]    |[3]      |[4]   |[7]   |[8]    |[9]    |[10]   |
|-------------------|-------|------ |-------|---------|------|------|------ |------ |------ |
|SPLIT BY           |patient|image  |image  |patient  |image |image |image  |patient|patient| 
|OFFICIAL SPLIT     |Yes    |No     |No     |No       |No    |No    |No     |Yes    |Yes    |
|Atelectasis        |0.7003 |0.72   |0.81   |0.772    |0.80  |0.76  |0.853  |0.767  |0.733  |
|Cardiomegaly       |0.8100 |0.81   |0.904  |0.9248   |0.81  |0.91  |0.939  |0.883  |0.858  |
|Effusion           |0.7585 |0.78   |0.859  |0.8638   |0.87  |0.86  |0.903  |0.828  |0.806  |
|Infiltration       |0.6614 |0.61   |0.695  |0.7345   |0.70  |0.69  |0.754  |0.709  |0.675  |
|Mass               |0.6933 |0.71   |0.792  |0.8676   |0.83  |0.78  |0.902  |0.821  |0.727  |
|Nodule             |0.6687 |0.67   |0.717  |0.7802   |0.75  |0.70  |0.828  |0.758  |0.778  |
|Pneumonia          |0.6580 |0.63   |0.713  |0.7680   |0.67  |0.71  |0.774  |0.731  |0.690  |
|Pneumothorax       |0.7993 |0.81   |0.841  |0.8887   |0.87  |0.86  |0.921  |0.846  |0.805  |
|Consolidation      |0.7032 |0.71   |0.788  |0.7901   |0.80  |0.78  |0.842  |0.745  |0.717  |
|Edema              |0.8052 |0.83   |0.882  |0.8878   |0.88  |0.89  |0.924  |0.835  |0.806  |
|Emphysema          |0.8330 |0.81   |0.829  |0.9371   |0.91  |0.90  |0.932  |0.895  |0.842  |
|Fibrosis           |0.7859 |0.77   |0.767  |0.8047   |0.78  |0.76  |0.864  |0.818  |0.757  |
|Pleural Thickening |0.6835 |0.71   |0.765  |0.8062   |0.79  |0.77  |0.837  |0.761  |0.724  |
|Hernia             |0.8717 |0.77   |0.914  |0.9164   |0.77  |0.90  |0.921  |0.896  |0.824  |


