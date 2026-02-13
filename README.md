

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
- conda install -c "nvidia/label/cuda-11.8.0" cuda-toolkit
- pip install ninja
- then check this: https://chatgpt.com/c/698e87c4-f2c8-838c-a273-bb7a81daf3db
  - GO TO EACH SUBMODULE & CALL pip install . --no-build-isolation -v
  - IF ISSUE; check gpt link



## Activate
- conda activate F:\conda_envs\3dgs_official
