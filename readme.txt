!nvcc --version
!g++ -v
!/opt/bin/nvidia-smi

!tar -xvf VanitySearch.tar -C /content
%cd VanitySearch
!make clean
# !make gpu=1 ccap=37 CXXCUDA=/usr/bin/g++ CUDA=/usr/local/cuda-11.1 all
!make gpu=1 ccap=75 CXXCUDA=/usr/bin/g++ CUDA=/usr/local/cuda-11.1 all


!./VanitySearch -t 0 -sk BC6AF35000000000 -sb 26 -gpu 16jY7q