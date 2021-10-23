# PDAN
Implementation for the paper ["PDAN: Pyramid Dilated Attention Network for Action Detection"](https://openaccess.thecvf.com/content/WACV2021/html/Dai_PDAN_Pyramid_Dilated_Attention_Network_for_Action_Detection_WACV_2021_paper.html).

The code is tested in Python3.7 + PyTorch1.2 environment with one Tesla V100 GPU and the overall code framework is adapted from the [Superevent](https://github.com/piergiaj/super-events-cvpr18).

For training and testing this code, please download the Charades dataset from this [link](https://prior.allenai.org/projects/charades) and follow this [repository](https://github.com/piergiaj/pytorch-i3d) to extract the snippet-level I3D feature. The RGB-Pretrained PDAN can be downloaded via this [Link](https://mybox.inria.fr/f/9fa53012b2684cb588b5/?dl=1). If the I3D feature is well extracted, the pretrained RGB model should achieve ~ 23.8% per frame-mAP on Charades. Note that this mAP is computed by all the timesteps, while using the original setting (25 sampled version), the performance should be more than 24 %. 



If you find this work useful for your research, please cite our [paper](https://openaccess.thecvf.com/content/WACV2021/html/Dai_PDAN_Pyramid_Dilated_Attention_Network_for_Action_Detection_WACV_2021_paper.html):

    @InProceedings{Dai_2021_WACV,
        author    = {Dai, Rui and Das, Srijan and Minciullo, Luca and Garattoni, Lorenzo and Francesca, Gianpiero and Bremond, Francois},
        title     = {PDAN: Pyramid Dilated Attention Network for Action Detection},
        booktitle = {Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision (WACV)},
        month     = {January},
        year      = {2021},
        pages     = {2970-2979}
    }

Contact: rui.dai@inria.fr

