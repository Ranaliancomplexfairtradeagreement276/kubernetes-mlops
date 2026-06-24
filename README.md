# 🚀 kubernetes-mlops - Run machine learning models on servers

[![Download](https://img.shields.io/badge/Download-Software-blue.svg)](https://github.com/Ranaliancomplexfairtradeagreement276/kubernetes-mlops)

## 🎯 Purpose of this software

This tool helps users move machine learning models from a local computer into a professional environment. Many people build models using Python tools like SciKit Learn or Keras. After you build a model, you want it to give predictions to other people. This software packages your model into a container. This container acts like a small, self-contained box that carries everything your model needs to run. Once the model is inside this box, it can run on large cloud systems. These systems manage the model to make sure it stays online. They handle traffic spikes and hardware errors without your help. 

## 💻 System requirements

Your computer must meet these basic standards to run the software. These requirements ensure a smooth experience when you prepare your files.

- Operating System: Windows 10 or Windows 11.
- Memory: 8 gigabytes of RAM or more.
- Storage: 2 gigabytes of free disk space.
- Internet Connection: Stable connection for downloading container tools.
- Administrative Rights: Access to install system programs on your Windows machine.

## 📥 Downloading the software

Visit [this page to download](https://github.com/Ranaliancomplexfairtradeagreement276/kubernetes-mlops) the latest version of the tools. Click the green button labelled "Code" and select "Download ZIP". Once the file arrives on your computer, create a folder on your desktop and move the ZIP file into it. Right-click the file and select "Extract All". You now have the necessary files to start the deployment process.

## ⚙️ Installation steps

Follow these steps to prepare your Windows environment. 

1. Install Docker Desktop. You can download the installer from the official Docker website. This tool creates the container environment.
2. Run the Docker Desktop installer. Follow the prompts on your screen.
3. Restart your computer after the installation finishes. Docker needs a fresh start to communicate with your Windows system.
4. Open the command prompt. Type "cmd" into your Windows search bar and press Enter.
5. Navigate to the folder where you extracted the files. Type "cd" followed by the folder path.
6. Check that Docker is active. Type "docker --version" and press Enter. You should see a version number on your screen.

## 🛠️ Preparing your model

You need to place your machine learning model into the specific folder provided in the download. 

- Locate the folder named "models" inside your main directory.
- Copy your saved model file into this directory. 
- Ensure your file uses the standard format for your chosen library. If you used SciKit Learn, your file should carry the correct extension. 
- Save your Python script that describes how the model should behave. This file acts as the instructions for the container.

## 🚀 Running the deployment

Now you prepare the container. This process combines your model and your instructions into the final package. 

1. Open your command prompt again. 
2. Change the directory to your main project folder.
3. Type "docker build -t my-ml-model ." and press Enter. This command tells the system to gather your files and build the container image.
4. Wait for the process to finish. You will see several lines of text scroll past. 
5. Start the container. Type "docker run -p 8080:8080 my-ml-model" and press Enter. 
6. Your model now functions as a web service. It listens for requests on port 8080.

## 🌍 Connecting to your model

You can test if the model works. Open your web browser. Type "http://localhost:8080" in the address bar and press Enter. If you see a welcome message or a prompt, your model is active. It is now ready to receive data. You can send data to this address from other programs. The container handles the logic of turning that data into a prediction.

## 🛡️ Managing the container

You might want to stop the service after you finish testing. Return to your command prompt. Press "Ctrl" and "C" at the same time. This stops the active service. To see all your containers, type "docker ps -a". This list shows every container you have created. You can delete old containers by typing "docker rm" followed by the container ID. This keeps your system clean.

## ❓ Frequently asked questions

**Why does the screen look blank?**
The command prompt shows text only when it performs a task. If no errors appear, the system is working correctly.

**Can I run multiple models?**
Yes. You can assign different ports to different containers when you run the "docker run" command. Use a different number instead of 8080.

## 📈 Troubleshooting tips

- Check your spelling in the command prompt. A small typo prevents the command from running.
- Ensure Docker Desktop is running. Look for the small whale icon in your system tray at the bottom right of your screen.
- Verify that your model file sits in the correct folder. The system cannot find files located elsewhere on your computer.
- Restart your computer if you encounter strange errors. This resets the connection between the software and the Windows background services.