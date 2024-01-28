# HDD dataset
This repository provides the HDD dataset used in the evaluation for the method proposed in the paper entitled "[Consistent pretext and auxiliary tasks with relative remaining useful life estimation](https://ieeexplore.ieee.org/document/10415283)." The original data is provided by [Backblaze, inc.](https://www.backblaze.com/cloud-storage/resources/hard-drive-test-data) Please check out the web page for the license. You are solely responsible for how you use the data in the repository.

# Data processing
1. Open create_backblaze_HDD_semisupervised_10pattern_label_4.ipynb
2. Run the notebook.

# Processed data
The preprocessed data is located in './backblaze_HDD'. The directory includes 10 directories for training data and a directory for testing data. Each of the directories for training includes datasets with different labeled data and unlabeled data. The labeled data is located in the directory whose name is 'supervised'. The unlabeled data is located in the directory whose name is 'unsupervised'. The directories include CSV files, each of which is either run-to-failure data or run-to-maintenance data. The directory whose name is 'testing' includes testing data. The file, 'RUL_test_backblazeHDD.txt' records RUL at the end of the corresponding multivariate time series. The multivariate time series are in 'test_backblazeHDD'. The file names are corresponding to the row numbers of 'RUL_test_backblazeHDD.txt'. The detailed processing steps can be found in create_backblaze_HDD_semisupervised_10pattern_label_4.ipynb.
