---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---


# Facetron: A Multi-speaker Face-to-Speech Model Based on Cross-Modal Latent Representations
### Submitted to EUSIPCO 2023 (paper number: 1537)


## Abstract 
---

In this paper, we propose a multi-speaker face-to-speech waveform generation model that also works for unseen speaker conditions.

Using a generative adversarial network (GAN) with linguistic and speaker characteristic features as auxiliary conditions, our method directly converts face images into speech waveforms under an end-to-end training framework. The linguistic features are extracted from lip movements using a lip-reading model, and the speaker characteristic features are predicted from face images using crossmodal learning with a pre-trained acoustic model. Since these two features are uncorrelated and controlled independently, we can flexibly synthesize speech waveforms whose speaker characteristics vary depending on the input face images. 

We show the superiority of our proposed model over conventional methods in terms of objective and subjective evaluation results. Specifically, we evaluate the performances of linguistic features by measuring their accuracy on an automatic speech recognition task. In addition, we estimate speaker and gender similarity for multi-speaker and unseen conditions, respectively. We also evaluate the naturalness of the synthesized speech waveforms using a mean opinion score (MOS) test and non-intrusive objective speech quality assessment (NISQA).





<br />

## Small dataset
---
We trained our model using a small dataset consisting of **four speakers** (s1, s2, s4, s29).  
Although Lip2Wav samples show similar speech quality with Facetron, **pronunciation of Facetron samples is more correct** compared to all of previous models.

<br />

<head>
	<style>
		table{
			border-width : 1px;
			border-style : solid;
			border-collapse : collapse;
		}
		td{
			border-width : 1px;
			border-style : solid;
			text-align: center;
		}
	</style>
</head>

<table style="width: auto; table-layout: fixed; word-wrap: normal;" borded="1" border-collapse="collapse">
<tr>
    <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Speaker</strong></td>
    <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Silent video</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Reference</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Facetron (Ours)</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Lip2Wav</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Voc-based</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>GAN-based</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Text</strong></td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s1</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s1_pwwy2n_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s1_pwwy2n_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s1_pwwy2n_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s1_pwwy2n_lip2wav.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s1_pwwy2n_voc.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s1_pwwy2n_gan.webm' type='video/webm'></video></td>
	<td> place white with <br> y 2 now </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s2</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s2_lbid1n_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s2_lbid1n_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s2_lbid1n_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s2_lbid1n_lip2wav.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s2_lbid1n_voc.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s2_lbid1n_gan.webm' type='video/webm'></video></td>
	<td> lay blue in <br> d 1 now </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s4</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s4_bgbu1p_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s4_bgbu1p_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s4_bgbu1p_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s4_bgbu1p_lip2wav.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s4_bgbu1p_voc.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s4_bgbu1p_gan.webm' type='video/webm'></video></td>
	<td> bin green by <br> u 1 please </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s29</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s29_swir8p_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s29_swir8p_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s29_swir8p_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s29_swir8p_lip2wav.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s29_swir8p_voc.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/small/s29_swir8p_gan.webm' type='video/webm'></video></td>
	<td> set white in <br> r 8 please </td>
</tr>
</table>







<br />
## Large dataset - seen
---
Out of the 33 speakers in the full dataset, we set **four speakers (s1, s2, s4, s29) as unseen speakers** and excluded them from the training process.   
Samples below are from **seen speakers**.  
Facetron outperforms than Lip2Wav in terms of speaker similiarty, speech quality and accuracy.


<br />


<table style="width: auto; table-layout: fixed; word-wrap: normal;" borded="1" border-collapse="collapse">
<tr>
    <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Speaker</strong></td>
    <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Silent video</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Reference</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Facetron (Ours)</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Lip2Wav</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Text</strong></td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s5</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s5_braf6p_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s5_braf6p_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s5_braf6p_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s5_braf6p_lip2wav.webm' type='video/webm'></video></td>
	<td> bin red at <br> f 6 please </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s6</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s6_bgwn8s_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s6_bgwn8s_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s6_bgwn8s_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s6_bgwn8s_lip2wav.webm' type='video/webm'></video></td>
	<td> bin green with <br> n 8 soon </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s11</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s11_bwaf7a_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s11_bwaf7a_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s11_bwaf7a_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s11_bwaf7a_lip2wav.webm' type='video/webm'></video></td>
	<td> bin white at f <br> 7 again </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s14</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s14_bbbk9p_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s14_bbbk9p_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s14_bbbk9p_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s14_bbbk9p_lip2wav.webm' type='video/webm'></video></td>
	<td> bin blue by <br> k 9 please </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s15</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s15_bbbk6n_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s15_bbbk6n_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s15_bbbk6n_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s15_bbbk6n_lip2wav.webm' type='video/webm'></video></td>
	<td> bin blue by <br> k 6 now </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s23</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s23_bgws7a_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s23_bgws7a_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s23_bgws7a_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_seen/s23_bgws7a_lip2wav.webm' type='video/webm'></video></td>
	<td> bin green with <br> s 7 again </td>
</tr>
</table>





<br />
## Large dataset - unseen
---

Samples below are from **unseen speakers**.  
Facetron generates correct gender voice (male face with male voice / female face with female voice).   
Facetron maintains the speech quality for unseen speakers, which is not maintained in Lip2Wav.

<br />




<table style="width: auto; table-layout: fixed; word-wrap: normal;" borded="1" border-collapse="collapse">
<tr>
    <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Speaker</strong></td>
    <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Silent video</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Reference</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Facetron (Ours)</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Lip2Wav</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Text</strong></td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s1</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s1_lbwy7s_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s1_lbwy7s_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s1_lbwy7s_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s1_lbwy7s_lip2wav.webm' type='video/webm'></video></td>
	<td> lay blue with <br> y 7 soon </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s1</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s1_pgwr4n_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s1_pgwr4n_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s1_pgwr4n_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s1_pgwr4n_lip2wav.webm' type='video/webm'></video></td>
	<td> place green with <br> r 4 now </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s2</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s2_bwaa2a_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s2_bwaa2a_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s2_bwaa2a_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s2_bwaa2a_lip2wav.webm' type='video/webm'></video></td>
	<td> bin white at <br> a 2 again </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s2</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s2_sgii1n_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s2_sgii1n_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s2_sgii1n_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s2_sgii1n_lip2wav.webm' type='video/webm'></video></td>
	<td> set green in <br> i 1 now </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s4</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s4_bgwb3p_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s4_bgwb3p_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s4_bgwb3p_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s4_bgwb3p_lip2wav.webm' type='video/webm'></video></td>
	<td> bin green with <br> b 3 please </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s4</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s4_lwbz4a_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s4_lwbz4a_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s4_lwbz4a_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s4_lwbz4a_lip2wav.webm' type='video/webm'></video></td>
	<td> lay white by <br> z 4 again </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s29</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s29_bgiq6n_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s29_bgiq6n_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s29_bgiq6n_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s29_bgiq6n_lip2wav.webm' type='video/webm'></video></td>
	<td> bin green in <br> q 6 now </td>
</tr>
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>s29</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s29_pwiazn_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s29_pwiazn_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s29_pwiazn_facetron.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/large_unseen/s29_pwiazn_lip2wav.webm' type='video/webm'></video></td>
	<td> place white in <br> a 0 now </td>
</tr>
</table>



<br />

## Ablation study - disentanglement
---
Samples below show successful **disentanglement of linguistic and speaker identity features** in Facetron.  
They are synthesized using lip features and face embedding **from different speakers** on the large dataset scenario.  
Facetron models lip features from original lip movements (without speech) and estimates face embedding from a target face.  
Therefore, the synthesized speech should contain the same text with that of the reference speech and the voice should be able to match the target face.
<br />




<table style="width: auto; table-layout: fixed; word-wrap: normal;" borded="1" border-collapse="collapse">
<tr>
    <td style="column-width: 160px; padding-left: 10px; padding-right: 10px"><strong>Reference speech <br> with original face</strong></td>
	<td style="column-width: 160px; padding-left: 10px; padding-right: 10px"><strong>Target face</strong></td>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Synthesized speech <br> with target face</strong></td>
</tr>
<tr>
	<td><video controls style="width: 160px;"><source src='./assets/disentangle/s6_brwk8s.webm' type='video/webm'></video></td>
	<td><img src='./assets/disentangle/s6.png'></td>
	<td><audio controls><source src='./assets/disentangle/s6_brwk8s_syn.wav'></audio></td>
</tr>
<tr>
	<td><video controls style="width: 160px;"><source src='./assets/disentangle/s7_brwz3s.webm' type='video/webm'></video></td>
	<td><img src='./assets/disentangle/s7.png'></td>
	<td><audio controls><source src='./assets/disentangle/s7_brwz3s_syn.wav'></audio></td>
</tr>
<tr>
	<td><video controls style="width: 160px;"><source src='./assets/disentangle/s13_brwq8a.webm' type='video/webm'></video></td>
	<td><img src='./assets/disentangle/s13.png'></td>
	<td><audio controls><source src='./assets/disentangle/s13_brwq8a_syn.wav'></audio></td>
</tr>
<tr>
	<td><video controls style="width: 160px;"><source src='./assets/disentangle/s17_bbbj7s.webm' type='video/webm'></video></td>
	<td><img src='./assets/disentangle/s17.png'></td>
	<td><audio controls><source src='./assets/disentangle/s17_bbbj7s_syn.wav'></audio></td>
</tr>
<tr>
	<td><video controls style="width: 160px;"><source src='./assets/disentangle/s18_bgwf1a.webm' type='video/webm'></video></td>
	<td><img src='./assets/disentangle/s18.png'></td>
	<td><audio controls><source src='./assets/disentangle/s18_bgwf1a_syn.wav'></audio></td>
</tr>
<tr>
	<td><video controls style="width: 160px;"><source src='./assets/disentangle/s24_bgiy5a.webm' type='video/webm'></video></td>
	<td><img src='./assets/disentangle/s24.png'></td>
	<td><audio controls><source src='./assets/disentangle/s24_bgiy5a_syn.wav'></audio></td>
</tr>
</table>



<br />

## Ablation study - effect of cosine similarity (CS) loss 
---
We conducted ablation study to verify the effectiveness of CS loss.  
Facetron, which is trained with CS loss, produces **clearer and more intelligible speech samples for the predicted unseen speaker** compared to the model without CS loss.  
The samples from the model without CS loss show unclear pronunciation and poor sound quality because the generation process are not confined to a specific speaker's characteristic. 
<br />


<table style="width: auto; table-layout: fixed; word-wrap: normal;" borded="1" border-collapse="collapse">
<tr>
    <td style="column-width: 600px; padding-left: 10px; padding-right: 10px"><strong>Reference speech <br> with original face</strong></td>
	<td style="column-width: 600px; padding-left: 10px; padding-right: 10px"><strong>With CS loss (Facetron)</strong></td>
	<td style="column-width: 600px; padding-left: 10px; padding-right: 10px"><strong>Without CS loss</strong></td>
</tr>
<tr>
	<td><img src='./assets/ablations/reference/bwwu2p.PNG' ></td>
	<td><img src='./assets/ablations/with_CS/bwwu2p.PNG' ></td>
	<td><img src='./assets/ablations/without_CS/bwwu2p.PNG' ></td>
</tr>
<tr>
	<td><audio controls><source src='./assets/ablations/reference/s1_bwwu2p.wav'></audio></td>
	<td><audio controls><source src='./assets/ablations/with_CS/s1_bwwu2p_syn_00250000.wav'></audio></td>
	<td><audio controls><source src='./assets/ablations/without_CS/s1_bwwu2p_syn_00500000.wav'></audio></td>
</tr>
<tr>
	<td><img src='./assets/ablations/reference/lbwy7s.PNG' ></td>
	<td><img src='./assets/ablations/with_CS/lbwy7s.PNG' ></td>
	<td><img src='./assets/ablations/without_CS/lbwy7s.PNG' ></td>
</tr>
<tr>
	<td><audio controls><source src='./assets/ablations/reference/s1_lbwy7s.wav'></audio></td>
	<td><audio controls><source src='./assets/ablations/with_CS/s1_lbwy7s_syn_00250000.wav'></audio></td>
	<td><audio controls><source src='./assets/ablations/without_CS/s1_lbwy7s_syn_00500000.wav'></audio></td>
</tr>
<tr>
	<td><img src='./assets/ablations/reference/pwad3s.PNG' ></td>
	<td><img src='./assets/ablations/with_CS/pwad3s.PNG' ></td>
	<td><img src='./assets/ablations/without_CS/pwad3s.PNG' ></td>
</tr>
<tr>
	<td><audio controls><source src='./assets/ablations/reference/s1_pwad3s.wav'></audio></td>
	<td><audio controls><source src='./assets/ablations/with_CS/s1_pwad3s_syn_00250000.wav'></audio></td>
	<td><audio controls><source src='./assets/ablations/without_CS/s1_pwad3s_syn_00500000.wav'></audio></td>
</tr>
<tr>
	<td><img src='./assets/ablations/reference/sgwdzn.PNG' ></td>
	<td><img src='./assets/ablations/with_CS/sgwdzn.PNG' ></td>
	<td><img src='./assets/ablations/without_CS/sgwdzn.PNG' ></td>
</tr>
<tr>
	<td><audio controls><source src='./assets/ablations/reference/s1_sgwdzn.wav'></audio></td>
	<td><audio controls><source src='./assets/ablations/with_CS/s1_sgwdzn_syn_00250000.wav'></audio></td>
	<td><audio controls><source src='./assets/ablations/without_CS/s1_sgwdzn_syn_00500000.wav'></audio></td>
</tr>
</table>








