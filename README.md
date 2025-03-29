# AI-driven Pneumothorax Detection

## About this project

This project focuses on using artificial intelligence to predict the presence of pneumothorax in chest X-rays, 
helping healthcare professionals quickly identify cases for further evaluation.

Pneumothorax occurs when air escapes from the lung into the chest cavity, which can be life-threatening if not 
detected in time. By leveraging AI, this tool aims to assist healthcare workers in the rapid detection of pneumothorax,
potentially improving patient outcomes—especially in regions with limited access to radiologists.

This project is done as part of the [UBC Medicine Datathon 2025](https://datascienceandhealth.ubc.ca/events/ubc-medicine-datathon)
organised by [UBC Data Science and Health](https://datascienceandhealth.ubc.ca).

### Our dataset

The data used in our project is the [NIH Chest X-rays] dataset obtained from [Kaggle](https://www.kaggle.com/datasets/nih-chest-xrays/data).
This dataset is comprised of 112,120 X-ray images with disease labels from 30,805 unique patients. The disease labels 
are obtained by text-mining disease  classifications from the associated radiological reports using Natural Language Processing.

This dataset was produced as a result of the work supported by the [Intramural Research Program of the NClinical Center](www.clinicalcenter.nih.gov) 
and [National Library of Medicine](www.nlm.nih.gov).

### Our product

We leveraged the use of a pre-trained DenseNet121 model from [PyTorch](https://pytorch.org/vision/main/models/generated/torchvision.models.densenet121.html)
to classify x-ray images into `Pneumothorax` and `Negative`. All the work done has been documented in a [Jupyter Notebook](report.ipynb) and the presentation
can be viewed [here](presentation.pdf).

### Running our notebook

If you wish to run our [Jupyter Notebook](report.ipynb), you may do so using the following steps:

1. Clone this GitHub repository.
2. Sign up (if required) and log in to [Kaggle](https://www.kaggle.com).
3. Create a new notebook by clicking the `Create` button on the top left corner of the web page.
4. Under the notebook title `notebook....`, click `File > Import Notebook`.
5. Drag and drop `report.ipynb` and click `Import`.
6. Select `Settings` under the top bar and click `Turn on internet`.
7. Select `Settings > Accelerator` under the top bar and ensure that `GPU T4 x2` is selected.
8. Click `Run All` under the top bar.
9. Running our notebook will take a substantial amount of time (at least 30 min) due to the computational resources required to train a neural network.
You can leave the webpage while the notebook is running. Once the notebook has been fully executed, you will receive an email from Kaggle.

Please avoid running the notebook locally or on any other platform. The notebook is designed to utilise Kaggle's GPU resources and eliminates 
the need to download the 42 GB dataset.

## Contributors

Our team is formed by a group of graduate and undergraduate students at the University of British Columbia, with 
backgrounds in allied health, data science, engineering, medicine, and social sciences. This repository showcases 
the collaborative efforts of our interdisciplinary team.

- Alison Luo [@AlisonLuo](https://github.com/AlisonLuo)
- Danish Karlin Isa [@mdkbmi](https://github.com/mdkbmi)
- Lucy Hui
- Morris Huang
- Robin Matheson [@robinmatheson](https://github.com/robinmatheson)
- Shannon Pflueger [@Shan-non](https://github.com/Shan-non)

## About UBC Medicine Datahon 2025

The UBC Medicine Datathon brings together students and professionals from diverse health disciplines and data-related 
fields to tackle healthcare challenges through data-driven approaches. This interdisciplinary event offers a welcoming space 
for participants to apply their skills and learn from their fellow participants.

In this event, participants work in diverse teams, gain hands-on experience, and contribute to innovative 
solutions in healthcare and technology. In the datathon, participants were given approximately 10 hours to conceptualise, 
prototype and present our product from a selection of 3 different datasets.

## License

This project is licensed under the terms of the MIT license, which can be viewed [here](LICENSE).

The dataset is licensed under the terms of CC0 1.0 Universal license, which can be viewed [here](https://creativecommons.org/publicdomain/zero/1.0/).
