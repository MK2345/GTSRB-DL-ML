## Traffic Sign Classification using Deep Learning and Machine Learning

This project uses the German Traffic Sign Recognition Benchmark (GTSRB), a large dataset of more than
50,000 traffic sign images in 43 classes. The GTSRB is widely used for evaluating machine learning
and computer vision algorithms in the context of traffic sign recognition.

You will find several SVM and CNN models I created in the master branch.



Below are some sample images of the dataset.

![gtsrbDatensatz](https://github.com/MK2345/GTSRB-DL-ML/assets/24621381/bcfce9d8-655d-4837-8be3-2791e8775f92)


### Class distribution:

The training dataset is imbalanced, with significant variations in the number of samples across different
traffic sign classes. This imbalance is an important characteristic of the GTSRB dataset and reflects the
real-world frequency of different traffic signs.

Key points about the class distribution:
1. Some classes are overrepresented with thousands of samples.
2. Other classes are underrepresented with only a few hundred samples.
3. This imbalance can affect model performance and requires careful consideration during training and evaluation.

To address this imbalance, I employed techniques such as using class weights and Data augmentation.

![stratified_distribution_39209_gtsrb](https://github.com/MK2345/GTSRB-DL-ML/assets/24621381/47592cfc-13ac-4c51-a170-40288825d2e6)

### Stratified Class Density Visualization (500 Images)
![plot_500](https://github.com/MK2345/GTSRB-DL-ML/assets/24621381/b4c90437-8c86-4cca-9812-7cb90bfb6acd)

### Stratified Class Density Visualization (whole dataset)
![plot_39209](https://github.com/MK2345/GTSRB-DL-ML/assets/24621381/0df62558-6641-41bc-8b1a-6f9e64779174)

### Histogram equalization

The pictures were taken under different weather conditions. The contrast of low-contrast images was increased by means of histogram equalization.

![GTSRB_Hist_eq](https://github.com/MK2345/GTSRB-DL-ML/assets/24621381/02700502-6f0c-4593-b31d-495c28f9d659)
![GTSRB_Hist_eq_v](https://github.com/MK2345/GTSRB-DL-ML/assets/24621381/5611f024-3e9b-4804-a4c7-5163580a99f2)

### HOG-Features

The SVMs were trained with HOG features of the images, among other things.

![GTSRB_HOG](https://github.com/MK2345/GTSRB-DL-ML/assets/24621381/19117e85-b5ee-4941-8c28-fb00ee86d7d1)


### Model Development and Optimization

Multiple SVM and CNN models were trained with varying amounts of training data to determine the threshold 
at which one model type outperforms the other. Additionally, to ensure optimal performance Grid Search was 
utilized for hyperparameter tuning of select models
  
