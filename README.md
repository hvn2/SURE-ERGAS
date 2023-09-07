# SURE-ERGAS
Pytorch codes for the paper "SURE-ERGAS: UNSUPERVISED DEEP LEARNING MULTISPECTRAL AND HYPERSPECTRAL IMAGE FUSION", in Proceeding of IEEE IGARSS 2023, Pasadena, USA, 15-22 July, 2023. <br>
**Authors:** Han V. Nguyen $^\ast \dagger$, Magnus O. Ulfarsson $^\ast$,  Johannes R. Sveinsson $^\ast$, and Mauro Dalla Mura $^\ddagger$ <br>
$^\ast$ Faculty of Electrical and Computer Engineering, University of Iceland, Reykjavik, Iceland<br>
$^\dagger$ Department of Electrical and Electronic Engineering, Nha Trang University, Khanh Hoa, Vietnam<br>
$^\ddagger$ GIPSA-Lab, Grenoble Institute of Technology, Saint Martin d’Hères, France.<br>
Email: hvn2@hi.is

## Abstract:<br>
This paper proposes a new loss function to train a convolutional neural network (CNN) for multispectral and hyperspectral (MS-HS) image fusion. The loss function is based on the relative dimensionless global error synthesis (ERGAS), where we exchange the mean squared error (MSE) for its unbiased estimate using Stein's risk unbiased estimate (SURE). The loss function has a good balance between the spectral and spatial information implied by the weighted MSE, therefore it does not need a parameter to balance the spectral and spatial terms as in MSE loss function, and it also converges faster than the MSE one. Additionally, the loss function enables unsupervised training and avoids overfitting, since it is derived by using SURE. Experimental results show that the proposed method yields good results and outperforms the competitive methods. 
<br><br>.
 **Please cite our paper if you are interested**<br>
 @inproceedings{nguyen2023sure-ergas,
  title={Hyperspectral Super-Resolution by Unsupervised Convolutional Neural Network and Sure},
  author={Nguyen, Han V and Ulfarsson, Magnus O and Sveinsson, Johannes R and Dalla Mura, Mauro},
  booktitle={IGARSS 2023-2023 IEEE International Geoscience and Remote Sensing Symposium},
  pages={0--0},
  year={2023},
  organization={IEEE}
}
## Usage:<br>
The following folders contanin:
- data: The simulated PU dataset.
- models: python scripts define the model (network structure)
- utils: additional functions<br>
**Run the jupyter notebook and see results.**
## Environment
- Pytorch 1.8
- Numpy, Scipy, Skimage.
- Matplotlib