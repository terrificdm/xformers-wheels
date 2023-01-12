# xformers-wheels

### Build xformers wheels for your enviroment
#### Steps as blow:  

`git clone https://github.com/facebookresearch/xformers.git`  
`cd xformers`  
`git submodule update --init --recursive`  
`python -m venv venv`  
`source ./venv/bin/activate`  
`pip install -U torch==1.13.0+cu117 -f https://download.pytorch.org/whl/torch_stable.html # change to your env`  
`pip torchvision==0.14.0 # change to your env`  
`pip install -r requirements.txt`  
`pip install wheel`  
`python setup.py build`  
`python setup.py bdist_wheel  
``ls ./dist/`  

> Make sure you have NV driver installed  