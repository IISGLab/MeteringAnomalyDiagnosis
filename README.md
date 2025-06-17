# Metering Anomaly Diagnosis(MAD)
Metering Anomaly Diagnosis (MAD) is a metering anomaly diagnosis dataset for smart meters in smart grid substation, which is used to support multivariate time series classification research.

## Introduction of MAD
These data are all from the actual deployment of Advanced Metering Infrastructure (AMI) system, which has a high engineering application representative. The dataset contains 504 three-phase four-wire smart electricity meters, of which 382 are normal meters and 122 are meters with various types of abnormalities that were manually inspected on site or marked by professionals.
The sampling interval of the data was 30 minutes. Because we split the samples on a daily basis, each sample contains 48 data points.

The data set has been preprocessed, resulting in 7421 usable samples, which are stored in the MAD.npz file. The training and test sets have been split into 2319 and 5414 samples, respectively, which can be extracted from (x_train, y_train, x_test, y_test).

The samples of the dataset contain 7 categories, 0 is normal, and 1 to 6 are abnormal types. The specific sample distribution is shown in the table below:

| Category ID | Description | number of samples |
| ---- | ---- | ---- |
| 0 | normal | 6212 |
| 1 | Exception -1 | 196 |
| 2 | Anomaly -2 | 85 |
| 3 | Anomaly -3 | 88 |
| 4 | Abnormal -4 | 525 |
| 5 | Anomaly -5 | 81 |
| 6 | Exception -6 | 234 |

---
## Introduction of sample
All data were collected from three-phase four-wire smart electricity meters, and each sample contained 14 variables, which were 3-phase voltage, 3-phase current, total active power and 3-phase active power, and total power factor and 3-phase power factor. Each variable has been normalized, and the samples of normal and six abnormal cases are as follows:

<p align="center">
<img src="./imgs/normal.png" height = "500" alt="" align=center />
<br><br>
<b>Figure 1.</b> Normal Smaple
</p>

<p align="center">
<img src="./imgs/abnormal-1.png" height = "500" alt="" align=center />
<br><br>
<b>Figure 2.</b>  Abnormal-1
</p>

<p align="center">
<img src="./imgs/abnormal-2.png" height = "500" alt="" align=center />
<br><br>
<b>Figure 3.</b>  Abnormal-2
</p>

<p align="center">
<img src="./imgs/abnormal-3.png" height = "500" alt="" align=center />
<br><br>
<b>Figure 4.</b>  Abnormal-3
</p>

<p align="center">
<img src="./imgs/abnormal-4.png" height = "500" alt="" align=center />
<br><br>
<b>Figure 5.</b>  Abnormal-4
</p>

<p align="center">
<img src="./imgs/abnormal-5.png" height = "500" alt="" align=center />
<br><br>
<b>Figure 6.</b>  Abnormal-5
</p>

<p align="center">
<img src="./imgs/abnormal-6.png" height = "500" alt="" align=center />
<br><br>
<b>Figure 7.</b>  Abnormal-6
</p>

---
If you use this dataset please cite the work:

```
@misc{MAD,
  author       = {Wang, F.},
  title        = {{Metering Anomaly Diagnosis}},
  year         = {2025},
  note         = {https://github.com/IISGLab/MeteringAnomalyDiagnosis} 
}
```
