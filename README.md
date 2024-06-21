# ISHARA - Machine Learning
Hi, this is machine learning part of ISHARA application made by Capstone Team C241-PS358 ✨

# Repositories

|   Learning Paths       |                                Link                                              |
| :----------------:     | :----------------------------------------------------------------:               |
|   Organization         |            [Github](https://github.com/ishara-bangkit-capstone-project)                    |
|  Machine Learning      |            [Github](https://github.com/ishara-bangkit-capstone-project/ishara-machine-learning )   |
|  Cloud Computing  |        [Github](https://github.com/ishara-bangkit-capstone-project/ishara-backend-api)        |
| Mobile Development     |            [Github](https://github.com/ishara-bangkit-capstone-project/ishara-mobile-app) |


# Machine Learning Team

|  Name | Bangkit ID | Contacts |
| ------------ | ------------ | ------------ |
| Yusraini Nurul Asra	 | M200D4KX2534 		 | [Github](https://github.com/yusrainiasraa) & [Linkedin](https://www.linkedin.com/in/yusrainiasraa/)  |
| Linaili Himmatus Suroyya	 | M200D4KX3108 		| [Github](https://github.com/linailisry) & [Linkedin](https://www.linkedin.com/in/linaili-himmatus-suroyya-a7a0b4212/) |
| Intan Meilyana	 | M200D4KX1861 		| [Github](https://github.com/itsmei24) & [Linkedin](https://www.linkedin.com/in/intanmeilyana/) |

# What We Do?
We are developing a BISINDO Hand-Sign Classification Model which classifies 26 alphabets from A to Z.

# What Packages that we use in Google Colab? ![image](https://www.google.com/url?sa=i&url=https%3A%2F%2Fmedium.com%2Fpython4u%2Fgoogle-colab-%25E6%2595%2599%25E5%25AD%25B8-2-%25E5%25BB%25BA%25E7%25AB%258B%25E5%258F%258A%25E4%25BD%25BF%25E7%2594%25A8-colab-%25E7%25AD%2586%25E8%25A8%2598%25E6%259C%25AC%25E7%25B7%25A8%25E5%25AF%25AB-python-8b0d1a5b920d&psig=AOvVaw2kWGwaP7R-EnurcsqtGibK&ust=1719041004743000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCLjGiu6U7IYDFQAAAAAdAAAAABAY)

|   Packages |                                
| :----------------: | 
|    Tensorflow |
|  Keras      |  
| Pandas |  
| Scikit-Learn |  
| Numpy |  
| Matplotlib |  


# Machine Learning Model
First, we find dataset. Then the data is being preprocessed, after that we built a sequential model using Tensorflow and Keras API. We use transfer learning MobileNetV2 for image classification.

Since the application is computer-vision based, it has some real-time detection issues where it will classify alphabets even though there is no hand detected. We improve and solve these issue by making 2 models, which is binary and multiclass. 

The binary model will detect whether there is a hand or not, then if there is a hand it goes to the multiclass model and classify 26 alphabets. 

# Datasets Link
- [Binary Model Dataset](https://drive.google.com/drive/folders/1-QVql2184LEP3PK6cxmAg2KpCFVmMzfH?usp=drive_link)
- [Multiclass Model Dataset](https://www.kaggle.com/datasets/agungmrf/indonesian-sign-language-bisindo)


# Binary Model
- [Binary Model Notebook](https://github.com/ishara-bangkit-capstone-project/ishara-machine-learning/blob/main/fix/notebooks/binary_model.ipynb)
- [Binary Model](https://github.com/ishara-bangkit-capstone-project/ishara-machine-learning/tree/main/fix/models/binary_model)

|   Model |
| :----------------: |
|   Transfer Learning : MobileNetV2     |
|  Input : image(224, 224)  |
| Total params: 3,570,753 |
| Trainable params: 1,312,769 |
| Non-trainable params: 2,257,984 |


# Multiclass Model
- [Multiclass Model Notebook](https://github.com/ishara-bangkit-capstone-project/ishara-machine-learning/blob/main/fix/notebooks/multiclass_model.ipynb)
- [Multiclass Model](https://github.com/ishara-bangkit-capstone-project/ishara-machine-learning/tree/main/fix/models/multiclass_model)

|   Model |
| :----------------: |
|   Transfer Learning : MobileNetV2     |
|  Input : image(224, 224)  |
| Output : 26 labels|
| Total params: 2,658,394 |
| Trainable params: 400,410 |
| Non-trainable params: 2,257984 |

# Model Inference
The binary model will detect whether there is a hand or not, then if there is a hand it goes to the multiclass model which contains 26 alphabets. [Notebook Link](https://github.com/ishara-bangkit-capstone-project/ishara-machine-learning/blob/main/fix/notebooks/model_inference.ipynb)