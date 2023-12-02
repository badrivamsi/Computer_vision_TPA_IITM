Our entire code for data downloading, model definition, training and testing 
is in the single ipynb file. 

At many places whenever required we added text block with explanation of the below block.

Before executing any cell , please enable GPU,  from the navigation menu

Edit -> Notebook Settings -> select T4 GPU

Dataset is downloaded from "http://data.vision.ee.ethz.ch/ihnatova/public/dped/dped.gz" 
using tf.keras.utils.get_file()
running the cell will download the data from the website, which will take around 10 mins

load_dataset(True) will load training dataset, where as load_dataset(False) will load test dataset

Need to mount, google drive, in order to save trained models or 
load tranined models. also to save images during tranining and inference.

Cells below the "Traning" heading, are need to be executed only when traninig the model. 
if we want to use saved model to load and do the inference, 

please create a folder "TPA9/TrainedModels" in MyDrive (if not created already)
and upload the shared model to the folder. 
 
Skip executing the training part.

Training will take 40 mins to complete. 

we have a cell with code to load the tranined model from the given path.

once the generator model is loaded from it, 

we can try the generator against the test_dataset (need to be loaded using test_dataset = load_dataset(False)

to generate output.
