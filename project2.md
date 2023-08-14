# Chest X-ray Denoising Diffusion Probabilistic Model 

Implementation of [Denoising Diffusion Probabilistic Model](https://arxiv.org/abs/2006.11239) [1] for chest X-ray image generation.  
The dataset used for this project is an open dataset [2] and is available publicly on [Kaggle](https://www.kaggle.com/datasets/francismon/curated-covid19-chest-xray-dataset).

<img src="./assets/images/project2/diffusion_chest.png" width="600"/>

## Code

The code is available on [![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/hippolytemayard/chest-x-ray-generative-models)

## Dataset
For this project, we utilize an open dataset called the Curated COVID-19 Chest X-ray Dataset [2]. This dataset contains a collection of chest X-ray images, including those of patients with COVID-19, pneumonia, and other respiratory conditions. The dataset is publicly available on Kaggle, providing a rich and diverse set of chest X-ray images for training and evaluation.

## Implementation Details
We base our implementation on an existing PyTorch implementation of DDPM [3] (see [![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/lucidrains/denoising-diffusion-pytorch)). This implementation serves as a solid foundation for our project, allowing us to leverage the power of PyTorch and build upon the existing codebase. By adapting the original DDPM framework to the specific task of generating chest X-ray images, we can explore the potential of this model in the medical imaging domain.


## Methodology
The Denoising Diffusion Probabilistic Model operates by iteratively applying a series of diffusion steps to a noise vector, gradually transforming it into a realistic image. This process involves denoising the image at each step using a trainable denoiser network. The model is trained by maximizing the likelihood of the target images in the training dataset. By optimizing the model parameters, we can generate high-quality chest X-ray images that capture the characteristics of different respiratory conditions.

<img src="./assets/images/project2/generated-sample.png" width="600"/>

## Conclusion
In this project, we propose the implementation of a Denoising Diffusion Probabilistic Model for generating chest X-ray images. By leveraging the power of DDPM and the availability of the Curated COVID-19 Chest X-ray Dataset, we aim to generate realistic and diverse chest X-ray images that can aid in medical research, diagnosis, and education. Through rigorous evaluation and comparison with existing methods, we seek to demonstrate the effectiveness and potential of the DDPM framework in the medical imaging domain.

## References
[1] Ho, J., Chen, X., Srinivas, A., Duan, Y., Abbeel, P., & Arora, S. (2020). Denoising Diffusion Probabilistic Models. *arXiv preprint arXiv:2006.11239*.

[2] Curated COVID-19 Chest X-ray Dataset. [Online]. Available: [https://www.kaggle.com/datasets/francismon/curated-covid19-chest-xray-dataset](https://www.kaggle.com/datasets/francismon/curated-covid19-chest-xray-dataset).

[3] Lucidrains. (n.d.). Denoising Diffusion Probabilistic Model - PyTorch. *GitHub Repository*. [Online]. Available: [https://github.com/lucidrains/denoising-diffusion-pytorch](https://github.com/lucidrains/denoising-diffusion-pytorch).
