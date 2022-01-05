## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/xxctm/tmtmp/edit/main/docs/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/xxctm/tmtmp/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

# Samples of Noisy-to-Noisy Voice Conversion Framework

Those samples come from the [paper](https://arxiv.org/abs/2111.07116).

Speech dataset: [VCC 2018 Evaluation set](https://datashare.ed.ac.uk/handle/10283/3061)

Noise dataset: [PNL 100 Nonspeech](http://web.cse.ohio-state.edu/pnl/corpus/HuNonspeech/HuCorpus.html) (N86 to N100 for evaluation set)

### 1. Noisy source (Speaker SF3;  Noise type: Cry (N93);  SNR level: 15dB):
<audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMDJf/noisy_sf3_30016_n93_snr15.wav"></audio>

Denosied source:
<audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQwOThf/denoised_sf3_30016_n93_snr15.wav"></audio>

Target (Speaker TF2): 
<audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQwODZf/TF2_30002.wav"></audio>

| Methods             | Clean         | Noisy            |
|---------------------|---------------|------------------|
|Baseline                    |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQwOTVf/base_clean_sf3tf2_30016_n93_snr15.wav"></audio>   |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMTk4NjIzODlf/da_15_sf3tf2_30016_n93.wav"></audio>   |
|Proposed (Improved 2 Direct)|   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQwOTZf/method2_clean_sf3tf2_30016_n93_snr15.wav"></audio>   |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMTk4NjI2MTZf/md_15_sf3tf2_30016_n93.wav"></audio>   |
|Upper Bound                 |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQwOTdf/upper_clean_sf3tf2_30016.wav"></audio>      |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMTk4NjIyNzBf/ca_15_sf3tf2_30016_n93.wav"></audio>   |


### 2. Noisy source (Speaker SF4;  Noise type: Phone dialing (N100);  SNR level: 7dB):
<audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMTNf/noisy_sf4_30026_n100_snr7.wav"></audio>

Denosied source:
<audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMTFf/denoised_sf4_30026_n100_snr7.wav"></audio>

Target (Speaker TM2): 
<audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMDRf/TM2_30002.wav"></audio>

| Methods             | Clean         | Noisy            |
|---------------------|---------------|------------------|
|Baseline                    |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMDlf/base_sf4tm2_30026_n100_snr7.wav"></audio>   |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMTk4NjIzMjdf/da_7_sf4tm2_30026_n100.wav"></audio>   |
|Proposed (Improved 2 Direct)|   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMTBf/method2_sf4tm2_30026_n100_snr7.wav"></audio>   |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMTk4NjI1OTNf/md_7_sf4tm2_30026_n100.wav"></audio>   |
|Upper Bound                 |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMTVf/upper_clean_sf4tm2_30026.wav"></audio>      |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMTk4NjIyMzdf/ca_7_sf3tm2_30026_n100.wav"></audio>   |


### 3. Noisy source (Speaker SM3;  Noise type: Snore (N87);  SNR level: 7dB):
<audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMTNf/noisy_sf4_30026_n100_snr7.wav"></audio>

Denosied source:
<audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMTFf/denoised_sf4_30026_n100_snr7.wav"></audio>

Target (Speaker TM2): 
<audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMDRf/TM2_30002.wav"></audio>

| Methods             | Clean         | Noisy            |
|---------------------|---------------|------------------|
|Baseline                    |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMDlf/base_sf4tm2_30026_n100_snr7.wav"></audio>   |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMTk4NjIzMjdf/da_7_sf4tm2_30026_n100.wav"></audio>   |
|Proposed (Improved 2 Direct)|   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMTBf/method2_sf4tm2_30026_n100_snr7.wav"></audio>   |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMTk4NjI1OTNf/md_7_sf4tm2_30026_n100.wav"></audio>   |
|Upper Bound                 |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMjA5NzQxMTVf/upper_clean_sf4tm2_30026.wav"></audio>      |   <audio id="audio" controls="" preload="none"><source id="wav" src="https://od.lk/s/NTBfMTk4NjIyMzdf/ca_7_sf3tm2_30026_n100.wav"></audio>   |





