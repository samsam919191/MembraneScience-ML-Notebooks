Membrane Distillation Machine Learning Analysis
This repository contains Jupyter notebooks that apply machine learning techniques to analyze data from four membrane distillation methods: Air Gap Membrane Distillation (AGMD), Vacuum Membrane Distillation (VMD), Sweep Gas Membrane Distillation (SGMD), and Direct Contact Membrane Distillation (DCMD). The notebooks implement models such as Deep Learning, Support Vector Regression (SVR), and XGBoost to evaluate performance metrics and feature importance.

Dataset Sources
The datasets used in this analysis are provided in the data folder as CSV files: agmd.csv, dcmd.csv, sgmd.csv, and vmd.csv. They were obtained from the following research papers:

VMD: G. Naidu, Y. Choi, S. Jeong, T. M. Hwang, S. Vigneswaran, "Experiments and modeling of a vacuum membrane distillation for high saline water," J. Ind. Eng. Chem. 20 (2014) 2174–2183. DOI: 10.1016/j.jiec.2013.09.048
Data Extraction: Extracted from graphs using WebPlotDigitizer.
DCMD: A. Khalifa, H. Ahmad, M. Antar, T. Laoui, M. Khayet, "Experimental and theoretical investigations on water desalination using direct contact membrane distillation," Desalination 404 (2017) 22-34. DOI: 10.1016/j.desal.2016.10.009
Data Extraction: Extracted from graphs using WebPlotDigitizer.
SGMD: M. Khayet, C. Cojocaru, "Artificial neural network model for desalination by sweeping gas membrane distillation," Desalination 308 (2013) 102–110. DOI: 10.1016/j.desal.2012.06.023
Data Extraction: Available directly as tables in the paper.
AGMD: M. Khayet, C. Cojocaru, "Artificial neural network modeling and optimization of desalination by air gap membrane distillation," Sep. Purif. Technol. 86 (2012) 171–182. DOI: 10.1016/j.seppur.2011.11.001
Data Extraction: Available directly as tables in the paper.
Note: For VMD and DCMD, the data was extracted from graphs using WebPlotDigitizer, which may introduce minor inaccuracies. For SGMD and AGMD, the data was copied directly from tables in the papers. Users are encouraged to refer to the original papers for the authoritative data.

Notebooks
This repository includes the following Jupyter notebooks:

AGMD.ipynb: Implements Deep Learning, SVR, and XGBoost models for AGMD, evaluating metrics such as MAE, MSE, R², and RMAE.
VMD.ipynb: Similar to AGMD.ipynb, but for VMD.
SGMD.ipynb: Similar to AGMD.ipynb, but for SGMD.
DCMD.ipynb: Similar to AGMD.ipynb, but for DCMD.
Piechart.ipynb: Uses XGBoost, SHAP, and ANOVA to analyze all four configurations together, providing insights into feature importance.
Data_Points_vs_RMAE_AGMD_VMD_DCMD.ipynb: Employs XGBoost to visualize the relationship between the number of data points and RMAE for AGMD, VMD, and DCMD.
Data_Points_vs_RMAE_SGMD.ipynb: Similar to the above, but for SGMD, with results averaged over multiple runs due to data sensitivity.

How to Use
Clone the Repository:
git clone https://github.com/samsam919191/MembraneScience-ML-Notebooks.git
Install Dependencies:
The notebooks require Python 3.x and the following libraries: pandas, numpy, scikit-learn, xgboost, shap, matplotlib, and others. Install them using:
pip install pandas numpy scikit-learn xgboost shap matplotlib
Check individual notebooks for any additional dependencies.
Run the Notebooks:
Open the .ipynb files in Jupyter Notebook, JupyterLab, or Google Colab.
The notebooks assume the datasets are in the data folder (e.g., data/agmd.csv). Adjust paths if necessary.


Data Extraction Details
For VMD and DCMD, datasets were extracted from graphs using WebPlotDigitizer. This process may introduce slight inaccuracies; refer to the original papers for precise data.
For SGMD and AGMD, datasets were directly copied from tables in the papers.
Contact
For questions or issues, please open a GitHub issue or contact [saman.tarhani@yahoo.com].

License
Code: MIT License
Data: Derived from the listed papers for research purposes. Please cite the original papers and respect publishers' copyright policies.
