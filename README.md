

## Install
- SET DISTUTILS_USE_SDK=1 # Windows only
- conda env create --file environment.yml --prefix F:\conda_envs\3dgs_official

## Try again

- SET DISTUTILS_USE_SDK=1
- conda create --prefix F:\conda_envs\3dgs_official -y python=3.8
- conda activate F:\conda_envs\3dgs_official
- pip install torch==2.1.2+cu118 torchvision==0.16.2+cu118 --extra-index-url https://download.pytorch.org/whl/cu118
- pip install plyfile
- pip install tqdm
- pip install opencv-python
- pip install joblib


- MAYBE NEEDED; FOR NOW I DON4T RUN IT
- conda install -c "nvidia/label/cuda-11.8.0" cuda-toolkit



## Activate
- conda activate F:\conda_envs\3dgs_official
