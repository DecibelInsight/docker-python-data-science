FROM python:3.7-buster

LABEL maintainer = "Gonzalo Bandeira <gbandeira@decibelinsight.com>"

# install the scientific stuff here
RUN pip3 install --no-cache-dir numpy==1.17.3 &&\
    pip3 install --no-cache-dir cython==0.29.13 &&\
    pip3 install --no-cache-dir joblib==0.14.0 &&\
    pip3 install --no-cache-dir pandas==0.25.2 &&\
    pip3 install --no-cache-dir scipy==1.3.1 &&\
    pip3 install --no-cache-dir scikit-learn==0.21.3 &&\
    pip3 install --no-cache-dir nltk==3.4.0 &&\
    pip3 install --no-cache-dir spacy==2.2.4

# install language dictionaries needed by NLP libraries
RUN /usr/local/bin/python -m nltk.downloader stopwords &&\
    /usr/local/bin/python -m nltk.downloader stopwords &&\
    /usr/local/bin/python -m nltk.downloader wordnet &&\
    /usr/local/bin/python -m nltk.downloader omw &&\
    /usr/local/bin/python -m nltk.downloader punkt &&\
    /usr/local/bin/python -m nltk.downloader averaged_perceptron_tagger &&\
    /usr/local/bin/python -m spacy download xx &&\
    /usr/local/bin/python -m spacy download en

RUN echo "finished"