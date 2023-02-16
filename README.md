# xformers-wheels

### The package is borrowed from [official facebook xformers github actions](https://github.com/facebookresearch/xformers/actions/workflows/wheels.yml)  , and you can download it from "Releases" page of this repo  

### You can also build your own xformers wheels refer below steps:  

`git clone https://github.com/facebookresearch/xformers.git`  
`cd xformers`  
`git submodule update --init --recursive`  
`python -m venv venv`  
`source ./venv/bin/activate`  
`# Change below to your env`  
`pip install torch==1.13.1+cu117 torchvision==0.14.1+cu117 --extra-index-url https://download.pytorch.org/whl/cu117`  
`pip install -r requirements.txt`  
`pip install wheel`  
`pip install ninja`  
`python setup.py build`  
`python setup.py bdist_wheel`  
`ls ./dist/`  

> Make sure you have Nvidia driver installed  
