# NICF
Group: Jiamo Liu, Yuqing Wang<br/> 
Data format Explaination:<br/> 
- First number in each line of data/env.dat is the userId, the demo set has userId 1-100 <br/> 
- All numbers after the first number is in the format a:b, example:<br/> 
3:4 means user gives movie ID 3 a rating of 4 stars.<br/> 




Instruction for environment configuration:

- Install docker, relevant info: <br/> 
https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository

- Pull the legacy tensorflow 1.15 image: <br/> 
docker pull tensorflow/tensorflow:1.15.2-py3-jupyter

- Spin up a bash terminal in docker container: <br/>  
docker run -it --rm tensorflow/tensorflow:1.15.2-py3-jupyter bash 

- Inside the docker bash terminal, install git, and other modules using the following: <br/> 
apt-get update <br/> 
apt-get install git <br/> 
pip install ipdb <br/> 
pip install sklearn 


- Clone the Repo:<br/> 
git clone https://github.com/JiamoLiu/NICF_Jiamo.git <br/> 
cd NICF_Jiamo

- Train the model using bash script:<br/> 
bash model_train.sh
