# (TMLR 2022) Modeling Object Dissimilarity for Deep Saliency Prediction 
[Transactions on Machine Learning Research]
Bahar Aydemir*, Deblina Bhattacharjee*, Tong Zhang, Seungryong Kim, Mathieu Salzmann and Sabine Süsstrunk
*Equal contribution

Code will be published soon. Thanks for your patience!

TMLR 2022 Paper:https://openreview.net/forum?id=NmTMc3uD1G
Project Page: https://ivrl.github.io/DisSal
![Figure Abstract](fig-abstract.png)
Overview of the proposed architecture. We use an object detector to extract object instances.
We then pass on these object features to calculate appearance dissimilarity (shown in orange), which results in a
dissimilarity score for each object instance. The object detection network also outputs a bounding box for each
object, which we use to calculate the normalized object size dissimilarity (shown in green) for each detection. We
then fuse (1) the encoded global saliency features resulting from the saliency encoder, (2) the object appearance
dissimilarity features, and (3) the normalized object size dissimilarity features. We train our saliency decoder on
this concatenated feature set. We supervise the training with a KLD loss between the predicted
saliency map and the ground-truth one
![Figure Method](fig-method.png)

1. Install pytorch,torchvision
2. Install apex
```
conda install -c conda-forge nvidia-apex 
```


##  Citation
If you find the code, data, or the models useful, please cite this paper:
```
  TBA
```
## License 
``` 
 [MIT License](https://choosealicense.com/licenses/mit/)
```
