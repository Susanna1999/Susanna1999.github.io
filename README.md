# Cases-of-CIF-based-segmenter

We propose a Continuous Integrate-and-Fire (CIF)-based speech segmentation method for two-pass streaming E2E ASR. 
Compared with VAD, the CIF estimator reuses the large encoder of ASR and optimizes jointly with ASR, which has a stronger modeling ability.
In addition, the CIF participates in the generation of token embedding in Paraformer, so the weight can also reflect the decoder's dependence on acoustic information contained in each frame. 
Continuous zero appearing in the CIF weight will be segmented. 
Furthermore, convolutional processing is adopted to detect the middle of the silent segment. 

Here are some cases of real audio segmentation. 
The gray background is the waveform of the audio, and the region where the waveform tends to the horizontal line represents the silence. 
The green dotted line is the token boundary predicted by CIF, and the red dotted line represents the segment boundary by the CIF-frame-300ms segmenter.
The corresponding audio is available under the wave/ folder.

![Case1](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/05d810ff-4df3-47e1-a2b2-f47995d0243f_01_29.png)
![Case2](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/05d810ff-4df3-47e1-a2b2-f47995d0243f_03_5.png)
![Case3](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/05d810ff-4df3-47e1-a2b2-f47995d0243f_05_28.png)
![Case4](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/05d810ff-4df3-47e1-a2b2-f47995d0243f_06_18.png)
![Case5](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/1d3362c2-10d1-4e7a-a34c-17e0ffc50e74_01_10.png)
![Case6](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/1d3362c2-10d1-4e7a-a34c-17e0ffc50e74_01_26.png)
![Case7](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/1d3362c2-10d1-4e7a-a34c-17e0ffc50e74_02_19.png)
![Case8](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/4dd57583-bda4-4a55-b944-f91261a1bfd3_04_3.png)
![Case9](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/6bbef4d0-5f32-416f-8822-34fe0fe0b2e5_04_17.png)
![Case10](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/6bbef4d0-5f32-416f-8822-34fe0fe0b2e5_06_5.png)
![Case11](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/6bbef4d0-5f32-416f-8822-34fe0fe0b2e5_06_13.png)
![Case12](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/1d3362c2-10d1-4e7a-a34c-17e0ffc50e74_03_34.png)
![Case13](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/2ca5b9ad-03f0-4019-8ac3-af49573a80a2_04_12.png)
![Case14](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/f7ed1260-bc0e-4e8a-be6b-1c2eb25d2a4a_01_32.png)
![Case15](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/f7ed1260-bc0e-4e8a-be6b-1c2eb25d2a4a_03_17.png)
![Case16](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/f7ed1260-bc0e-4e8a-be6b-1c2eb25d2a4a_03_39.png)
![Case17](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/f7ed1260-bc0e-4e8a-be6b-1c2eb25d2a4a_04_1.png)
![Case18](https://raw.githubusercontent.com/Susanna1999/Cases-of-CIF-based-segmenter/main/figure/f7ed1260-bc0e-4e8a-be6b-1c2eb25d2a4a_04_2.png)
