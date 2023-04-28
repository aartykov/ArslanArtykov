---
title: A Light-Weight Latent Composer
summary: Developed a light-weight controllable diffusion model with composable conditions based on Latent Diffusion Model.
tags:
  - Deep Learning
date: '2016-04-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: Code
    url: https://github.com/aartykov/Latent-Composer-pytorch
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

For this project, I developed a lightweight version of the [Composer: Creative and Controllable Image Synthesis with Composable Conditions](https://arxiv.org/pdf/2302.09778.pdf) based on the Latent Diffusion Model. The model provides users with a high degree of control over the image generation process. To achieve this, the input image is decomposed into its representative factors, and a diffusion model is trained on these factors to enable recomposition of the image. During inference, the generation process can be easily controlled by conditioning on different intermediate representations. The decomposed factors represent an enormous design space, which results in highly diverse and rich image content.  

To make the proposed architecture lighter, I opted to work directly in the latent space rather than the pixel space, and drew on the general concept of the Latent Diffusion Model to do so. During training, input images undergo a process in the pixel space where they are decomposed into their representative factors, such as color histogram, depth map, and canny edge map. The input images are then encoded into the latent space using a fixed encoder network. The input latent vectors then undergo a forward diffusion process where small amounts of noise are incrementally added until pure Gaussian noise is obtained. At the same time, the intermediate representations are passed through a spatial resizing block to bring them to the same spatial size as the latent vectors. Additionally, text prompts are utilized as an additional conditioning factor. I followed the same conditioning strategy proposed in the original [paper](https://arxiv.org/pdf/2302.09778.pdf) by summing the intermediate factors and concatenating the resultant vector with the noise vector. The CLIP image embeddings and text embeddings are projected, concatenated, and sent to the cross-attention layers of the U-Net transformer. For more details, please refer to the [paper](https://arxiv.org/pdf/2302.09778.pdf).

Cras aliquam rhoncus ipsum, in hendrerit nunc mattis vitae. Duis vitae efficitur metus, ac tempus leo. Cras nec fringilla lacus. Quisque sit amet risus at ipsum pharetra commodo. Sed aliquam mauris at consequat eleifend. Praesent porta, augue sed viverra bibendum, neque ante euismod ante, in vehicula justo lorem ac eros. Suspendisse augue libero, venenatis eget tincidunt ut, malesuada at lorem. Donec vitae bibendum arcu. Aenean maximus nulla non pretium iaculis. Quisque imperdiet, nulla in pulvinar aliquet, velit quam ultrices quam, sit amet fringilla leo sem vel nunc. Mauris in lacinia lacus.

Suspendisse a tincidunt lacus. Curabitur at urna sagittis, dictum ante sit amet, euismod magna. Sed rutrum massa id tortor commodo, vitae elementum turpis tempus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean purus turpis, venenatis a ullamcorper nec, tincidunt et massa. Integer posuere quam rutrum arcu vehicula imperdiet. Mauris ullamcorper quam vitae purus congue, quis euismod magna eleifend. Vestibulum semper vel augue eget tincidunt. Fusce eget justo sodales, dapibus odio eu, ultrices lorem. Duis condimentum lorem id eros commodo, in facilisis mauris scelerisque. Morbi sed auctor leo. Nullam volutpat a lacus quis pharetra. Nulla congue rutrum magna a ornare.

Aliquam in turpis accumsan, malesuada nibh ut, hendrerit justo. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Quisque sed erat nec justo posuere suscipit. Donec ut efficitur arcu, in malesuada neque. Nunc dignissim nisl massa, id vulputate nunc pretium nec. Quisque eget urna in risus suscipit ultricies. Pellentesque odio odio, tincidunt in eleifend sed, posuere a diam. Nam gravida nisl convallis semper elementum. Morbi vitae felis faucibus, vulputate orci placerat, aliquet nisi. Aliquam erat volutpat. Maecenas sagittis pulvinar purus, sed porta quam laoreet at.

