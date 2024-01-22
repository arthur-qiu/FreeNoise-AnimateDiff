# FreeNoise-AnimateDiff

This repository is the official implementation of [FreeNoise](https://arxiv.org/abs/2310.15169) in [AnimateDiff](https://arxiv.org/abs/2307.04725).

**[FreeNoise: Tuning-Free Longer Video Diffusion via Noise Rescheduling](https://arxiv.org/abs/2310.15169)**
</br>
Haonan Qiu,
Menghan Xia*,
Yong Zhang,
Yingqing He,
Xintao Wang,
Ying Shan,
Ziwei Liu*  
(*Corresponding Author)

**[AnimateDiff: Animate Your Personalized Text-to-Image Diffusion Models without Specific Tuning](https://arxiv.org/abs/2307.04725)**
</br>
Yuwei Guo,
Ceyuan Yang*,
Anyi Rao,
Yaohui Wang,
Yu Qiao,
Dahua Lin,
Bo Dai  
(*Corresponding Author)
</br>
</br>

<div align="center">
<img src=__assets__/animations/sample5_wo.gif>
<p>w/o Noise Rescheduling</p>

<img src=__assets__/animations/sample5.gif>
<p>w Noise Rescheduling</p>
</div>

## Run

Set up following the codebase [AnimateDiff](https://github.com/guoyww/AnimateDiff). Currently do not support the MotionLoRA.
```bash
  python scripts/animate.py
```

## BibTeX
```
@misc{qiu2023freenoise,
      title={FreeNoise: Tuning-Free Longer Video Diffusion Via Noise Rescheduling}, 
      author={Haonan Qiu and Menghan Xia and Yong Zhang and Yingqing He and Xintao Wang and Ying Shan and Ziwei Liu},
      year={2023},
      eprint={2310.15169},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```

```
@article{guo2023animatediff,
      title={AnimateDiff: Animate Your Personalized Text-to-Image Diffusion Models without Specific Tuning},
      author={Guo, Yuwei and Yang, Ceyuan and Rao, Anyi and Wang, Yaohui and Qiao, Yu and Lin, Dahua and Dai, Bo},
      journal={arXiv preprint arXiv:2307.04725},
      year={2023}
}
```

## Disclaimer
This project is released for academic use. We disclaim responsibility for user-generated content. Users are solely liable for their actions. The project contributors are not legally affiliated with, nor accountable for, users' behaviors. Use the generative model responsibly, adhering to ethical and legal standards.

## Support For Other Models
FreeNoise is supposed to work on other similar frameworks. An easy way to test compatibility is by shuffling the noise to see whether a new similar video can be generated (set eta to 0). If your have any questions about applying FreeNoise to other frameworks, feel free to contact [Haonan Qiu](http://haonanqiu.com/).

Current official implementation: [FreeNoise-VideoCrafter](https://github.com/AILab-CVC/FreeNoise), [FreeNoise-AnimateDiff](https://github.com/arthur-qiu/FreeNoise-AnimateDiff), [FreeNoise-LaVie](https://github.com/arthur-qiu/FreeNoise-LaVie) 

## Acknowledgements
Codebase built upon [AnimateDiff](https://github.com/guoyww/AnimateDiff).
