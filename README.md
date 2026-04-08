MECSNet: A Dual-Encoder Multi-Scale Attention Network for Polyp Segmentation
This is the official implementation of the paper MECSNet: A Dual-Encoder Multi-Scale Attention Network for Polyp Segmentation.
The model proposes a dual encoder-decoder architecture fusing CNN and CAFormer, and designs the MECS module (Median-enhanced Spatial and Channel Attention) and integrates CoordAtt module, achieving state-of-the-art performance on mainstream polyp segmentation benchmark datasets.


📋 Overview
Core Innovations
Dual Encoder Architecture: Fuses CNN's local detail extraction capability with CAFormer's global feature modeling advantage, enhancing multi-scale semantic representation.
MECS Module: Integrates average/max/median pooling, multi-scale deep convolution and improved attention mechanism, boosting feature extraction robustness and anti-noise performance.
CoordAtt in Skip Connection: Enhances spatial position modeling, significantly improving the localization accuracy of polyp boundaries.
Superior Performance: Achieves 1.3% mDice and 1.8% mIoU improvement on Kvasir-SEG dataset compared with SOTA methods.
Experimental Results
The model is evaluated on 4 mainstream polyp segmentation datasets (Kvasir-SEG, CVC-ClinicDB, CVC-ColonDB, ETIS-LaribPolypDB), and outperforms existing methods in most metrics, especially for small targets and blurred boundary polyps.


🔧 Environment Configuration
Dependencies
Python 3.8+
TensorFlow (the paper uses TensorFlow for implementation)
CUDA & cuDNN (matching TensorFlow version)
NumPy, OpenCV-Python, Pillow, SciPy, TQDM
scikit-learn (for metric calculation)
