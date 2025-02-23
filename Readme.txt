There are 4 different ways to Collecting the data - 

1. Manually Collecting like downloading the images from web/ which is not good. cause
   for collecting huge datasets are not efficient way through downloading process 
2. using python and web scrapping to collect the data in an automated ways
3. already created datasets and finally
4. Using falktun tools to collect the data which is chrome extension that can be used as well.


At first we will gor through a Data cleaning process since we don't know how
we are going to detect the images datasets.

So, we are going to detect only those images which have two eyes which will
give use a clear idea or, the machine which character it is.

if we detect the face or, two eyes clearly then we will take the image otherwise 
not.

for this process we will use OpenCV python library for image detection

// Now another thing is if there is Two persons with different identity in the same image
 then we will use manual verification which will clear to remove the one of the face and
 detect the other one.

// Also we will cropped faces with two eyes nad face through haar cascade method


Okay, The process will be - 

Raw images ----> Cropped faces with two eyes using haar cascade -----> Manual Data cleaning ---
-----> Wavelet transformed images for Feature engineering -------> Train our model with hyper tuning
-------> Then, saved our model to a file ------> Then, webpage design and  ------> 
Connect with flask Server -------> Save the model


// Now the cropped images folder has been created now I will do the Wavelet transformation of the
images which will extract the important features of the images

//There are other ways to extracting the features of the images but Wavelet transformation is
  one  of the effective way to extract the features of the images

// Study the -  1. Time domain and signal processing domain

// Now since I created the function that will transform the image into Wavelet
// Now I will iterate through the celebrity_img_dictionary to transform the image into Wavelet
  formation
  