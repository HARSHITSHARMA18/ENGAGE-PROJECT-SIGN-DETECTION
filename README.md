# ENGAGE INTERN 2022 PROJECT - ALPHABET DETECTION MODEL
<p>This project is made for the importance and awareness of sign language. In this model starting alphabet are detected due to contraint of days 

## Steps
<br />
<b>Step 1.</b> Clone this repository: https://github.com/HARSHITSHARMA18/ENGAGE-PROJECT-SIGN-DETECTION.git
<br/><br/>
<b>Step 2.</b> Create  new virtual environment 
<pre>
python -m venv tfod
</pre> 
<br/>
<b>Step 3.</b> Activate the  virtual environment
<pre>
source tfod/bin/activate # Linux
.\tfod\Scripts\activate # Windows 
</pre>
<br/>
<b>Step 4.</b> Install dependencies and add virtual environment to the Python Kernel
<pre>
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=tfodj
</pre>
<br/>
<b>Step 5.</b> Collect images using the Notebook <a href="https://github.com/HARSHITSHARMA18/ENGAGE-PROJECT-SIGN-DETECTION/blob/main/1.%20Image%20Collection.ipynb">1. Image Collection.ipynb</a> - ensure you change the kernel to the virtual environment as shown below
<img src="https://i.imgur.com/8yac6Xl.png"> 
<br/>
<b>Step 6.</b> Manually divide collected images into two folders train and test. So now all folders and annotations should be split between the following two folders. <br/>
\TFODCourse\Tensorflow\workspace\images\train<br />
\TFODCourse\Tensorflow\workspace\images\test
<br/><br/>
<b>Step 7.</b> Begin training process by opening <a href="https://github.com/HARSHITSHARMA18/ENGAGE-PROJECT-SIGN-DETECTION/blob/main/2.%20Training%20and%20Detection.ipynb">2. Training and Detection.ipynb</a>, this notebook will walk you through installing Tensorflow Object Detection, making detections, saving and exporting your model. 
<br /><br/>
<b>Step 8.</b> During this process the Notebook will install Tensorflow Object Detection. You should ideally receive a notification indicating that the API has installed successfully at Step 8 with the last line stating OK.  
<img src="https://i.imgur.com/FSQFo16.png">

<br /> <br/>
<b>Step 9.</b> Once you get to step 6. Train the model, inside of the notebook, you may choose to train the model from within the notebook. I have noticed however that training inside of a separate terminal on a Windows machine you're able to display live loss metrics. 
<img src="https://i.imgur.com/K0wLO57.png"> 
<br />
<b>Step 10.</b> You can optionally evaluate your model inside of Tensorboard. Once the model has been trained and you have run the evaluation command under Step 7. Navigate to the evaluation folder for your trained model e.g. 
<pre> cd Tensorlfow/workspace/models/my_ssd_mobnet/eval</pre> 
and open Tensorboard with the following command
<pre>tensorboard --logdir=. </pre>
Tensorboard will be accessible through your browser and you will be able to see metrics including mAP - mean Average Precision, and Recall.
<br />


<b>ERROR: 
Majority of error's solution can be found out here:https://docs.google.com/document/d/1wvrP5ZckR878VLZdDFavWc-63xM15BzSVw8bUVJfXQ8/edit?usp=sharing

<b>DEMO VIDEO 
 https://drive.google.com/file/d/1L9GsHdFKbnCqrfZD6ABYU6QC2ANzBETm/view?usp=sharing
