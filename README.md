# Dual Attension Sparse-RCNN

* Paper: [Dual-Attention Sparse R-CNN via Single ROI Transformer and Dynamic CBAM](https://ieeexplore.ieee.org/document/9954801)

# Install MMDetection and MS COCO2017
* follow installation [MMDetection](https://mmdetection.readthedocs.io/en/stable/get_started.html)

# Train
'''
#single GPU
python tools/train.py configs/dual_attn_sparsercnn/dual_attn_sparsercnn_r50_fpn_1x_coco.py

#multi GPU
bash tools/dist_train.sh configs/dual_attn_sparsercnn/dual_attn_sparsercnn_r50_fpn_1x_coco.py 2
'''
