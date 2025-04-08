# syntactic-processing-assignment
> Identifying Entities in Healthcare Data using NER technique


## Table of Contents
* [How to run](#how-to-run-project)
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)


## How to run project
```
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt
```

```
jupyter notebook \
    --notebook-dir="." \
    --ip=0.0.0.0 --port=3225
```

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- This project involves developing a custom Named Entity Recognition (NER) model for extracting disease and treatment entities from medical text data.
- **Objective**: Given a healthcare dataset in tokenized format, the goal is to identify and map diseases to their possible treatments using a CRF-based NER approach.
- **Use Case**: Such a solution is useful for healthcare platforms like BeHealthy, where structured information on diseases and treatments can assist in better services and data management.
- **Dataset**: The dataset includes tokenized medical notes split into training and test sets along with their corresponding labels:
    - Labels: `D` for Disease, `T` for Treatment, and `O` for Other.


## Conclusions
1. A CRF model was successfully trained using sentence- and word-level features such as part-of-speech tags, token casing, and surrounding words.
2. The model was able to identify key medical entities like diseases and treatments with satisfactory performance.
3. A disease-treatment dictionary was generated mapping each detected disease to its potential treatments.



## Technologies Used
- **Python**: Core programming language.
- **spaCy**: Used for PoS tagging and tokenization.
- **sklearn-crfsuite**: Conditional Random Field implementation for NER.
- **pandas & NumPy**: Data processing.
- **Jupyter Notebook**: Development and demonstration environment.



## Contact
Created by [@jafarijason](https://github.com/jafarijason) - feel free to reach out for collaboration or further inquiries.
Connect with me on [LinkedIn](https://www.linkedin.com/in/jasonjafari/).

