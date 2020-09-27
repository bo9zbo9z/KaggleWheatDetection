### Kaggle Wheat Detection

These are a series of notebooks forked from Object Detection Series  (https://fairyonice.github.io/tag/object-detection-using-yolov2-on-pascal-voc2012-series.html)  Github repo (https://github.com/FairyOnIce)

As you read the notebooks, I want to be clear, the vast majority of the code is straight from the original notebooks, I take no credit from their content.

Here is some background.  I entered the Kaggle Global Wheat Detection, https://www.kaggle.com/c/global-wheat-detection, which used a You Only Look Once, YOLO, type of solution.  I had no experience with this type of model, I read articles, reviewed notebooks, etc.  But. was not able to really understand the concepts.  My first attempt scored less than 1% accuracy, you could random guess better than that.....  So, I started looking at some of the on-line classes and Kaggle notebooks, which helped a little.

Then I found her blog on Object Detection using PASCAL VOC2012 data.  It was a series of notebooks that slowly walked you through all of the steps and concepts.  There were also reference links for more detailed information.

After going through them, it finally made sense, :).  I took her notebooks and modified them to use the Kaggle Wheat data, albumentations and other changes to be TF 2.x compliant.  Majority of the changes were very minor, I did have to change the Generator and loss inputs to resolve a problem with passing a tensor through to the loss.  (I was about ready to give up, but found an easy solution, you can look at the notebooks for additional information.)

I added three additional notebooks that build on the existing ones.  All are easy to understand and should give you an idea of what it takes to train a model using YOLO.  This is not a winning solution, but obtain accuracy around high 50% to low 60%.  I use the free Google Colab for my main training environment, which means I'm limited on memory, disk and GPU.  I believe results would be higher with increased capacity.  

I did not change any of the comments from the original notebooks, so you will see references back to PASCAL VOC2012 data.  I left them as is to help with the learning because majority of what she describes fits for Wheat Detection.  Those notebooks have "Part 1/2/3/4/5/6" in the titles.  The notebooks I added have "Part x" in their title.  These were specific to changes I had to make to resolve the tensor issue, albumentations, Colab training and Kaggle submission.
