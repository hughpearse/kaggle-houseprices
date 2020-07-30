# kaggle-houseprices

# Data
https://www.kaggle.com/c/digit-recognizer

# Program Usage
```bash
foo@bar:~$ pip install jupyterlab
foo@bar:~$ virtualenv sandbox
foo@bar:~$ virtualenv -p $(which python3) sandbox
foo@bar:~$ source sandbox/bin/activate
foo@bar:~$ pip install -r ./requirements.txt
foo@bar:~$ kaggle competitions download -c digit-recognizer -p ./data
foo@bar:~$ python -m ipykernel install --name=sandbox
foo@bar:~$ jupyter notebook
foo@bar:~$ deactivate
```

