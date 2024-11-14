# Research on Fire Classification and Detection Models Based on Deep Learning

Shenzhi Li, Biao Zhang, Shuanglin Zhao*, Peng Wang

___________

Abstract—This paper aims to address the early detection and identification of fires, proposing a deep learning-based fire classification and detection model named FireScene Identification and Classification Network, FICNet for short. The model analyzes the publicly available aerial imagery dataset from FlameVision to rapidly classify and detect wildfires. This paper provides a detailed introduction to the dataset, model construction, experimental procedures, and results, while also discussing the practical application value and future research directions of the model. The FlameVision dataset and the FICNet model have been publicly released at https://github.com/vzhb/FICNet .

![alt text](./FICNetNoFire.png)



![alt text](./FICNet_Model.jpg)

The FICNet model's network architecture consists of five layers:

  LAYER 1: Input layer, receiving 416x416 images.
  
  LAYER 2: Pre-trained layer, Utilizing the pre-trained ResNet50 model, excluding the top fully connected layer, and using average pooling to reduce the dimensionality of feature maps.
  
  LAYER 3: Global Average Pooling layer, Performing global average pooling to further reduce the dimensionality of feature maps, allowing them to be input to the fully connected layer.
  
  LAYER 4: Fully connected layer, A fully connected layer with softmax activation function, also known as the dense layer, used for the classification task. Here, it is assumed that there are two classes, but the number can be adjusted according to the needs.
  
  LAYER 5: Output layer, displaying the final classification results.

Citation
---------------------

**Please kindly cite the papers if this code is useful and helpful for your research.**

Shenzhi Li, Biao Zhang, Shuanglin Zhao, Peng Wang. Research on Fire Classification and Detection Models Based on Deep Learning. International Conferenge on Big Data and Data Mining, 2024, xx: yyyy. 

     @article{li2024cross,
     title={Research on Fire Classification and Detection Models Based on Deep Learning},
     author={Shenzhi Li, Biao Zhang, Shuanglin Zhao, Peng Wang},
     journal= International Conferenge on Big Data and Data Mining},
     volume={xxx},
     pages={yyyy},
     year={2024}
     }

System-specific notes
---------------------
Please refer to the file `requirements.txt` for the running environment of this code.

The FlameVision dataset can be downloaded from the following links:

Baiduyun: https://pan.baidu.com/s/1zwE-Y_AJYaLOMPkIzgTTug?pwd=qwer 

Acknowledgment
---------

This work was funded by Open Fund of Hunan Geological Disaster Monitoring Early Warning and Emergency Rescue Engineering Technology Research Center under (Grant No. hndzgczx202407); Hebei Key Laboratory of Resource and Environmental Disaster Mechanism and Risk Monitoring under (Grant No. FZ248201).

Contact Information:
--------------------

Shenzhi Li: lishenzhi@sues.edu.cn<br>
Shenzhi Li is with the City University of Macau, Macau, China and Hebei Key Laboratory of Resource and Environmental Disaster Mechanism and Risk Monitoring
 Sanhe, China.

Shuanglin Zhao*: zhaoshuanglin2024@163.com<br>
Shuanglin Zhao is with the Hunan Institute of Geological Disaster Investigation and Monitoring, Changsha, China.
