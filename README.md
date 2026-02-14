

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

## Training

- SET CUDA_VISIBLE_DEVICES=1
- python train.py -s F:\CARVATAR\flowers
 
### their data
- SET CUDA_VISIBLE_DEVICES=1
- python train.py -s F:\CARVATAR\scan01_format_3dgs_official
- python train.py -s F:\CARVATAR\scan01_format_3dgs_official --data_device cpu # SUPER IMPORTANT WHEN MANY IMAGES. OTHERWISE FOR SOME REASON VERY SLOW

##
- conda activate F:\conda_envs\3dgs_official
- SET CUDA_VISIBLE_DEVICES=1
- python train_alpha.py -s F:\CARVATAR\scan01_format_3dgs_official --data_device cpu --model_path F:\CARVATAR\scan01_output --resolution 1
-
-
-
