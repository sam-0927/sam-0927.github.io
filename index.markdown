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

<br />

<br />

### Comparison with other models (seen speakers)

---

We compare our model (red box) with generated samples from <a href="https://wendison.github.io/VCVTS-demo/">https://wendison.github.io/VCVTS-demo/</a> (white box).

Because of different experiment setting, we should use samples with different script. 

(All samples in other models are seen script for our model)

<br />

#### S1

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
		}
	</style>
</head>
<table style="width: auto; table-layout: fixed; word-wrap: normal;" borded="1" border-collapse="collapse">
    <tr>
        <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong></strong></td>
        <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Silent video</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Reference</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>XTS</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Lip2Wav</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>VCVTS+PWG</strong></td>
		<td bgcolor="#FFCDD2" style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Silent video</strong></td>
		<td bgcolor="#FFCDD2" style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Reference</strong></td>
		<td bgcolor="#FFCDD2" style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Facetron (Ours)</strong></td>
	</tr>
    <!--1-->
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>1</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_bbas3a_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_bbas3a_gt.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_bbas3a_xts.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_bbas3a_lip2wav.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_bbas3a_prop_pwg.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s1_lwbf5a_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s1_lwbf5a_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s1_lwbf5a_facetron.webm' type='video/webm'></video></td>
</tr>
<!--2-->
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>2</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_pgwl1s_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_pgwl1s_gt.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_pgwl1s_xts.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_pgwl1s_lip2wav.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_pgwl1s_prop_pwg.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_ours/s1_bwwu1s_sil.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_ours/s1_bwwu1s_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s1_bwwu1s_facetron.webm' type='video/webm'></video></td>
</tr>
<!--3-->
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>3</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_swwi8n_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_swwi8n_gt.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_swwi8n_xts.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_swwi8n_lip2wav.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s1_swwi8n_prop_pwg.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s1_bgbu2n_sil.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_ours/s1_bgbu2n_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s1_bgbu2n_facetron.webm' type='video/webm'></video></td>
</tr>
</table>







<br />

#### S2

<br />



<table style="width: auto; table-layout: fixed; word-wrap: normal;" borded="1" border-collapse="collapse">
    <tr>
        <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong></strong></td>
        <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Silent video</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Reference</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>XTS</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Lip2Wav</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>VCVTS+PWG</strong></td>
		<td bgcolor="#FFCDD2" style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Silent video</strong></td>
		<td bgcolor="#FFCDD2" style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Reference</strong></td>
		<td bgcolor="#FFCDD2" style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Facetron (Ours)</strong></td>
	</tr>
    <!--1-->
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>1</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_bbil4a_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_bbil4a_gt.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_bbil4a_xts.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_bbil4a_lip2wav.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_bbil4a_prop_pwg.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s2_bbbs6a_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s2_bbbs6a_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s2_bbbs6a_facetron.webm' type='video/webm'></video></td>
</tr>
<!--2-->
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>2</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_lgwaza_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_lgwaza_gt.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_lgwaza_xts.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_lgwaza_lip2wav.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_lgwaza_prop_pwg.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_ours/s2_pgaq8a_sil.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_ours/s2_pgaq8a_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s2_pgaq8a_facetron.webm' type='video/webm'></video></td>
</tr>
<!--3-->
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>3</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_pwaj5n_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_pwaj5n_gt.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_pwaj5n_xts.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_pwaj5n_lip2wav.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s2_pwaj5n_prop_pwg.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s2_pwij1n_sil.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_ours/s2_pwij1n_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s2_pwij1n_facetron.webm' type='video/webm'></video></td>
</tr>
</table>





<br />

#### S4

<br />



<table style="width: auto; table-layout: fixed; word-wrap: normal;" borded="1" border-collapse="collapse">
    <tr>
        <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong></strong></td>
        <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Silent video</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Reference</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>XTS</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Lip2Wav</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>VCVTS+PWG</strong></td>
		<td bgcolor="#FFCDD2" style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Silent video</strong></td>
		<td bgcolor="#FFCDD2" style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Reference</strong></td>
		<td bgcolor="#FFCDD2" style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Facetron (Ours)</strong></td>
	</tr>
    <!--1-->
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>1</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_bbir6a_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_bbir6a_gt.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_bbir6a_xts.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_bbir6a_lip2wav.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_bbir6a_prop_pwg.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s4_bbie5n_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s4_bbie5n_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s4_bbie5n_facetron.webm' type='video/webm'></video></td>
</tr>
<!--2-->
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>2</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_pgad6s_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_pgad6s_gt.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_pgad6s_xts.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_pgad6s_lip2wav.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_pgad6s_prop_pwg.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_ours/s4_prwd2s_sil.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_ours/s4_prwd2s_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s4_prwd2s_facetron.webm' type='video/webm'></video></td>
</tr>
<!--3-->
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>3</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_swbb9p_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_swbb9p_gt.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_swbb9p_xts.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_swbb9p_lip2wav.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s4_swbb9p_prop_pwg.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s4_lbwr1p_sil.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_ours/s4_lbwr1p_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s4_lbwr1p_facetron.webm' type='video/webm'></video></td>
</tr>
</table>









<br />

#### S29

<br />





<table style="width: auto; table-layout: fixed; word-wrap: normal;" borded="1" border-collapse="collapse">
    <tr>
        <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong></strong></td>
        <td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Silent video</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Reference</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>XTS</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Lip2Wav</strong></td>
		<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>VCVTS+PWG</strong></td>
		<td bgcolor="#FFCDD2" style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Silent video</strong></td>
		<td bgcolor="#FFCDD2" style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Reference</strong></td>
		<td bgcolor="#FFCDD2" style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>Facetron (Ours)</strong></td>
	</tr>
    <!--1-->
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>1</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_bgak6n_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_bgak6n_gt.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_bgak6n_xts.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_bgak6n_lip2wav.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_bgak6n_prop_pwg.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s29_brax4p_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s29_brax4p_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s29_brax4p_facetron.webm' type='video/webm'></video></td>
</tr>
<!--2-->
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>2</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_lrbv1s_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_lrbv1s_gt.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_lrbv1s_xts.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_lrbv1s_lip2wav.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_lrbv1s_prop_pwg.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_ours/s29_bwby3s_sil.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_ours/s29_bwby3s_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s29_bwby3s_facetron.webm' type='video/webm'></video></td>
</tr>
<!--3-->
<tr>
	<td style="column-width: auto; padding-left: 10px; padding-right: 10px"><strong>3</strong></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_pgin7a_sil.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_pgin7a_gt.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_pgin7a_xts.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_pgin7a_lip2wav.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_vcvts/s29_pgin7a_prop_pwg.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s29_sbwe9s_sil.webm' type='video/webm'></video></td>
    <td><video controls style="width: 150px;"><source src='./assets/demo_ours/s29_sbwe9s_ref.webm' type='video/webm'></video></td>
	<td><video controls style="width: 150px;"><source src='./assets/demo_ours/s29_sbwe9s_facetron.webm' type='video/webm'></video></td>
</tr>
</table>





