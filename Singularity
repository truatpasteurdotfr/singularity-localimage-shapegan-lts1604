Bootstrap: localimage
From: /master/home/tru/singularity.d/containers/singularity-docker-lts1604-conda-pytorch-2020-02-05-1913.sif
### or build from scratch by adapting the singularity-docker-lts1604-conda-pytorch/Singularity file

%post
PATH=/opt/miniconda3/bin:$PATH
export PATH

# shapegan via pip
python3 -m pip install \
	 mesh-to-sdf \
	 trimesh \
	 pyopengl \
	 pyrender \
	 sklearn \
	 scikit-image \
	 pygame \
	 opencv-python  \

# missing X11?
apt-get -y update
apt-get -y install libx11-6 libxext6 libgl1 libsm6 libxrender1 libx11-dev nano git zip unzip libglu1-mesa libglib2.0
 
%environment
PATH=/opt/miniconda3/bin:$PATH
export PATH


