# Custom Named-Entity-Recognition

# About

This is an implementation of the Custom Named-Entity-Recognition which applies BERT. <br>
The objective is to find useful information present in resume like Education, Skills, Experience, etc. <br>
BERT - https://github.com/google-research/bert#what-is-bert <br>

# Links
Dataset - (https://www.kaggle.com/dataturks/resume-entities-for-ner)

# Install venv and activate
```bash
pip install virtualenv
virtualenv venv
cd venv/Scripts
activate 
OR 
source venv/bin/activate
```

# Install requirements
```bash
pip install -r req.txt
```

# Training

To train the model, Run:
```bash
python train.py
``` 
optional arguments:

-e epochs &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Number of Epochs

-o path &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Output path to save the trained model

# Flask REST API

```bash
python app.py
```
API will be live at endpoints : https://localhost:5000/predict/

### Test the API
Either use cURL, Postman or any other REST client
```bash
curl --location --request POST "http://localhost:5000/predict" --form "resume=@/resume-path.pdf"
```

NER Demo result
![NER results](https://github.com/sumedhkhodke/Custom-Named-Entity-Recognition/blob/main/Screenshot%202021-11-30%20230039.jpg)

For bugs and suggestions, please raise a pull request or drop me a mail at sumedh.khodke@gmail.com
