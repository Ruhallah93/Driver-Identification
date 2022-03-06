# Discrete Wavelet Transform for Generative Adversarial Network to Identify Drivers Using Gyroscope and Accelerometer Sensors.

### [Paper](https://ieeexplore.ieee.org/document/9716101)

[Rouhollah Ahmadian](https://homes.cs.washington.edu/~royorel/)<sup>1</sup> ,
[Mehdi Ghatee](https://aut.ac.ir/cv/2174/MEHDI-GHATEE?slc_lang=en&&cv=2174&mod=scv)<sup>1</sup>,
[Johan Wahlström](https://www.cs.ox.ac.uk/people/johan.wahlstrom/)<sup>2</sup><br>
<sup>1</sup>Amirkabir University of Technology, <sup>2</sup>University of Oxford

## Abstract

Driver identification is a central research area in intelligent transportation systems, with applications in commercial
freight transport and usage-based insurance. One way to perform the identification is to use smartphones as the main
sensor devices. After extracting features from smartphone-embedded sensors, various machine learning methods can be used
to identify the driver. However, the accuracy often degrades as the number of drivers increases. This paper uses a
Generative Adversarial Network (GAN) for data augmentation to obtain a driver identification algorithm that maintains
excellent performance also when the number of drivers increases. Since GAN diversifies the drivers’ data, it makes it
possible to apply the identification algorithm on a larger number of drivers without overfitting. Although GANs are
commonly used in image processing for image augmentation, their use for driving signal augmentation is novel. However,
GAN’s training on raw driving signals diverges. This challenge is solved by getting the Discrete Wavelet Transform (DWT)
on driving signals before feeding to GAN. Our experiments prove the usefulness of GAN model for generating driving
signals emanating from DWT on smartphones’ accelerometer and gyroscope signals. After collecting the augmented data,
their histograms along the overlapped windows are fed to machine learning methods covered by a Stacked Generalization
Method (SGM). The presented hybrid GAN-SGM approach identifies drivers with 97% accuracy, 98% precision, 97% recall, and
97% F1-measure that outperforms standard machine learning methods that utilize features extracted by the statistical,
spectral, and temporal approaches.

## Pre-Requisits

- To implement the algorithms, we used Scikit-learn version 0.22, Tensorflow version 1.13.2, and Keras version 2.3.0.
- A model selection for hyperparameter tuning is needed to achieve the best accuracy.

## Dataset

In this project, to evaluate the methods, the driving data of this [dataset] has been used.

## Citation

If you use this code for your research, please cite our paper.

```
@ARTICLE{9716101,
  author={Ahmadian, Rouhollah and Ghatee, Mehdi and Wahlström, Johan},
  journal={IEEE Sensors Journal}, 
  title={Discrete Wavelet Transform for Generative Adversarial Network to Identify Drivers Using Gyroscope and Accelerometer Sensors}, 
  year={2022},
  volume={},
  number={},
  pages={1-1},
  doi={10.1109/JSEN.2022.3152518}}
```

[dataset]: <https://github.com/mghatee/Overall-Driving-Behavior-Recognition-By-Smartphone>

[https://doi.org/10.1109/JSEN.2022.3152518]: <https://ieeexplore.ieee.org/document/9716101>
