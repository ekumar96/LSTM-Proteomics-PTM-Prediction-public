# LSTM-Proteomics-Tyrosine-Sulfation-Prediction
[Link](https://drive.google.com/file/d/1rP9UiiMO52I5wiX1_1aqCO63FvHN9Ksd/view) to Presentation.

On top of my regular work at Codexis, Inc., I went the extra mile and took the initiative to brainstorm, devise and independently build several ML-based Bioinformatics tools, including an LSTM-based tool for in-silico Hemophilia proteomics gene therapy research (post-translational modification prediction), with industry-leading 0.968 Matthews Correlation Coefficient score using Python Tensorflow. To do so, I had to take several steps:
1) I optimized the model ensemble parameters with a 10,000 model grid search for a highly skewed and scarce dataset
2) I collaborated with the gene therapy team to fine-tune tool and add front-end functionality to best fulfill and exceed project needs
3) I deployed the tool in the company-wide software suite for use in other projects
This tool led to greater confidence in the therapeutic safety of the evolved Factor VIII gene before insertion into the human body, and is still used by the company today.

Note: Due to confidentiality, whether or not I can release code snippets from this project is still pending. 

## Data set:
The data for this project is from the pdb, or the protein database. As this project is investigating Tyrosine Sulfation, several proteins with Sulfated Tyrosines were selected, as well as several without. This gave us roughly 10,000 protein sequences. Each protein sequence was sliced into pieces with variable length overhang surrounding each tyrosine, and each tyrosine's sulfation status was also recorded as the Y variables. The X variables were a sequence of amino acids surrounding a Tyrosine, and the Y variables were a 1 or a 0 representing suflation status. After data preprocessing, data augmentation was also used to increase the size of the scarce and skewed dataset. 
