# DISCLAMER: THIS SOFTWARE SUPPOSE TO BE USED AS AUXILIARY ART TOOL FOR CONTENT CREATORS. IT'S NOT INTENDED TO BELITTLE, OFFENCE, ETC ANY INDIVIDUAL, RACE, NATIONALITY, ETC.


Being fascinated by neural networks, I naturally dug into insides and found some interesting things.   

First, here a notebook for [image generation](https://colab.research.google.com/github/dobrosketchkun/latent_space_adventures/blob/main/files/Image_generation_styleGAN2_ada_pythorch.ipynb) from neural networks from my [network zoo](https://github.com/dobrosketchkun/wd_network_zoo)

Using [projection notebook](https://colab.research.google.com/github/dobrosketchkun/latent_space_adventures/blob/main/files/Latent_space_projection_styleGAN2_ada_pytorch.ipynb) you can project an image (thanks to project.py from the original [styleGAN2-ada-pytorch](https://github.com/NVlabs/stylegan2-ada-pytorch) repository, though results are often subpar (unless you try to project an image from FFHQ), but we can salvage this) and after that extract the state vector and use it on other similarly trained neural networks. Why do you want to do this? Well, let say you big fun of one particular person and you want for some reason change something in they appearence.

![Harold project](https://raw.githubusercontent.com/dobrosketchkun/latent_space_adventures/main/files/harold_proj.jpg)

You, of course, can save the state vector of any of the results in .npz file.

If you want more control, I have you covered. In [tweaking notebook](https://colab.research.google.com/github/dobrosketchkun/latent_space_adventures/blob/main/files/Latent_space_tweaking_styleGAN2_ada_pytorch.ipynb) you can use your npz file or start over to:

* Tweak randomly a face of a person

![Harold small](https://raw.githubusercontent.com/dobrosketchkun/latent_space_adventures/main/files/harold_small.jpg)

* Use a style of the original image and faces from random seeds

![Harold seeds](https://raw.githubusercontent.com/dobrosketchkun/latent_space_adventures/main/files/harold_seeds.jpg)

* Or you can apply styles from various seed onto your image 

![Harold styles](https://raw.githubusercontent.com/dobrosketchkun/latent_space_adventures/main/files/harold_styles.jpg)
