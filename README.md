# MNIST_Docker
MNIST in simple docker using Jupyter notebook


## 📝 Table of Contents
- [About](#about)
- [Usage](#usage)
- [Built Using](#built_using)
- [Authors](#authors)
- [Acknowledgments](#acknowledgement)
- [License](#licence)




## :bulb: About <a name = "about"></a>

# MNIST Handwritten digits

The MNIST handwritten digits implementation in Docker: Jupyter Notebooks


### General description on the project
The project will make you to run the MNIST Handwritten digits problem in a Jupyter Notebooks Docker. The Docker is based on the latest Jupyter Datascience Docker slacks. The data required for the model training is avaialble as csv files and the corresponding Jupyter Notebooks is also included in the repo 



### Idea and goal of the project
To demonstrate the docker implementation with a small machine learning project


### Prerequisites
Docker installed in the system


## 🎈 Usage <a name="usage"></a>
Add notes about how to use the system.

The deocker can be deployed in the following steps:

Note: avoid sudo if necessary

1. Clone this repository having the data and jupyter notebook and move to the main folder
```
cd MNIST_Docker
```
2. Run the latest image from jupyter docker slacks and then run the image mounting the ´pwd´ containing all our files as reference. The port of Jupyter Notebook is mapped to localhost port 80 and the container is named as "jupyter"

```
sudo docker run --name=jupyter -d -p 80:8888 -v $(pwd):/home/jovyan -w /home/jovyan jupyter/datascience-notebook:latest
```

3. Get the token to log in the jupyter using:

```
sudo docker logs jupyter
```
Copy the token and open the browser run local host ´http://localhost:80/´

After sucessfully inputing the token, the jupyter will be loaded and will be ready to run. 

4. Follow the steps in the Notebook for the MNIST Handwritten digits model


## ⛏️ Built Using <a name = "built_using"></a>
Tested on Docker Version 20.10.13 running on ubuntu 20.04.3



## ✍️ Authors <a name = "authors"></a>
Jibinraj Antony



## 🎉 Acknowledgements <a name = "acknowledgement"></a>
1. Jupyter Docker stacks: https://github.com/jupyter/docker-stacks
2. Source of data: https://python-course.eu/machine-learning/training-and-testing-with-mnist.php 



## ✒️ License <a name= "licence"></a>
No informations --
