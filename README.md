# RescueNet Dataset

## Overview

The escalating frequency and severity of natural disasters pose significant threats to human health, infrastructure, and ecosystems. The timely and accurate provision of information has the potential to revolutionize disaster management, particularly in accessing visual data for rapid response and recovery. Unmanned aerial systems (UAS) with affordable sensors offer opportunities to collect extensive high-resolution data, especially from inaccessible areas. However, the challenge lies in effectively analyzing these large datasets.

The [RescueNet](https://arxiv.org/abs/2202.12361) initiative contributes high-resolution UAS imagery with detailed classification, semantic segmentation, and visual question-answering annotations. This challenge will have several tracks including semi-supervised semantic segmentation and VQA.

 1. Track 1: Semi-Supervised Semantic Segmentation
 2. Track 2: Visual Question Answering

## Dataset Details

The data is collected with a small UAS platform, DJI Mavic Pro quadcopters, after Hurricane Michael.

For Track 1 ( Semi-supervised Classification and Semantic Segmentation),  in the training set, we have around 400 labeled images (~25% of the training set) and around 1050 unlabeled images (~75% of the training set ).

For Track 2 ( Supervised VQA), in the training set we have around 1450 images and there are a total 4511 image-question pairs.   


### Track 1

Semi-Supervised Semantic Segmentation: The semantic segmentation labels include: 1) Background, 2) Water, 3)Building No Damage, 4) Building Minor Damage, 5) Building Major Damage, 6) Building Total Destruction, 7) Road-Clear, 8) Road-Blocked, 9) Vehicle, 10) Tree, 11) Pool. Only a small portion of the training images have their corresponding masks available.

The dataset for Track 1 can be downloaded from this link: [https://drive.google.com/drive/folders/1Gv7fr5YiIkNrEdVKMiIIKugTxuB6dHQH?usp=sharing](https://drive.google.com/drive/folders/1Gv7fr5YiIkNrEdVKMiIIKugTxuB6dHQH?usp=sharing)

### Track 2

For the Visual Question Answering (VQA) task, we will provide QA pairs. These questions can be divided into the 9 categories: Simple Counting (SC), Complex Counting (CC), Building Condition Recognition (BCR), Road Condition Recognition (RCR), Level of Damage (LOD), Risk Assessment (RA), Density Estimation (DE), Positional (POS) and Change Detection (CD).

  1. In Simple Counting, we mainly ask to count the objects within the images regardless of attributes. For example, “How many buildings are in the image?”.
  
  2. In Complex Counting, attribute-based counting questions will be asked. “How many majorly damaged structures are seen in the images?”.
  
  3. In Building Condition Recognition, we ask questions to identify whether there is any building present for a given attribute. “Are there any structures that have been destroyed completely by the disaster?” is an example of this question category.
  
  4. In Road Condition Recognition, we consider comprehending the road condition by asking questions. ”What is the condition of the road?”, “Is any part of the road undamaged in this scene?”.
  
  5. In Level of Damage, we ask questions to identify the overall level of damage in a scene. “How badly damaged is the scene?” is an example.
  
  6. In Risk Assessment, we evaluate the risk due to the damages. “Does the recovery action need to be taken urgently?” is an example of a question for this category.
  
  7. In the Density Estimation question category, we estimate the density of buildings in a given scene. This category includes questions such as “How dense is the area?”.
  
  8. Dataset includes the Positional question category for which high-level scene understanding is necessary. “How much damage does the largest building in this image have?”, and “What is the damage status of the smallest building in this image?” are examples.
  
  9. In Change Detection, we identify whether there is a change in the number of buildings before and after the disaster due to the total number of destroyed buildings. “Is there any change in the number of buildings after the disaster on the scene?”.

The dataset for Track 2 can be downloaded from this link: [https://drive.google.com/drive/folders/1_BOY2AaHLkQWoN8ZjQ0kjHnDKp0YTMjZ?usp=sharing](https://drive.google.com/drive/folders/1_BOY2AaHLkQWoN8ZjQ0kjHnDKp0YTMjZ?usp=sharing)

### Paper Link
The Segmentation paper can be downloaded from this [link](https://arxiv.org/abs/2202.12361) and VQA paper from this [link](https://ieeexplore.ieee.org/document/10281747)
Please cite our paper when using the dataset

 ```
@article{chowdhury2022rescuenet,
  title={RescueNet: A High Resolution UAV Semantic Segmentation Benchmark Dataset for Natural Disaster Damage Assessment},
  author={Rahnemoonfar, Maryam and Chowdhury, Tashnim and Murphy, Robin},
  journal={arXiv preprint arXiv:2202.12361},
  year={2023}
}

@inproceedings{10281747,
  author={Sarkar, Argho and Rahnemoonfar, Maryam},
  booktitle={IGARSS 2023 - 2023 IEEE International Geoscience and Remote Sensing Symposium}, 
  title={RESCUENet-VQA: A Large-Scale Visual Question Answering Benchmark for Damage Assessment}, 
  year={2023},
  volume={},
  number={},
  pages={1150-1153},
  doi={10.1109/IGARSS52108.2023.10281747}
}

```
