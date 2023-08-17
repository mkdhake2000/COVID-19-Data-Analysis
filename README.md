# Plugins-
Software: python3 jupyter notebook (.sh files run python3 jupyter notebooks)

Environments: python 3.7.3


Dependencies-
Python Libraries: pandas v1.3.2, collections, numpy v1.20.2, json 2.0.9,  datetime, math,
		  matplotlib.pyplot(matplotlib v3.4.3), openpyxl(for reading excel file of census data)


Programs-

.sh files:

assign1.sh 
top level script that runs the entire assignment

neighbor-districts-modifier.sh
runs Q1.ipynb as
jupyter nbconvert --to notebook --execute Q1.ipynb

edge-generator.sh
runs Q2.ipynb as
jupyter nbconvert --to notebook --execute Q2.ipynb

case-generator.sh
runs Q3.ipynb as
jupyter nbconvert --to notebook --execute Q3.ipynb

peaks-generator.sh
runs Q4.ipynb as
jupyter nbconvert --to notebook --execute Q4.ipynb

vaccinated-count-generator.sh
runs Q5_Asgn1.ipynb as
jupyter nbconvert --to notebook --execute Q5.ipynb

vaccination-population-ratio-generator.sh
runs Q6.ipynb as
jupyter nbconvert --to notebook --execute Q6.ipynb

vaccine-type-ratio-generator.sh
runs Q7.ipynb as
jupyter nbconvert --to notebook --execute Q7.ipynb

vaccinated-ratio-generator.sh
runs Q8.ipynb as
jupyter nbconvert --to notebook --execute Q8.ipynb

complete-vaccination-generator.sh
runs Q9.ipynb as
jupyter nbconvert --to notebook --execute Q9.ipynb

Jupyter Notebook files:

Q1.ipynb
Input: neighbor-districts.json, cowin_vaccine_data_districtwise.csv
Output: neighbor-districts-modified.json

Q2.ipynb
Input: neighbor-districts-modified.json
Output: edge-graph.csv

Q3.ipynb
Input: neighbor-districts-modified.json, districts.csv
Output: cases-week.csv, cases-month.csv, cases-overall.csv

Q4.ipynb
Input: neighbor-districts-modified.json, districts.csv, cowin_vaccine_data_districtwise.csv
Output: district-peaks.csv, state-peaks.csv, overall-peaks.csv

Q5.ipynb
Input: neighbor-districts-modified.json, cowin_vaccine_data_districtwise.csv
Output: district-vaccinated-count-week.csv, district-vaccinated-count-month.csv,
	district-vaccinated-count-overall.csv, state-vaccinated-count-week.csv, 
	state-vaccinated-count-month.csv, state-vaccinated-count-overall.csv

Q6.ipynb
Input: neighbor-districts-modified.json, cowin_vaccine_data_districtwise.csv,
	DDW_PCA0000_2011_Indiastatedist.xlsx
Output: district-vaccination-population-ratio.csv, state-vaccination-population-ratio.csv,
	overall-vaccination-population-ratio.csv

Q7.ipynb
Input: neighbor-districts-modified.json, cowin_vaccine_data_districtwise.csv,
	DDW_PCA0000_2011_Indiastatedist.xlsx
Output: district-vaccine-type-ratio.csv, state-vaccine-type-ratio.csv,
	overall-vaccine-type-ratio.csv

Q8.ipynb
Input: neighbor-districts-modified.json, cowin_vaccine_data_districtwise.csv,
	DDW_PCA0000_2011_Indiastatedist.xlsx
Output: district-vaccinated-dose-ratio.csv, state-vaccinated-dose-ratio.csv,
	overall-vaccine-type-ratio.csv

Q9.ipynb
Input: neighbor-districts-modified.json, cowin_vaccine_data_districtwise.csv,
	DDW_PCA0000_2011_Indiastatedist.xlsx
Output: complete-vaccination.csv

How to use:
In order to run all programs sequentially, run the following command from the terminal-
bash assign1.sh 
