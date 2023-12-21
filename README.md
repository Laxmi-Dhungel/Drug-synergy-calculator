# Drug-synergy-calculator
In drug synergy experiment, we examine effectiveness of combination treatment of drugs against cells (e.g. cancer cells) compared to treatment with its single components. If synergistic then the combination treatment with drugs will exhibit higher inhihibition compared to treatment with its single component. However, if antagonistic an opposite effect can be seen. Combination treatment with multiple drugs are in rise for treatment of diseases such as cancer. These type of combination treatment can provide benefits such as reduced toxixity, multiple targets and can adress resistance issues(Ayoub, 2021). However, these drugs need to act synergistically to obtain their benefits.

This code is for the analysis of drug synergy experiment testing effectinveness of combination of two different drugs. Both drugs are used in a range of concentrations in a 96 well plate. A sample plate design for the experiment is shown below. Here, each drugs are used with an increment in concentration of 10 uM. However, the concentration of drugs used may depend on study. 

<img width="432" alt="Plate design" src="https://github.com/Laxmi-Dhungel/Drug-synergy-calculator/assets/154451345/ab41064a-eea7-4ceb-91f9-d1e247fb7dd6">

The experiment is conducted and the optical density is measured. A sample csv file format is attached. Here, I have combined two separate experiment into a csv file. Hence, results from multiple experiments can also be analyzed using this calculator.

<img width="935" alt="csv_for_data" src="https://github.com/Laxmi-Dhungel/Drug-synergy-calculator/assets/154451345/832f8c4f-b85a-4c66-a92a-c6073a26f6ed">

The well that consists of concentration of 0 uM for both drug is untreated (hence control for the experiment). For convenience in data analysis, the OD value for A0-B0 for each experiment is copied to the last row and is named control. The user also need to upload the data in this format and assign a row for control. 

After the code is run, users will be asked to provide input on filename, first shell name in the csv file (which is treatment here), control name, title and labels for heat map. A heat map is generated using these information which can be saved.

<img width="461" alt="Input_filename" src="https://github.com/Laxmi-Dhungel/Drug-synergy-calculator/assets/154451345/22f06ad4-1982-4575-a2bd-68b8f503d782">

![heatmap](https://github.com/Laxmi-Dhungel/Drug-synergy-calculator/assets/154451345/264ed8a7-e3d2-4548-a5fb-162445eddf15)

Then the user will be asked to provide information on barchart. For statistical analysis, it is important that there are atleast 3 replicates of sample. Uer will be asked if they want to generate a bargraph with or without statistics (need to type correct option). I have typed 2 here opting for barchart with statistical analysis. Then a barchart is generated that can be saved. Users will also be provided with the information on type of statistical test used (which is Tukey hsd test). 

<img width="471" alt="barchart_information" src="https://github.com/Laxmi-Dhungel/Drug-synergy-calculator/assets/154451345/5f770cf3-5382-4257-acba-5dd3bff57563">

![barchart](https://github.com/Laxmi-Dhungel/Drug-synergy-calculator/assets/154451345/47896316-9ddc-4e7d-9ec3-2e3027d5540a)

The users will also be provided with an option to save the csv file on mean percentage survival. This data may be needed for  future analysis or to calculate synergy using SynergyFinder. SynergyFinder is an online based tool that uses different models to determine the synergy between combination of drugs used (https://synergyfinder.fimm.fi/synergy/20231221200024168277/). It provides heatmap and 3D models showing synergistic and antagosnistic pattern in the combination of drugs used. The use of this calculator based code is different than SynergyFinder as this is focussed on calculating percentage survival from OD values obtained and generates bargraph and heatmap showing information on the percentage survival. 

<img width="461" alt="save_file" src="https://github.com/Laxmi-Dhungel/Drug-synergy-calculator/assets/154451345/ad2d6ec2-747e-45bc-b1a2-250778f1128a">


At the end, I cannot thank python and its tool enough for making this hours of work possible in just few minutes!!

References:
1. Ayoub NM. Editorial: Novel Combination Therapies for the Treatment of Solid Cancers. Front Oncol. 2021;11:708943
