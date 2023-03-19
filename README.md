# Project: Weakly supervised learning-- label noise and correction


### [Full Project Description](doc/project3_desc.md)

Term: Spring 2023

+ Team 2
+ Team members
	+ Hu, Liang lh3057@columbia.edu
	+ Pan, Xinming xp2203@columbia.edu
	+ Qi, Yi Xuan yq2339@columbia.edu
	+ Tao, Ranran rt2796@columbia.edu
	+ Xia, Weijie wx2281@columbia.edu
	+ Zhou, Sicheng sz3094@columbia.edu

+ Project summary: In this project, we built two predictive models for image classification with 50k images as the training dataset. Among them, 10k have clean labels while the rest of them have noisy labels. In addition to a baseline logistic model, we built a Convolution Neural Network model, treating all 50k labels as clean labels. Considering the lack of testing data, we split the data into 80% of the training set and 20% of the validation test. The model I achieves a validation accuracy of 21% with a running time of 103 seconds in 5 epochs. We further built another convolution neural network model based on model I, incorporating the weakly supervised learning method into it in order to solve the problem of the presence of noisy labels. We first trained a "label-correction" model using 10k images with clean labels given, and use this model to correct the labels for 40k images initially with noisy labels. Finally, we trained the final predictive model II using the corrected dataset. Compared to the model I, model II was implemented with a more sophisticated convolution neural network architecture in order to improve performance and accuracy. At the same time, several layers were added in order to avoid the risk of overfitting and ensure the balance between the running time cost and the complexity of the model. We split the data into 90% of the training set and 10% of the validation set. Ultimately, model II achieved a validation accuracy of 56% with a running time of about 1197 seconds. Overall, we believe that model II significantly outperforms the baseline model and the simpler convolution neural network model without the weakly supervised learning feature in terms of predictive accuracy. 
	

**Contribution statement**: ([default](doc/a_note_on_contributions.md)) All team members contributed equally in all stages of this project. All team members approve our work presented in this GitHub repository including this contributions statement. 

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
