# Dali/DDPM

<p align="center">
  <img src="https://github.com/user-attachments/assets/3d9a8ff5-be7d-4c28-ba42-ec89fe2aa031" alt="Image 1" width="400"/>
  <img src="https://github.com/user-attachments/assets/41036af9-98cd-4476-9435-74d196c32c35" alt="Image 2" width="400"/>
</p>


![Pasted image 20240816183120](https://github.com/user-attachments/assets/3d9a8ff5-be7d-4c28-ba42-ec89fe2aa031)

## Diffusion Models — Introduction
Diffusion Models are generative models, meaning that they are used to generate data similar to the data on which they are trained. Fundamentally, Diffusion Models work by destroying training data through the successive addition of Gaussian noise, and then learning to recover the data by reversing this noising process. After training, we can use the Diffusion Model to generate data by simply passing randomly sampled noise through the learned denoising process.
![image](https://github.com/user-attachments/assets/9d18359f-dea3-49ec-82de-6a4a15770b39)

Diffusion models are inspired by non-equilibrium thermodynamics. They define a Markov chain of diffusion steps to slowly add random noise to data and then learn to reverse the diffusion process to construct desired data samples from the noise. Unlike VAE or flow models, diffusion models are learned with a fixed procedure and the latent variable has high dimensionality (same as the original data).

Now get deeper into the diffusion models:
diffusion models consists of two processes as shown in the image below:

- Forward process (with red lines).
- Reverse process (with blue lines).


## Usage
run this command `python sd_gradio.py`



![Pasted image 20240818155133](https://github.com/user-attachments/assets/41036af9-98cd-4476-9435-74d196c32c35)





## Results:

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/83f8d84f-754c-49cb-ab33-73eaa66805d3" alt="output" width="200"/></td>
    <td><img src="https://github.com/user-attachments/assets/90104a77-db5b-4031-b91d-d4d89b78b764" alt="d" width="200"/></td>
    <td><img src="https://github.com/user-attachments/assets/24478566-b22e-41be-adcc-e77cd3d9dff9" alt="output_image" width="200"/></td>
    <td><img src="https://github.com/user-attachments/assets/26c059b3-7437-41ab-8307-3a7e4a3793f2" alt="s" width="200"/></td>
    <td><img src="https://github.com/user-attachments/assets/4cba0dfe-38c3-40c1-890d-f83559c49132" alt="test" width="200"/></td>
  </tr>
  <tr>
    <td><b>Prompt:</b> A cat stretching on the floor, highly detailed, ultra sharp, cinematic, 100mm lens, 8k resolution</td>
    <td><b>Prompt:</b> A dog reading a book, wearing glasses, comfy hat, highly detailed, ultra sharp, cinematic, 100mm lens, 8k resolution</td>
    <td><b>Prompt:</b> A dog stretching on the floor wearing sunglasses, looking to the camera, highly detailed, ultra sharp, cinematic, 100mm lens, 8k resolution</td>
    <td><b>Prompt:</b> An astronaut on the moon, highly detailed, ultra sharp, cinematic, 100mm lens, 8k resolution</td>
    <td><b>Prompt:</b> A black dog sitting between a bush and a pair of green pants standing up with nobody inside them, highly detailed, ultra sharp, cinematic, 100mm lens, 8k resolution</td>
  </tr>
</table>



---
```BibTex
@misc{ho2020denoising,
    title   = {Denoising Diffusion Probabilistic Models},
    author  = {Jonathan Ho and Ajay Jain and Pieter Abbeel},
    year    = {2020},
    eprint  = {2006.11239},
    archivePrefix = {arXiv},
    primaryClass = {cs.LG}
}

@misc{rombach2021highresolution,
      title={High-Resolution Image Synthesis with Latent Diffusion Models}, 
      author={Robin Rombach and Andreas Blattmann and Dominik Lorenz and Patrick Esser and Björn Ommer},
      year={2021},
      eprint={2112.10752},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}

@misc{https://doi.org/10.48550/arxiv.2204.11824,
  doi = {10.48550/ARXIV.2204.11824},
  url = {https://arxiv.org/abs/2204.11824},
  author = {Blattmann, Andreas and Rombach, Robin and Oktay, Kaan and Ommer, Björn},
  keywords = {Computer Vision and Pattern Recognition (cs.CV), FOS: Computer and information sciences, FOS: Computer and information sciences},
  title = {Retrieval-Augmented Diffusion Models},
  publisher = {arXiv},
  year = {2022},  
  copyright = {arXiv.org perpetual, non-exclusive license}
}
```
