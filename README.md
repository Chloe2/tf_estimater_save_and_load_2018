## tf_estimater_save_and_load  
Author: Toby  

### **General description:**  
The [Kaggle NYC taxi fare challenge](https://www.kaggle.com/c/new-york-city-taxi-fare-prediction) comes with a coupon of intro to tensorflow on google cloude. But during the process, I found that many necessary components were missing. That's the main reason why this notebook is written.

### **Content:**  
In this notebook, we use a toy example to see how to:
1. prepare data for the model
2. define a tf estimator
3. train your model from a fresh start
4. train your model from last check point
5. export (/save) your model
6. reload your saved model
7. use your trained model to make predictions
8. monitor the training process with tensor board.

### **Conclusion**  
From the online class offered by google on coursera on tensorflow, I believe tf estimator is a product designed to be friendly and easy-to-use for machine learning beginners. However, after finished the online class and tried tf estimator by myself on the kaggle challenge, I personally will not recommend tf estimator as a good starting point for anyone's attempt in learning machine learning. I have mainly 3 reasons/aguments: 
1. there are many (actually too many) documents about tensorflow. But most of the official ones don't come with an example. 
2. tensorflow has a very complicated structure (keras-estimator-session-lower level...) with two different modes (eager and lazy.) Each has their unique syntax and package. This make debugging tf very difficult for less experience coders.
3. as powerful as tf estimator, it doesn't really provide you everything you will need to be a real data scientists. Under many occations you will find that the thing you wanna control and change is not available via estimator.

After a little bit research online, I made my decision to move forward with pytorch:
1. (personally) most of my friends at NYU use pytorch in their classes
2. pytorch has a GREAT collection of documents, and almost every function comes with a handy example (which I REALLY like.)
3. pytorch is more pythonic compared to tensorflow. It's much easier to use all the debugging techniques you learned in python.
4. as far as you are not building a product serving millions of people, pytorch is as powerful as tensorflow
5. I heard a lot good things from pytroch especially the recent news about [pytorch from fast.ai](http://www.fast.ai/2017/09/08/introducing-pytorch-for-fastai/)


### **Reference**  
This article on Medium towards data science group is a great summary on 7 reasons why the auther think [pytorch is great](https://towardsdatascience.com/pytorch-vs-tensorflow-spotting-the-difference-25c75777377b)

This [Serve Tensorflow Estimator with SavedModel Article](http://shzhangji.com/blog/2018/05/14/serve-tensorflow-estimator-with-savedmodel/) turn out to be very helpful!





### **Drafts**

Next 09-29-2018:

It will be useful to figure out how to load estimator and continue training.

--tbh, use session & graph instead of estimator will make all those much easier...OTZ
