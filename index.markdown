---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---


# Facetron: Multi-speaker Face-to-Speech Model based on Cross-modal Latent Representations



### Abstract 
---
In this paper, we propose an effective method to synthesize speaker-specific speech waveforms by conditioning on videos of an individual's face.
Using a generative adversarial network (GAN) with linguistic and speaker characteristic features as auxiliary conditions, our method directly converts face images into speech waveforms under an end-to-end training framework.
The linguistic features are extracted from lip movements using a lip-reading model, and the speaker characteristic features are predicted from face images using cross-modal learning with a pre-trained acoustic model.
Since these two features are uncorrelated and controlled independently, we can flexibly synthesize speech waveforms whose speaker characteristics vary depending on the input face images. Therefore, our method can be regarded as a multi-speaker face-to-speech waveform model.
We show the superiority of our proposed model over conventional methods in terms of both objective and subjective evaluation results. Specifically, we evaluate the performances of the linguistic feature and the speaker characteristic generation modules by measuring the accuracy of automatic speech recognition and automatic speaker/gender recognition tasks, respectively. We also evaluate the naturalness of the synthesized speech waveforms using a mean opinion score (MOS) test.



### Samples
---
#### Small dataset 
<iframe width="480" height="300" src="https://www.youtube.com/embed/bzYuJNijAfI" frameborder="0" allowfullscreen></iframe>


#### Large dataset - Seen speakers
<iframe width="480" height="300" src="https://www.youtube.com/embed/2iN6fR1soaM" frameborder="0" allowfullscreen></iframe>


#####  Large dataset - Unseen speakers
<iframe width="480" height="300" src="https://www.youtube.com/embed/GZJcvP1x8cw" frameborder="0" allowfullscreen></iframe>






