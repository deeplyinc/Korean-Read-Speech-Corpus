# Deeply Korean Read Speech Corpus
---
## Summary
Pairs of Korean speakers reading a script with <u>*__3 distinct text sentiments (negative, neutral, positive)__*</u>, with <u>*__3 distinct voice sentiments (negative, neutral, positive)__*</u>, are recorded. The recordings took place in <u>*__3 different types of places__*</u>, which are *an anechoic chamber, studio apartment, and dance studio*, of which the level of reverberation differs. And in order to examine the effect of the distance of mic from the source and device, every experiment is recorded at <u>*__3 distinct distances__*</u> with <u>*__2 types of smartphone__*</u>, *iPhone X, and Galaxy S7*.

There were two individuals in a group, and each group was distinguished by a unique key(subject ID). Two speakers(speaker a, speaker b) were facing each other 1.4m apart from each other (0.7m from the middle line). They read the allocated scripts alternating between speaker a and b, as if they were talking to each other.

 **Recording environment** | **Studio Apartment(moderate reverb), Dance studio(high reverb),<br /> Anechoic Chamber(no reverb)** |
 :-:|:-:|
  **Device** | **[iPhone X(iOS)](https://en.wikipedia.org/wiki/IPhone_X), [Samsung Galaxy S7](https://en.wikipedia.org/wiki/Samsung_Galaxy_S7)** |
 **Recording distance from the source** | **0.4m, 2.0m, 4.0m** |
  **Volume(Sample)** | **\~ 290(~ 3) hours, ~ 190,000(~ 2,000) utterances, ~ 107(~ 0.5) GB** |
  **Format** | **wav/h5(16/44.1kHz, 16-bit, mono)** |
  **Language** | **Korean** |

 Studio Apartment | Dance studio | Anechoic Chamber |  
:-:|:-:|:-:|
![Studio](https://github.com/deeplyinc/Korean-Read-Speech-Corpus/blob/main/etc/StudioApartment.jpeg) | ![Dacne studio](https://github.com/deeplyinc/Korean-Read-Speech-Corpus/blob/main/etc/DanceStudio.jpeg) | ![Studio](https://github.com/deeplyinc/Korean-Read-Speech-Corpus/blob/main/etc/AnechoicChamber.jpeg) |

Refer to the dataset descriptions in 'docs' for detailed description and statistics of the full set of the dataset.

The dataset is a subset(approximately 1%) of a much bigger dataset which were recorded under the same circumstances as these open source samples. Please contact us(contact@deeplyinc.com) for the full set with the academic/commercial license.

## Dataset statistics
The illustrations below are the statistics about the Deeply Korean Read Speech Corpus. The first three are from the sample dataset, And the others are from the full dataset. To attain more insight about the dataset, please refer to the detailed description in 'docs' and 'Korea_Read_Speech_Corpus.json' in 'Dataset'.

The sample is a partial set of recordings from a single subject group(sub1001), which consists of 20-year-old female(speaker a) and 49-year-old female(speaker b).

<p float="left">
  <img src="https://github.com/deeplyinc/Korean-Read-Speech-Corpus/blob/main/etc/fig0.png" width="275" />
  <img src="https://github.com/deeplyinc/Korean-Read-Speech-Corpus/blob/main/etc/fig1.png" width="275" /> 
  <img src="https://github.com/deeplyinc/Korean-Read-Speech-Corpus/blob/main/etc/fig2.png" width="275" />
</p>
<p float="left">
  <img src="https://github.com/deeplyinc/Korean-Read-Speech-Corpus/blob/main/etc/fig3.png" width="275" />
  <img src="https://github.com/deeplyinc/Korean-Read-Speech-Corpus/blob/main/etc/fig4.png" width="275" /> 
  <img src="https://github.com/deeplyinc/Korean-Read-Speech-Corpus/blob/main/etc/fig5.png" width="275" /> 
</p>
  <img src="https://github.com/deeplyinc/Korean-Read-Speech-Corpus/blob/main/etc/fig6.png" width="275" /> 

## Structure
```
├── Dataset
│   ├── AirbnbStudio
│   │   ├── sub100100a00000.wav
│   │   └── ...
│   ├── AnechoicChamber
│   │   ├── sub100120a00000.wav
│   │   └── ...
│   ├── DanceStudio
│   │   ├── sub100110a00000.wav
│   │   └── ...
│   └── Korean_Read_Speech_Corpus.json
└── docs
    ├── Deeply\ Korean\ Read\ Speech\ Corpus_Eng.pdf
    └── Deeply\ Korean\ Read\ Speech\ Corpus_Kor.pdf
```

```
Korean_Read_Speech_Corpus.json

{'AirbnbStudio': 
                {'sub100100a00000': {'text_sentiment': 0,
                                    'voice_sentiment': -1,
                                    'subjectID': 'sub1001',
                                    'speaker': 'a',
                                    'age': 20,
                                    'sex': 0,
                                    'noise': 0,
                                    'location': 0,
                                    'distance': 0,
                                    'device': 0,
                                    'text': '저 식당 음식이 정말 맛있나 봐요.',
                                    'text_code': 'aa0',
                                    'rms': 0.024304501712322235,
                                    'length': 2.71825},
                  ...
                  },
   ...
}
```
### How to decode
_Text sentiment_: {-1: negative, 0: neutral, 1: positive}  

_Vocie sentiment_: {-1: negative, 0: neutral, 1: positive}  

_Subject ID_: Unique 'sub + 4-digit' key allocated to each subject group  

_Speaker_: unique key allocated to each indiivdual in the subject group.  

_Sex_: {0: Female, 1: Male}  

_Noise_: {0: Noiseless, 1: Indoor noise, 2: Outdoor noise, 3: Both indoor/outdoor noise}  

_Location_: {0: Studio apartment, 1: Dance studio, 2: Anechoic chamber}  

_Distance_: {0: 0.4m, 1: 2.0m, 2: 4.0m}  

_Device_: {0: iPhone X, 1: Galaxy S7}  

_Text_: the content of the script  

_Text code_: unique key allocated to each line of the script  

_Rms_: Root mean square value of the signal  

_Length_: length of the signal in secods  

## License
Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)  
![Vue](https://github.com/deeplyinc/Korean-Read-Speech-Corpus/blob/main/etc/by-nc-nd.png)

## Contact
Tel:   (+82) 70-7459-0704  
Web:   http://deeplyinc.com/  
Email: contact@deeplyinc.com

