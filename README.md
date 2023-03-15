# Brain_Tumor_Class_DL
### Brain Tumor MRI Classification with Deep Learning 

Author: Franceschin Sarah, Grisi Caterina, Pozza Giacomo, Tonello Alessio, Viberti Andrea

#### Abstract 

In this notebook our group deals with the classification of brain tumors: abnormal masses of tissue, the growth of which exceeds and is uncoordinated with that of the normal tissues. During the last decades the medical field is facing a real IT revolution, big data is undermining our sanitary system; in addition to this, facing Covid19 pandemic, hospitals are running out of health care workers. In order to deal with these actual problems, Machine Learning algorithms have been developed to assure: enhancement of decision-making and operational skills, reduction of errors and saving of resources. Specifically, a Deep Learning approach is the most powerful tool. A lot of time has been spent to develop a precise and robust solution for the automatic classification of brain tumors. Nevertheless, due to high inter and intra shape, and contrast variations, it remains a challenging problem. To go over these issues, we applied a CNN to obtain a model whose trained weights make us possible to predict if there is a brain tumor or not. In case of positive result, we discriminate between three different types of tumor: glioma, meningioma and pituitary. Our original dataset is composed of MRI images and by now we can see there is no balance between class dimensions. At this point, it has been adopted a transfer learning approach: taking into account an already made up neural network and changing the very last layers with the aim of exploit the already set net to achieve our task.
The original network for this purpose is EfficientNetB0, which gives us especially high performance. For the purpose of assessing the good results coming from this method, our group adopted various ideas. First of all, we tried to solve our dataset’s issues: class imbalance as stated before; by visual inspection, the no tumor class is characterized by an high percentage of axial images. Besides, always concerning about the dataset (as usual in the biomedical domaine), it could be considered too poor, so we performed a data augmentation. In addition, we also exploit the Grad-CAM method, this for the sake of showing: why the model mis-classify some images; where the model focuses to accomplish the task. Thereupon, our group tried to enhance the original performance by applying the transfer learning approach using different pre trained networks, such as EfficientNetB2 and VGG16. In the first case, no significant improvements can be noticed, despite the increased number of trainable parameters, which leads us to avoid this strategy. In the second case, performances of the model can not achieve those obtained originally through EfficientNetB0, which can be justify taking into account the number of trainable parameters. Finally, as a means to provide a more accurate estimate of performance than a single run, performance is averaged over the 5 iterations typical of 5-fold cross validation, which confirmed the high performances originally view in the training procedure. As a bonus widget, our group tried to re-adapt the original model with the aim to classify the proposed images in two different classes: Tumor and No Tumor. Also in this case, the model shows very good performances.

With our investigations, we've verified that the performances of the network are not affected by the unbalance of the training set and that EfficientNetB0 could be considered an optimal network because realizes a trade-off between the complexity of the model and its accuracy. Moreover, by the implementation of the Grad-CAM algorithm, we had the opportunity to verify that the network succeed into focusing on regions where the tumor is present: we think that future improvements could be the expansion of it and perform localization.


### Notebook Link (kaggle)

- FIRST PART:  https://www.kaggle.com/code/sahfra/first-part-group-8/notebook

- SECOND PART: https://www.kaggle.com/code/caterinagrisi/second-part-group-8/notebook

- THIRD PART:  https://www.kaggle.com/code/alessiotonello/third-part-group-8/notebook



