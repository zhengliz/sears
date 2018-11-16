# sears
Code for [Semantically Equivalent Adversarial Rules for Debugging NLP Models](https://homes.cs.washington.edu/~marcotcr/acl18.pdf)

# Installation
Run the following:
```
git clone git@github.com:marcotcr/sears.git
cd sears
virtualenv -p python3 ENV
source ENV/bin/activate
pip3 install editdistance keras numpy==1.14.5 jupyter tensorflow-gpu==1.10.1 torchtext==0.1.1 spacy==2.0.0
pip3 install http://download.pytorch.org/whl/cu90/torch-0.4.0-cp35-cp35m-linux_x86_64.whl
python -m ipykernel install --user --name=sears
python -m spacy download en
git clone https://github.com/marcotcr/OpenNMT-py
cd OpenNMT-py/
python setup.py install
cd ..
```

Download and unpack [the translation models](https://drive.google.com/open?id=1b2upZvq5kM0lN0T7YaAY30xRdbamuk9y) into the `translation_models` folder.

Run `jupyter notebook`, change kernel to `sears`, and run the notebook :)
