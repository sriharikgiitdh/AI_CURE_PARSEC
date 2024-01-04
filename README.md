# AI Cure - PARSEC 4.0


## Task
The goal is to construct an advanced model capable of accurately predicting an individual's heart rate.The dataset encompasses diverse attributes derived from signals measured through ECG recordings for various individuals, each exhibiting different heart rates at the respective time of measurement. These features collectively contribute to determining the heart rate at the specific moment for each individual.

## File Descriptions

The dataset is provided in `train_data.csv`.  

## Data Dictionary

Following is the data dictionary for the features you will come across in the files mentioned:

- `MEAN_RR`: Mean of RR intervals
- `MEDIAN_RR`: Median of RR intervals
- `SDRR`: Standard deviation of RR intervals
- `RMSSD`: Root mean square of successive RR interval differences
- `SDSD`: Standard deviation of successive RR interval differences
- `SDRR_RMSSD`: Ratio of SDRR / RMSSD
- `pNN25`: Percentage of successive RR intervals that differ by more than 25 ms
- `pNN50`: Percentage of successive RR intervals that differ by more than 50 ms
- `KURT`: Kurtosis of distribution of successive RR intervals
- `SKEW`: Skew of distribution of successive RR intervals
- `MEAN_REL_RR`: Mean of relative RR intervals
- `MEDIAN_REL_RR`: Median of relative RR intervals
- `SDRR_REL_RR`: Standard deviation of relative RR intervals
- `RMSSD_REL_RR`: Root mean square of successive relative RR interval differences
- `SDSD_REL_RR`: Standard deviation of successive relative RR interval differences
- `SDRR_RMSSD_REL_RR`: Ratio of SDRR/RMSSD for relative RR interval differences
- `KURT_REL_RR`: Kurtosis of distribution of relative RR intervals
- `SKEW_REL_RR`: Skewness of distribution of relative RR intervals
- `uuid`: Unique ID for each patient
- `VLF`: Absolute power of the very low frequency band (0.0033 - 0.04 Hz)
- `VLF_PCT`: Principal component transform of VLF
- `LF`: Absolute power of the low-frequency band (0.04 - 0.15 Hz)
- `LF_PCT`: Principal component transform of LF
- `LF_NU`: Absolute power of the low-frequency band in normal units
- `HF`: Absolute power of the high-frequency band (0.15 - 0.4 Hz)
- `HF_PCT`: Principal component transform of HF
- `HF_NU`: Absolute power of the highest frequency band in normal units
- `TP`: Total power of RR intervals
- `LF_HF`: Ratio of LF to HF
- `HF_LF`: Ratio of HF to LF
- `SD1`: Poincaré plot standard deviation perpendicular to the line of identity
- `SD2`: Poincaré plot standard deviation along the line of identity
- `Sampen`: Sample entropy which measures the regularity and complexity of a time series
- `higuci`: Higuci fractal dimension of heart rate
- `datasetId`: ID of the whole dataset
- `condition`: Condition of the patient at the time the data was recorded
- `HR`: Heart rate of the patient at the time of data recorded

## Submission Details
In addition to the Jupyter notebook containing your experiments, you are required to provide a file named `run.py`. This script should utilize your final model and accept the input file `test_data.csv` as a command line argument. The output of the script should be a file named `results.csv` that contains the predicted Heart Rate values.

Evaluation of submissions will be based on a separate set of test data that is not disclosed to participants. For reference, a sample test data file named `sample_test_data.csv` and the expected output file `sample_output_generated.csv` are provided.
