# Benchmark dataset of memes with text transcriptions for automatic detection of multi-modal misogynistic content
The benchmark here provided is composed of 800 memes collected from the most popular social media platforms, such as Facebook, Twitter,
Instagram and Reddit, and consulting websites dedicated to collection and creation of memes.
The dataset provided is composed of the 800 memes, the labels given by the experts and those obtained by the crowdsourcing validation, and the transcribed texts. 

This data can be used to approach the problem of automatic detection of misogynistic content on the Web relying on both textual and visual cues, facing phenomenons 
that are growing every day such as cybersexism and technology-facilitated violence.
For further information on the data provided and on the methodologies adopted in the data collection and labeling phase, please consult our [paper](https://arxiv.org/abs/2106.08409).
___
## Data
In order to develop efficient machine learning techniques able to automatically detect multi-modal misogynistic messages online, we here present a dataset composed of: 
- **800 memes**, saved as jpeg images, resized to have the greatest dimension equal to 640 pixels. These memes are saved with a progressive unique ID.
- A **table** saved as a .csv file, where all the data collected are reported, according to the following structure: 
  - *memeID*: unique identifier associated to the meme;
  - *text*: transcription of the text reported in the meme;
  - *misogynisticDE*: Boolean attribute related to the presence of misogynistic content as reported by the  Domain Experts (DE);
  - *aggressiveDE*: Boolean attribute; in case of a misogynist meme it represents the presence of aggressiveness, as reported by the DE;
  - *ironicDE*: Boolean attribute; in case of a misogynist meme it represents the presence of irony, as reported by the DE;
  - *misogynisticCS*: Boolean attribute related to the presence of misogynistic content, as reported by the annotators of the CrowdSourcing  platform (CS);
  - *aggressiveCS*: Boolean attribute; in case of misogynist meme it represents the presence of aggressiveness, as reported by the CS;
  - *ironicCS*: Boolean attribute; in case of misogynist meme it represents the presence of irony, as reported by the CS.
  - *confidence\_M\_CS*: agreement on the misogynist attribute among the CS;
  - *confidence\_A\_CS*: agreement on the aggressiveness attribute among the CS;
  - *confidence\_I\_CS*: agreement on the misogynist irony among the CS;

## Data Access
The datasets is exclusively reserved for for research purposes. 
The data may be distributed upon request and for academic purposes only. 
To request the datasets, please fill out the following form: https://forms.gle/52amNcsh1dzrYN3DA

After submitting the required info, requesters will have the password to un-zip the data provided here in '.zip' format.
For the unzipping process we suggest to use 7-zip (more information for the extraction process can be finde below).

This repository contains two .zip files, both protected by the same password, obtainable from the aforementioned form.
The files have the following structure:
```
- Misogynistic-MEME_pt1.zip
    ├─ Images [folder containg 400 misogynous memes]
    └─ table.csv
- Misogynistic-MEME_pt2.zip
    └─ Images-pt2 [folder containg 400 non-misogynous memes]

```

### Data extraction with 7-zip
Once downloaded and installed [7-zip](https://www.7-zip.org/download.html), right click on the '.zip' file, choose 7-Zip and Extract Files.
In the current window, choose a place to extract the file and type the password.
Once this is done, press ok. You can now open the folder and access the dataset.
