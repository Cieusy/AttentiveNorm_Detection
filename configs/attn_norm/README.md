# Attentive Normalization
This repo contains the code and pretrained models for [AOGNets: Compositional Grammatical Architectures for Deep Learning
](https://arxiv.org/abs/1711.05847)(CVPR 2019) and [Attentive Normalization](https://arxiv.org/abs/1908.01259). The models are trained on COCO object detection and instance segmentation task with Mask-RCNN and Cascade-Mask-RCNN model. We replace the backbone with [our imagenet pretrained backbones](https://github.com/iVMCL/AOGNet-v2) and head normalization with our Attentive Normalization. The results and trained models could be found in the table below. 

```
@article{li2019attentive,
  title={Attentive Normalization},
  author={Li, Xilai and Sun, Wei and Wu, Tianfu},
  journal={arXiv preprint arXiv:1908.01259},
  year={2019}
}

@inproceedings{li2019aognets,
  title={AOGNets: Compositional Grammatical Architectures for Deep Learning},
  author={Li, Xilai and Song, Xi and Wu, Tianfu},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
  pages={6220--6230},
  year={2019}
}
```
## Getting Started

## Results and Models
Mask-RCNN
<table>
  <tr>
    <th>Architecture</th>
    <th>Backbone</th>
    <th>Head</th>
    <th>#Params</th>
    <th>box AP</th>
    <th>mask AP</th>
    <th>Download</th>
  </tr>
  <tr>
    <td rowspan="5">ResNet-50</td>
    <td>BN</td>
    <td>-</td>
    <td>45.71M</td>
    <td>39.2</td>
    <td>35.2</td>
    <td><a href="">Google Drive</a></td>
  </tr>
  <tr>
    <td>AN (w/ BN)</td>
    <td>-</td>
    <td>45.91M</td>
    <td>40.8</td>
    <td>36.4</td>
    <td><a href="">Google Drive</a></td>
  </tr>
    <tr>
    <td>*GN</td>
    <td>GN</td>
    <td>45.72M</td>
    <td>40.3</td>
    <td>35.7</td>
    <td>-</td>
  </tr>
    <tr>
    <td>*SN</td>
    <td>SN</td>
    <td>-</td>
    <td>41.0</td>
    <td>36.5</td>
    <td>-</td>
  </tr>
    <tr>
    <td>AN (w/ BN)</td>
    <td>AN (w/ GN)</td>
    <td>45.96M</td>
    <td>41.6</td>
    <td>37.4</td>
    <td><a href="">Google Drive</a></td>
  </tr>
  <tr>
    <td rowspan="4">ResNet-101</td>
    <td>BN</td>
    <td>-</td>
    <td>64.70M</td>
    <td>41.4</td>
    <td>36.8</td>
    <td><a href="">Google Drive</a></td>
  </tr>
  <tr>
    <td>AN (w/ BN)</td>
    <td>-</td>
    <td>65.15M</td>
    <td>43.1</td>
    <td>38.2</td>
    <td><a href="">Google Drive</a></td>
  </tr>
    <tr>
    <td>*GN</td>
    <td>GN</td>
    <td>64.71M</td>
    <td>41.8</td>
    <td>36.8</td>
    <td>-</td>
  </tr>
  <tr>
    <td>AN (w/ BN)</td>
    <td>AN (w/ GN)</td>
    <td>65.20M</td>
    <td>43.2</td>
    <td>38.8</td>
    <td><a href="">Google Drive</a></td>
  </tr>
  <tr>
    <td rowspan="3">AOGNet-12m</td>
    <td>BN</td>
    <td>-</td>
    <td>33.09M</td>
    <td>40.7</td>
    <td>36.4</td>
    <td><a href="">Google Drive</a></td>
  </tr>
  <tr>
    <td>AN (w/ BN)</td>
    <td>-</td>
    <td>33.21M</td>
    <td>42.0</td>
    <td>37.8</td>
    <td><a href="">Google Drive</a></td>
  </tr>
  <tr>
    <td>AN (w/ BN)</td>
    <td>AN (w/ GN)</td>
    <td>33.26M</td>
    <td>43.0</td>
    <td>38.7</td>
    <td><a href="">Google Drive</a></td>
  </tr>
  <tr>
    <td rowspan="3">AOGNet-40m</td>
    <td>BN</td>
    <td>-</td>
    <td>60.73M</td>
    <td>43.4</td>
    <td>38.5</td>
    <td><a href="">Google Drive</a></td>
  </tr>
  <tr>
    <td>AN (w/ BN)</td>
    <td>-</td>
    <td>60.97M</td>
    <td>44.1</td>
    <td>39.0</td>
    <td><a href="">Google Drive</a></td>
  </tr>
  <tr>
    <td>AN (w/ BN)</td>
    <td>AN (w/ GN)</td>
    <td>61.02M</td>
    <td>44.9</td>
    <td>40.2</td>
    <td><a href="">Google Drive</a></td>
  </tr>
</table>


Cascade Mask-RCNN

<table>
  <tr>
    <th>Architecture</th>
    <th>Backbone</th>
    <th>Head</th>
    <th>#Params</th>
    <th>box AP</th>
    <th>mask AP</th>
    <th>Download</th>
  </tr>
  <tr>
    <td rowspan="2">ResNet-101</td>
    <td>BN</td>
    <td>-</td>
    <td>96.32M</td>
    <td>44.4</td>
    <td>38.2</td>
    <td><a href="">Google Drive</a></td>
  </tr>
  <tr>
    <td>AN (w/ BN)</td>
    <td>-</td>
    <td>96.77M</td>
    <td>45.8</td>
    <td>39.6</td>
    <td><a href="">Google Drive</a></td>
  </tr>
  <tr>
    <td rowspan="2">AOGNet-40m</td>
    <td>BN</td>
    <td>-</td>
    <td>92.35M</td>
    <td>45.6</td>
    <td>39.3</td>
    <td><a href="">Google Drive</a></td>
  </tr>
  <tr>
    <td>AN (w/ BN)</td>
    <td>-</td>
    <td>92.58M</td>
    <td>46.5</td>
    <td>40.0</td>
    <td><a href="">Google Drive</a></td>
  </tr>
</table>