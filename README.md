# DRE7053 Generative Models
## Department of Data Science and Analytics - BI Norwegian Business School

Repository for the DRE7053 Generative Models course, where you can find all the course material.

**Note:** The course will be offered for the first time in the NORA Summer School 2024 at UiA. 

## Reading Material 
* Probabilistic Graphical Models
  - Directed Graphical Models [11] 
* Variational Inference 
  - Latent Variable Models
  - Variational Inference [1,2]
  - Deriving the Evidence Lower Bound [3,11]
* Variational Autoencoder [3]
  - Amortized Inference [2]
  - Reparameterization Trick [3,11]
* Should we optimize the ELBO?
  - Bound on Mutual Information [4,5,10]
  - Posterior Collapse [5,6]
* Multimodal Learning
  - Multimodal VAEs [7,8,9,10,20]
  - Product and Mixture of Experts [7,8,9]
  - Cross-Modal Generation [7,8,9,10,20]
  - Consensus of Dependent Distributions [20]
* Clustering with VAEs [12,19]
* Semi-supervised Learning [13,14]
* Diffusion Models [15,16,17,18]

## Papers
* [1] [Variational Inference: A Review for Statisticians](https://arxiv.org/abs/1601.00670)
* [2] [:fire: Advances in Variational Inference :fire:](https://arxiv.org/abs/1711.05597)
* [3] [:fire: Auto-Encoding Variational Bayes :fire:](https://arxiv.org/abs/1312.6114)
* [4] [:fire: ELBO surgery: yet another way to carve up the variational evidece lower bound :fire:](https://www.cs.columbia.edu/~blei/fogm/2020F/readings/HoffmanJohnson2016.pdf)
* [5] [Avoiding Latent Variables Collapse with Generative Skip Models](https://arxiv.org/abs/1807.04863)
* [6] [Don't Blame the ELBO! A Linear VAE Perspective on Posterior Collapse](https://arxiv.org/abs/1911.02469)
* [7] [:fire: Multimodal Generative Models for Scalable Weakly-Supervised Learning :fire:](https://arxiv.org/abs/1802.05335)
* [8] [Variational Mixture-of-Experts Autoencoders for Multi-Modal Deep Generative Models](https://arxiv.org/abs/1911.03393)
* [9] [:fire: Generalized Multimodal ELBO :fire:](https://arxiv.org/abs/2105.02470)
* [10] [Discriminative multimodal learning via conditional priors in generative models](https://doi.org/10.1016/j.neunet.2023.10.048)
* [11] [Deep Generative Models in Credit Scoring](https://munin.uit.no/handle/10037/20407)
* [12] [Variational Deep Embedding](https://arxiv.org/abs/1611.05148)
* [13] [:fire: Semi-supervised Learning with Deep Generative Models :fire:](https://arxiv.org/abs/1406.5298)
* [14] [Deep Generative Models for Reject Inference in Credit Scoring](https://www.sciencedirect.com/science/article/pii/S0950705120301660)
* [15] [Deep Unsupervised Learning using Nonequilibrium Thermodynamics](https://arxiv.org/abs/1503.03585)
* [16] [:fire: Denoising Diffusion Probabilistic Models :fire:](https://arxiv.org/abs/2006.11239)
* [17] [Denoising diffusion implicit models](https://arxiv.org/abs/2010.02502)
* [18] [Improved denoising diffusion probabilistic models](https://arxiv.org/abs/2102.09672)
* [19] [Deep variational incomplete multi-view clustering: exploring shared clustering structures](https://ojs.aaai.org/index.php/AAAI/article/view/29548)
* [20] [Aggregation of Dependent Expert Distributions in Multimodal Variational Autoencoders](https://arxiv.org/abs/2505.01134)

## Tutorials
* [1] [VAEs](https://jaan.io/what-is-variational-autoencoder-vae-tutorial/)
* [2] [ELBOs](https://yugeten.github.io/posts/2020/06/elbo/)
* [3] [Diffusion Models](https://github.com/FilippoMB/Diffusion_models_tutorial)

## Usage
You can run the codes in the folder `python` directly from `Google Colab` (make sure your session uses a GPU) as follows
```python
# download right version of tf (still using keras 2)
!pip install tensorflow==2.15.0 &> /dev/null
!pip install tensorflow-probability[tensorflow]==0.23 &> /dev/null

# clone repository
!git clone https://github.com/BI-DS/DRE7053.git

# move to right folder and create output folder
%cd DRE7053
!mkdir output
%cd python

# train VAE
!python ./train_VAE_prob.py --epochs 3
```

## Evaluation 
* Individual paper, limited to 8 content pages
* Pass/fail
* Ideas for the paper: 
  - Replicate a previous work with your own data and problem setting 
  - Propose a new idea/model, related to your own research, clearly stating the research question(s), method(s) (including the derivation of the ELBO), and experimental design
