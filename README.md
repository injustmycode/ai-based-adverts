# ai-based-advertisement-hikey970

AI based advertisement on Hikey 970
====================================
This application detects a face in OpenCV, then recognizes a gender and age from the face detected using Keras and plays an appropriate advertisement according to the gender and age of the person.

Hardware required:
------------------

  * Hikey 970
  * USB Video Camera

Pre-requisites for Hikey970:
----------------------------
This project has these software pre-requisites to run on Hikey970

  * tensorflow
  * python3
  * python3-pip
  * git
  * git-lfs
  * OpenCV on python3
  * Keras
  
Except for OpenCV on python3 all the other pre-requisites can be installed by running these commands.Tensorflow is already installed in Hikey970 with pre-built Tensorflow.

```
$ sudo apt-get update
$ sudo apt install python3-dev python3-pip git
$ echo 'deb http://http.debian.net/debian stretch-backports main' >> /etc/apt/sources.list
$ sudo apt update
$ curl -s https://packagecloud.io/install/repositories/github/git-lfs/script.deb.sh | sudo bash
$ sudo apt-get install git-lfs
$ git lfs install
$ sudo apt install libopenblas-dev libhdf5-dev python3-scipy python3-h5py
$ pip3 install keras

```

Steps for the AI based advertisement Demo:
-------------------------------------------
To run Run a demo of this project please follow these steps.
We assume that you have already installed the pre-requisites before following these steps

Step 1 : Cloning the Project
----------------------------
on Hikey970 run command to clone this project
```
$ git clone https://github.com/injustmycode/ai-based-adverts.git
```
Step 2: Starting the Demo on Hikey970
-------------------------------------
Run the Demo program
```
$ python3 realtime_demo.py
```
When you run the code, the application detects a face and recognizes the age and gender of the person using that face.Once, the gender and age is recognized it plays different advertisements for different age and gender categories. 

No actual advertisements are placed in the repository due to copyright issues. Download any advertisement(in mp4 format) you want to display and place them in ai-based-adverts root folder. Edit line nos. 130, 140, 150 and 161 and replace the parameter passed with my_function.
For example:  
```
my_function("name_of_your_video.mp4")
```

Inspired by the work of: Tony607
