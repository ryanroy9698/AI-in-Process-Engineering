## Dataset Overview

The dataset comprises 36,733 instances, consisting of 11 sensor measures aggregated over one hour from a gas turbine plant in Turkey. The primary focus is on the study of flue gas emissions, specifically Carbon Monoxide (CO) and Nitrogen Oxides/derivatives (NOx).

### Objectives

Develop a multivariate regression model to predict CO and NOx emissions using sensor measures as features. The dataset includes gas turbine parameters and ambient variables. The goal is to leverage this information for accurate Turbine Energy Yield (TEY) prediction.

### Dataset Characteristics

- **Number of Instances:** 36,733

### Feature Units and Statistics

The 11 features in the dataset are as follows:

| Variable                       | Abbreviation | Unit    | Min     | Max     | Mean    |
|--------------------------------|--------------|---------|---------|---------|---------|
| Ambient temperature            | AT           | degree C| -6.23   | 37.10   | 17.71   |
| Ambient pressure               | AP           | mbar    | 985.85  | 1036.56 | 1013.07 |
| Ambient humidity               | AH           | %       | 24.08   | 100.20  | 77.87   |
| Air filter difference pressure | AFDP         | mbar    | 2.09    | 7.61    | 3.93    |
| Gas turbine exhaust pressure   | GTEP         | mbar    | 17.70   | 40.72   | 25.56   |
| Turbine inlet temperature      | TIT          | C       | 1000.85 | 1100.89 | 1081.43 |
| Turbine after temperature      | TAT          | C       | 511.04  | 550.61  | 546.16  |
| Compressor discharge pressure  | CDP          | mbar    | 9.85    | 15.16   | 12.06   |
| Turbine energy yield           | TEY          | MWH     | 100.02  | 179.50  | 133.51  |
| Carbon monoxide                | CO           | mg/m3   | 0.00    | 44.10   | 2.37    |
| Nitrogen oxides                | NOx          | mg/m3   | 25.90   | 119.91  | 65.29   |

**IMPORTANT NOTE:** AFDP and GTEP are assumed to be in bar, not millibar. This assumption is made based on typical operating pressures of equipment, which are usually higher than ambient pressure.

### Data Range

The dataset covers the time period from 01-01-2011 to 31-12-2015.

### Model Development

**Objective:** Predict CO and NOx emissions.
**Features:** Utilize gas turbine parameters and ambient variables.

### Potential Limitations Involved with the Dataset

- **No Time Stamp:** The dataset lacks a column indicating the time stamp of the readings. However, it's mentioned that instances were taken every 1 hour, the data points are sorted chronologically, and the plant was fully operational throughout the specified date range.
