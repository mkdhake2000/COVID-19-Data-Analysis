# **Assignment Details:**

## **Plugins:**
- **Software:** Python3 Jupyter Notebook (.sh files run Python3 Jupyter Notebooks)
- **Environments:** Python 3.7.3

## **Dependencies:**
- **Python Libraries:**
  - Pandas v1.3.2
  - Collections
  - Numpy v1.20.2
  - Json 2.0.9
  - Datetime
  - Math
  - Matplotlib.pyplot (Matplotlib v3.4.3)
  - Openpyxl (for reading Excel file of census data)

## **Programs:**
### **.sh Files:**
- `assign1.sh`: Top-level script that runs the entire assignment
- `neighbor-districts-modifier.sh`: Runs `Q1.ipynb` using the command: `jupyter nbconvert --to notebook --execute Q1.ipynb`
- `edge-generator.sh`: Runs `Q2.ipynb` using the command: `jupyter nbconvert --to notebook --execute Q2.ipynb`
- `case-generator.sh`: Runs `Q3.ipynb` using the command: `jupyter nbconvert --to notebook --execute Q3.ipynb`
- `peaks-generator.sh`: Runs `Q4.ipynb` using the command: `jupyter nbconvert --to notebook --execute Q4.ipynb`
- `vaccinated-count-generator.sh`: Runs `Q5_Asgn1.ipynb` using the command: `jupyter nbconvert --to notebook --execute Q5.ipynb`
- `vaccination-population-ratio-generator.sh`: Runs `Q6.ipynb` using the command: `jupyter nbconvert --to notebook --execute Q6.ipynb`
- `vaccine-type-ratio-generator.sh`: Runs `Q7.ipynb` using the command: `jupyter nbconvert --to notebook --execute Q7.ipynb`
- `vaccinated-ratio-generator.sh`: Runs `Q8.ipynb` using the command: `jupyter nbconvert --to notebook --execute Q8.ipynb`
- `complete-vaccination-generator.sh`: Runs `Q9.ipynb` using the command: `jupyter nbconvert --to notebook --execute Q9.ipynb`

### **Jupyter Notebook Files:**
- **Q1.ipynb**
  - **Input:** neighbor-districts.json, cowin_vaccine_data_districtwise.csv
  - **Output:** neighbor-districts-modified.json

- **Q2.ipynb**
  - **Input:** neighbor-districts-modified.json
  - **Output:** edge-graph.csv

- **Q3.ipynb**
  - **Input:** neighbor-districts-modified.json, districts.csv
  - **Output:** cases-week.csv, cases-month.csv, cases-overall.csv

- **Q4.ipynb**
  - **Input:** neighbor-districts-modified.json, districts.csv, cowin_vaccine_data_districtwise.csv
  - **Output:** district-peaks.csv, state-peaks.csv, overall-peaks.csv

- **Q5_Asgn1.ipynb**
  - **Input:** neighbor-districts-modified.json, cowin_vaccine_data_districtwise.csv
  - **Output:** district-vaccinated-count-week.csv, district-vaccinated-count-month.csv,
	district-vaccinated-count-overall.csv, state-vaccinated-count-week.csv, 
	state-vaccinated-count-month.csv, state-vaccinated-count-overall.csv

- **Q6.ipynb**
  - **Input:** neighbor-districts-modified.json, cowin_vaccine_data_districtwise.csv,
	DDW_PCA0000_2011_Indiastatedist.xlsx
  - **Output:** district-vaccination-population-ratio.csv, state-vaccination-population-ratio.csv,
	overall-vaccination-population-ratio.csv

- **Q7.ipynb**
  - **Input:** neighbor-districts-modified.json, cowin_vaccine_data_districtwise.csv,
	DDW_PCA0000_2011_Indiastatedist.xlsx
  - **Output:** district-vaccine-type-ratio.csv, state-vaccine-type-ratio.csv,
	overall-vaccine-type-ratio.csv

- **Q8.ipynb**
  - **Input:** neighbor-districts-modified.json, cowin_vaccine_data_districtwise.csv,
	DDW_PCA0000_2011_Indiastatedist.xlsx
  - **Output:** district-vaccinated-dose-ratio.csv, state-vaccinated-dose-ratio.csv,
	overall-vaccine-type-ratio.csv

- **Q9.ipynb**
  - **Input:** neighbor-districts-modified.json, cowin_vaccine_data_districtwise.csv,
	DDW_PCA0000_2011_Indiastatedist.xlsx
  - **Output:** complete-vaccination.csv

## **How to Use:**
In order to run all programs sequentially, run the following command from the terminal:
```bash
bash assign1.sh
```
