<div align="center">

<h1>Control Color: Multimodal Diffusion-based Interactive Image Colorization</h1>

<div>
    <a href='https://zhexinliang.github.io/' target='_blank'>Zhexin Liang</a>&emsp;
    <a href='https://www.linkedin.com/in/zhaochen-li/' target='_blank'>Zhaochen Li</a>&emsp;
    <a href='https://shangchenzhou.com/' target='_blank'>Shangchen Zhou</a>&emsp;
    <a href='https://li-chongyi.github.io/' target='_blank'>Chongyi Li</a>&emsp;
    <a href='https://www.mmlab-ntu.com/person/ccloy/' target='_blank'>Chen Change Loy</a>
</div>
<div>
    S-Lab, Nanyang Technological University&emsp; 
</div>

<!-- <div>
    :star: <strong>Accepted to ICCV 2023, Oral</strong>
</div> -->
<!-- <div>
    <h4 align="center">
        <a href="https://zhexinliang.github.io/Control_Color/" target='_blank'>[Project Page]</a> •
        <a href="https://arxiv.org/abs/2303.17569" target='_blank'>[arXiv]</a> •
        <a href="https://youtu.be/tSCwA-srl8Q" target='_blank'>[Demo Video]</a>
        <img src="https://api.infinitescript.com/badgen/count?name=sczhou/Control_Color&ltext=Visitors&color=3977dd">
    </h4>
</div> -->

<div>
    <h4 align="center">
        <a href="https://zhexinliang.github.io/Control_Color/" target='_blank'>
        <img src="https://img.shields.io/badge/🐳-Project%20Page-blue">
        </a>
         <a href="https://arxiv.org/abs/2402.10855" target='_blank'>
        <img src="https://img.shields.io/badge/arXiv-2402.10855-b31b1b.svg">
        </a> 
        <a href="https://youtu.be/tSCwA-srl8Q" target='_blank'>
        <img src="https://img.shields.io/badge/Demo%20Video-%23D11507.svg?logo=YouTube&logoColor=white">
        </a>
        <img src="https://api.infinitescript.com/badgen/count?name=sczhou/ControlColor&ltext=Visitors&color=3977dd">
    </h4>
</div>

<img src="assets/teaser_aligned.png" width="100%"/>

<strong>Control Color (CtrlColor) achieves highly controllable multimodal image colorization based on stable diffusion model.</strong>

</div>

<table>
<tr>
    <td><img src="assets/region.gif" width="100%"/></td>
    <td><img src="assets/iterative.gif" width="100%"/></td>
</tr>
<tr>
    <td align='center' width='46%'>Region colorization</td>
    <td align='center' width='54%'>Iterative editing</td>
    <!-- <td align='center' width='33%'></td> -->
<tr>
</table>

:open_book: For more visual results and applications of CtrlColor, go checkout our <a href="https://zhexinliang.github.io/Control_Color/" target="_blank">project page</a>.

---


<!-- <table>
<tr>
    <td><img src="assets/region.gif" width="100%"/></td>
    <td><img src="assets/iterative.gif" width="90%"/></td>
</tr>
<tr>
    <td align='center' width='50%'>Stroke-based Colorization</td>
    <td align='center' width='50%'>Iterative Editing based on same seed</td>
<tr>
</table> -->

<!-- <table>
<tr>
    <td><img src="assets/region.gif" width="100%"/></td>
    <td><img src="assets/region_cond.gif" width="100%"/></td>
</tr>
<tr>
    <td align='center' width='50%'>Text-based Colorization</td>
    <td align='center' width='50%'>Exemplar-based Colorization</td>
<tr>
</table> -->

## :mega: Updates
- **2024.12.16**: The test codes (gradio demo), colorization model checkpoint, and autoencoder checkpoint are now publicly available.

## :desktop_computer: Requirements

- required packages in `CtrlColor_environ.yaml`

```
# git clone this repository
git clone https://github.com/ZhexinLiang/Control-Color.git
cd Control_Color

# create new anaconda env and install python dependencies
conda env create -f CtrlColor_environ.yaml
conda activate CtrlColor
```

## :running_woman: Inference

### Prepare models:

Please download the checkpoints of both colorization model and vae from [[Google Drive](https://drive.google.com/drive/folders/1lgqstNwrMCzymowRsbGM-4hk0-7L-eOT?usp=sharing)] and put both checkpoints in `./pretrained_models` folder.

### Testing:

You can use the following cmd to run gradio demo:

```
python test.py
```
Then you will get our interactive interface as below:

<img src=".\assets\hf_demo1.png" width="100%">

## :love_you_gesture: Citation
If you find our work useful for your research, please consider citing the paper:
```
@article{liang2024control,
  title={Control Color: Multimodal Diffusion-based Interactive Image Colorization},
  author={Liang, Zhexin and Li, Zhaochen and Zhou, Shangchen and Li, Chongyi and Loy, Chen Change},
  journal={arXiv preprint arXiv:2402.10855},
  year={2024}
}
```

### Contact
If you have any questions, please feel free to reach out at `zhexinliang@gmail.com`. 

<!-- ## :newspaper_roll: License

Distributed under the S-Lab License. See `LICENSE` for more information.

## :raised_hands: Acknowledgements

This study is supported by NTU NAP, MOE AcRF Tier 2 (T2EP20221-0033), and under the RIE2020 Industry Alignment Fund – Industry Collaboration Projects (IAF-ICP) Funding Initiative, as well as cash and in-kind contribution from the industry partner(s).

This project is built on source codes shared by [Style -->
