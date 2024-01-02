FROM nvidia/cuda:12.1.1-runtime-ubuntu20.04

RUN apt-get update -y && apt-get install -y python3.9 python3.9-distutils curl vim git
RUN curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
RUN python3.9 get-pip.py
RUN ln -s /usr/bin/python3.9 /usr/bin/python
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install accelerate==0.25.0 colorama datasets einops exllamav2==0.0.11
RUN pip install gradio==3.50.2 hqq==0.1.1.post1 lm_eval==0.3.0 markdown numpy==1.24.4 optimum==1.16.1
RUN pip install pandas peft==0.7.1 Pillow==10.1.0 pyyaml requests rich safetensors==0.4.1 scipy sentencepiece
RUN pip install tensorboard transformers==4.36.2 tqdm wandb
RUN pip install bitsandbytes==0.41.1