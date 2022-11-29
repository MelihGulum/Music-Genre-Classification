<p align="center"> 
  <img src="static/img/MGC-logo.png" alt="MGC Logo" width="350px" height="100px">
</p>
<h1 align="center"> Music Genre Classification </h1>

<h2 id="table-of-contents"> :book: Table of Contents</h2>

<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about_the_project"> ABOUT THE PROJECT</a></li>
    <li><a href="#dataset">  DATASET</a></li>
    <li><a href="#preprocess"> PREPROCESS</a></li>
    <li><a href="#deep_learning"> DEEP LEARNING</a></li>
    <li><a href="#web_application_flask"> WEB APPLICATION - FLASK</a></li>
    <li><a href="#how_to_run"> HOW TO RUN</a></li>
  </ol>
</details>

<h2 id="dataset"> :pencil: About The Project</h2>
<p align="justify">This project aims to classify music genres. Music Genre Classification is an Audio Signal Processing project. <strong>Signal Processing</strong> is one of the sub-fields of Deep Learning apart from <em>Image Processing</em> and <em>Natural Language Processing</em>. The GTZAN dataset consists of "<strong>wav</strong>" audio files. The Librosa library was used to extract the features of these audio files (more on Preprocess section). Different architectures have been created to classification (NN, LSTM, CNN...).</p>

<h2 id="preprocess"> :floppy_disk: DATASET</h2>
<p align="justify">The <a href="https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification">GTZAN</a> dataset was used. Briefly, the data set consists of 10 classes and the CSV file contains many attributes such as MFCC, Chroma, RMS. In addition, there are two different CSV in the dataset, whose attributes are extracted on the basis of 3 seconds and 30 seconds. </p>
<p align="center">   
  <img src="https://user-images.githubusercontent.com/81585804/204538070-b036f85f-a95b-4a92-858c-d64687081f1a.png" alt="The Classes of GTZAN (Image by Author)"     width="45%" height="45%">
</p>
 <p align="center"> <em>The Classes of GTZAN (Image by Author)</em> </p>


<h2 id="preprocess"> :hammer_and_wrench: PREPROCESS</h2>
<p align="justify"> As I said earlier, Librosa was used for feature extraction. Features in CSV were not used. I extracted my own features instead of these features,. These features are the top 13 of the MFCCs. Each data was read sequentially. At the same time, the MFCC features are extracted and their labels are respectively added to a json file. </p>
<p align="justify">The code cell below, can be seen how MFCC's are extracted.</p>

```python
y, sample_rate = librosa.load(file_path, sr=SAMPLE_RATE)
librosa.feature.mfcc(y, sample_rate, n_mfcc=13, n_fft=2048, hop_length=512)
```

<h2 id="deep_learning"> :desktop_computer: DEEP LEARNING</h2>




<h2 id="web_application_flask"> :rocket: WEB APPLICATION - FLASK</h2>



<h2 id="how_to_run"> :running: HOW TO RUN</h2>










