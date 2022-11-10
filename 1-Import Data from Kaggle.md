# **Import Data from Kaggle**
**STEP 1 : Create an account in Kaggle**
- Go to https://www.kaggle.com/
- Click on Register to create an account

**STEP 2 : Download API Credentials** 
- To download data from Kaggle, you need to authenticate with the Kaggle services. For this purpose, you need an API token. This token can be easily generated from the profile section of your Kaggle account. Simply, navigate to your Kaggle profile and then,
![alt text](https://editor.analyticsvidhya.com/uploads/82084ds.PNG)

- Click the Account tab and then scroll down to the API section (Screenshot from Kaggle profile)
A file named “kaggle.json” will be download which contains the username and the API key.
This is a one-time step and you don’t need to generate the credentials every time you download the dataset.

**STEP 3 : Setup the Colab Notebook**
-  upload the “kaggle.json” file that you just downloaded from Kaggle.

![alt text](https://editor.analyticsvidhya.com/uploads/56124e.PNG)

- Now you are all set to run the commands need to load the dataset. Follow along with these commands:

- Note: Here we will run all the Linux and installation commands starting with “!”. As Colab instances are Linux-based, you can run all the Linux commands in the code cells.
1. Install the Kaggle library
```
! pip install kaggle
```
2. Make a directory named .kaggle

```
! mkdir ~/.kaggle
```
3. Copy the “kaggle.json” into this new directory
```
! cp kaggle.json ~/.kaggle/
```
4. Allocate the required permission for this file.
```
! chmod 600 ~/.kaggle/kaggle.json
```
**STEP 4 : Downloading Datasets**

```
! kaggle datasets download jutrera/stanford-car-dataset-by-classes-folder`
```
- Unzip the dataset

```
! unzip /content/stanford-car-dataset-by-classes-folder.zip
```

