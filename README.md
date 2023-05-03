# Transfer Learning for Application Classification in Network Traffic Data

## Project Goals & Objectives
This project is aimed at classifying applications in 3 types of network traffic flows (regular; VPN; TOR). The purpose of this project is to investigate the effectiveness of transfer learning in the classification of application traffic when a model is applied to previously unseen data.

## Dataset Description
The dataset used in this project is an augmented labeled dataset which contains data from ISCX VPN-nonVPN traffic dataset (ISCX-VPN), ISCX Tor-nonTor dataset (ISCX-Tor) and a small packet capture (TAU). This dataset was introduced by T. Shapira and Y. Shavitt in  "FlowPic: A Generic Representation for Encrypted Traffic Classification and Applications Identification," in IEEE Transactions on Network and Service Management. 

Portion of the dataset used:

![image](https://user-images.githubusercontent.com/52237625/236002480-13fcb06e-fa1b-4f84-9546-1f0fd0ab1aeb.png)

## Project Structure
vpn_tor_classification.ipynb: Jupyter notebook containing the code for this project
README.md: This file providing information about the project

## Dependencies
This project requires the following Python libraries:
numpy
pandas
scikit-learn
tensorflow
matplotlib

## Usage
The notebook contains the code for the following:
Data preprocessing
Building and training a Naive Bayes model
Building and training a Feed Forward Neural Net model
Freezing initial layers
Evaluating model performance
Experiments to compare model performances

## Results
The best performing model achieved an accuracy of % on the original data and an accuracy of % on the new data. The F1 score was 0.65 on the original data and 0.3 on the new data. The experiments performed on transfer learning and pre-trained models provided insight into the limitations of transfer learning and the benefits of using a pre-trained model.

## Citations
Dataset:
T. Shapira and Y. Shavitt, "FlowPic: A Generic Representation for Encrypted Traffic Classification and Applications Identification," in IEEE Transactions on Network and Service Management, doi: 10.1109/TNSM.2021.3071441.

T. Shapira and Y. Shavitt, "FlowPic: Encrypted Internet Traffic Classification is as Easy as Image Recognition," IEEE INFOCOM 2019 - IEEE Conference on Computer Communications Workshops (INFOCOM WKSHPS), Paris, France, 2019, pp. 680-687.

Gerard Drapper Gil, Arash Habibi Lashkari, Mohammad Mamun, Ali A. Ghorbani, "Characterization of Encrypted and VPN Traffic Using Time-Related Features", In Proceedings of the 2nd International Conference on Information Systems Security and Privacy(ICISSP 2016) , pages 407-414, Rome, Italy.

Arash Habibi Lashkari, Gerard Draper-Gil, Mohammad Saiful Islam Mamun and Ali A. Ghorbani, "Characterization of Tor Traffic Using Time Based Features", In the proceeding of the 3rd International Conference on Information System Security and Privacy, SCITEPRESS, Porto, Portugal, 2017.
