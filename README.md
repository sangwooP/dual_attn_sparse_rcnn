# Dual Attension Sparse-RCNN

* Paper: [Dual-Attention Sparse R-CNN via Single ROI Transformer and Dynamic CBAM](https://ieeexplore.ieee.org/document/9954801)

# Install MMDetection and MS COCO2017
* follow installation [MMDetection](https://mmdetection.readthedocs.io/en/stable/get_started.html)

# Train
```
#single GPU
python tools/train.py configs/dual_attn_sparsercnn/dual_attn_sparsercnn_r50_fpn_1x_coco.py

#multi GPU
bash tools/dist_train.sh configs/dual_attn_sparsercnn/dual_attn_sparsercnn_r50_fpn_1x_coco.py 2
```

# Results

| Model                 | Backbone | parameters (M) | mAP  | config                                                                                                                                                   | download                                                                                                                                                                                                                                                                                                                  |
|-----------------------|----------|----------------|------|----------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Sparse-RCNN           | R-50-FPN | 106.1          | 37.9 | [config](https://github.com/open-mmlab/mmdetection/blob/master/configs/sparse_rcnn/sparse_rcnn_r50_fpn_1x_coco.py)                                       | [model](https://download.openmmlab.com/mmdetection/v2.0/sparse_rcnn/sparse_rcnn_r50_fpn_1x_coco/sparse_rcnn_r50_fpn_1x_coco_20201222_214453-dc79b137.pth) \| [log](https://download.openmmlab.com/mmdetection/v2.0/sparse_rcnn/sparse_rcnn_r50_fpn_1x_coco/sparse_rcnn_r50_fpn_1x_coco_20201222_214453-dc79b137.log.json) |
| Dual-Attn-Sparse-RCNN | R-50-FPN | 65.5           | 38.0 | [config](https://github.com/sangwooP/dual_attn_sparse_rcnn/blob/master/mmdetection/configs/dual_attn_sparsercnn/dual_attn_sparsercnn_r50_fpn_1x_coco.py) | [model](https://drive.google.com/file/d/1bLIzUP9eK1hksIket3fRvfbI8oBloscL/view?usp=sharing) \| [log](https://drive.google.com/file/d/1q1Ny8ZciT2zFGtl4C2F7klKOeIy4GKpg/view?usp=sharing)                                                                                                                                  |
