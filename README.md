# ISHARA - Machine Learning
Hi, this is machine learning part of ISHARA application made by Capstone Team C241-PS358 ✨

# Table of Contents
- [Introduction](https://github.com/Obesifix-Bangkit-2023/Machine_Learning#machine-learning-team)
- [ML Team](https://github.com/Obesifix-Bangkit-2023/Machine_Learning#machine-learning-team)
- [What We Do?](https://github.com/Obesifix-Bangkit-2023/Machine_Learning#what-we-do)
- [What We Use?](https://github.com/Obesifix-Bangkit-2023/Machine_Learning#What-Packages-that-we-use-in-Google-Colab/Jupyter-Notebook)
- [Repositories](https://github.com/Obesifix-Bangkit-2023/Machine_Learning#repositories)
- [Image Classification Model](https://github.com/Obesifix-Bangkit-2023/Machine_Learning#image-classification-model)
- [Recommendation System](https://github.com/Obesifix-Bangkit-2023/Machine_Learning#recommendation-system)
- [Machine Learning Model](https://github.com/Obesifix-Bangkit-2023/Machine_Learning#endpoint#machine-learning-model)

# Machine Learning Team

|  Name | Bangkit ID | Contacts |
| ------------ | ------------ | ------------ |
| Yusraini Nurul Asra	 | M200D4KX2534 		 | [Github](https://github.com/yusrainiasraa) & [Linkedin](https://www.linkedin.com/in/yusrainiasraa/)  |
| Linaili Himmatus Suroyya	 | M200D4KX3108 		| [Github](https://github.com/linailisry) & [Linkedin](https://www.linkedin.com/in/linaili-himmatus-suroyya-a7a0b4212/) |
| Intan Meilyana	 | M200D4KX1861 		| [Github](https://github.com/itsmei24) & [Linkedin](https://www.linkedin.com/in/intanmeilyana/) |

# What We Do?
We are developing a BISINDO Hand-Sign Classification model which contains 26 alphabets.

# What Packages that we use in Google Colab/Jupyter Notebook?

|   Packages |                                
| :----------------: | 
|    Tensorflow |
|  Keras      |  
| Pandas |  
| Scikit-Learn |  
| Numpy |  
| Matplotlib |  

# Repositories

|   Learning Paths       |                                Link                                              |
| :----------------:     | :----------------------------------------------------------------:               |
|   Organization         |            [Github](https://github.com/ishara-bangkit-capstone-project)                    |
|  Machine Learning      |            [Github](https://github.com/ishara-bangkit-capstone-project/ishara-machine-learning )   |
|  Cloud Computing  |        [Github](https://github.com/ishara-bangkit-capstone-project/ishara-backend-api)        |
| Mobile Development     |            [Github](https://github.com/ishara-bangkit-capstone-project/ishara-mobile-app) |


# Machine Learning Model
First, we find dataset for both models. Then the data is being preprocessed, after that we built a sequential model using Tensorflow and Keras API. We use transfer learning MobileNetV2 for image classification.

Since the application is computer-vision based, it has some real-time detection issues where it will classify aplhabets even though there is no hand detected. We improve and resolve these issue by making 2 models, which is binary and multiclass. 

The binary model will detect whether there is a hand or not, then if there is a hand it goes to the multiclass model which contains 26 alphabets. 

# Datasets Link
- [Binary Model Dataset](https://drive.google.com/drive/folders/1-QVql2184LEP3PK6cxmAg2KpCFVmMzfH?usp=drive_link)
- [Multiclass Model Dataset](https://www.kaggle.com/datasets/agungmrf/indonesian-sign-language-bisindo)


# Binary Model
- [Notebook](https://drive.google.com/drive/folders/1-QVql2184LEP3PK6cxmAg2KpCFVmMzfH?usp=drive_link)
- [Model](https://github.com/ishara-bangkit-capstone-project/ishara-machine-learning/tree/main/fix/models/binary_model)

|   Model |
| :----------------: |
|   Transfer Learning : MobileNetV2     |
|  Input : image(224, 224)  |
| Total params: 3,570,753 |
| Trainable params: 1,312,769 |
| Non-trainable params: 2,257,984 |


# Multiclass Model
- [Notebook](https://drive.google.com/drive/folders/1-QVql2184LEP3PK6cxmAg2KpCFVmMzfH?usp=drive_link)
- [Model](https://github.com/ishara-bangkit-capstone-project/ishara-machine-learning/tree/main/fix/models/multiclass_model)

|   Model |
| :----------------: |
|   Transfer Learning : MobileNetV2     |
|  Input : image(224, 224)  |
| Output : 26 labels|
| Total params: 2,658,394 |
| Trainable params: 400,410 |
| Non-trainable params: 2,257984 |

# Model Inference
[Notebook Link](https://github.com/ishara-bangkit-capstone-project/ishara-machine-learning/blob/main/fix/notebooks/model_inference.ipynb)