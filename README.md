# emotional-TTS - Pytorch Implementation
감정TTS

이 프로젝트는 Microsoft의 [**FastSpeech 2(Y. Ren et. al., 2020)**](https://arxiv.org/abs/2006.04558)와 NCSOFT의 [**VocGAN()**](https://arxiv.org/), [**GST(Wang, Yuxuan, et al.)**](https://arxiv.org/abs/1803.09017)로 모델을 구성해 감정 TTS 모델을 구축하고 [**Korean Single Speech dataset (이하 KSS dataset)**](https://www.kaggle.com/bryanpark/korean-single-speaker-speech-dataset)에서 동작하도록 구현한 것.

본 프로젝트에서는 아래와 같은 contribution을 제공함.
* kss dataset에 대해 동작하게 만든 소스코드
* Montreal Forced Aligner로부터 추출한 kss dataset의 text-utterance duration 정보 (TextGrid)
* kss dataset에 대해 학습한 FastSpeech2(Text-to-melspectrogram network) pretrained model
* FastSpeech2에 GST layer가 합쳐진 acoustic model
* kss dataset에 대해 학습한 [VocGAN](https://arxiv.org/pdf/2007.15256.pdf)(Neural vocoder)의 pretrained model

프로젝트 상세 기술
https://www.notion.so/deepdaiv/TTS-9934df955ee84a78988c5f20ef56ca6b?pvs=4

# References
- [FastSpeech 2: Fast and High-Quality End-to-End Text to Speech](https://arxiv.org/abs/2006.04558), Y. Ren, *et al*.
- [FastSpeech: Fast, Robust and Controllable Text to Speech](https://arxiv.org/abs/1905.09263), Y. Ren, *et al*.
- [Jackson Kang's Korean-FastSpeech2-Pytorch](https://github.com/HGU-DLLAB/Korean-FastSpeech2-Pytorch)
- [foamliu's GST-Tacotron-Korean](https://github.com/foamliu/GST-Tacotron-Korean)
- [rishikksh20's VocGAN implementation](https://github.com/rishikksh20/VocGAN)
