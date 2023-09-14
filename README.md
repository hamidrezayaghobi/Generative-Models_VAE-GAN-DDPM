# VAE-GAN-DDPM

Welcome to the Image Generation repository! In this project, I've implemented three powerful generative models: Variational Autoencoder (VAE), Generative Adversarial Network (GAN), and Diffusion Probabilistic Models (DDPM). Using these models, I've generated captivating new images from the Fashion-MNIST dataset.
![Screenshot from 2023-09-14 21-07-01](https://github.com/hamidrezayaghobi/VAE-GAN-DDPM/assets/59170724/14d0ed6f-4147-4072-9440-8bba36cbf060) ,</br>


## Dataset
I've used the Fashion-MNIST dataset as the source of inspiration for generating new images. Fashion-MNIST is a collection of fashion items, making it an exciting choice for creative image generation.

## Variational Autoencoder (VAE)
VAE is a generative model consisting of an encoder network and a decoder network. The encoder maps the input data into a latent space, where probability distributions represent the data. A decoder network generates the output data from samples of the latent space.

VAE is trained using a variational inference approach, where the goal is to maximize the evidence lower bound (ELBO) of the log-likelihood of the data. The ELBO consists of the reconstruction loss, which measures how well the decoder can reconstruct the input data from the latent space, and the KL divergence between the prior (considered Gaussian) and posterior distributions over the latent space. The posterior distribution is usually considered Gaussian, and the encoder only tries to learn its mean and variance. Given the mean and the variance, one can use the reparameterization trick to sample from the encoder.
### Examples
Interpolated between two randomly chosen points in the latent space, and choose 10 equally distant latent points between the random points
![Screenshot from 2023-09-14 21-11-23](https://github.com/hamidrezayaghobi/VAE-GAN-DDPM/assets/59170724/eaaa14a6-ac02-4de1-ad11-07e34112305e)
![Screenshot from 2023-09-14 21-11-41](https://github.com/hamidrezayaghobi/VAE-GAN-DDPM/assets/59170724/44dcb400-cc09-4911-9f2f-b0928e6328d1)
![Screenshot from 2023-09-14 21-11-57](https://github.com/hamidrezayaghobi/VAE-GAN-DDPM/assets/59170724/7143e7ee-06e3-42b7-b437-1064474eaadd)


