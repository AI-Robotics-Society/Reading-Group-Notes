# VIDEO INSTANCE SEGMENTATION

* Started by Adobe for their work 

### Dataset Info 
* Each Sequence => Set of frames 
* **Constraint:** Temporal consistency is important 
* Tracking has to be done (same instance IDs across frames for different instances) 
* Each video – about 30 to 40 frames 

### Approaches 
* Tracking by Detection 
* Integral Approach 

**[VIS](https://arxiv.org/pdf/1905.04804.pdf) - This paper talks about Integrated approach**

![assets/img1.png](assets/img1.png)

### MaskTrack-RCNN
_MaskTrack-RCNN_ is an addition to _Mask-RCNN_.

_Mask-RCNN has 3 heads:_ 
* Classification 
* Bounding Box Regression 
* Binary Segmentation 

MaskTrack-RCNN adds 1 more head: 
* Tracking Head 

### Notes for tracking mechanism
_IOU Tracker_ for tracking can perform poorly in cases of occlusion (E.g. crowd of people). 

So, _Instance Consistency Similarity_ is used.
In the paper, they used _IOUTracker+_ which include the instance consistencies as mentioned above. 

![assets/img2.png](assets/img2.png)

 
## Other Related Papers:
* [Classifying, Segmenting, and Tracking Object Instances in Video with Mask Propagation](https://arxiv.org/pdf/1912.04573.pdf) 
* [TubeTK: Adopting Tubes to Track Multi-Object in a One-Step Training Model](https://arxiv.org/pdf/2006.05683.pdf) 
* [STEm-Seg: Spatio-temporal Embeddings for Instance Segmentation in Videos](https://arxiv.org/pdf/2003.08429.pdf) 
* [SipMask: Spatial Information Preservation for Fast Image and Video Instance Segmentation](https://arxiv.org/pdf/2007.14772.pdf)
