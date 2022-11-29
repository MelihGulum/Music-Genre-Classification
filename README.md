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

<h2 id="about_the_project"> :pencil: About The Project</h2>
<p>This project aims to classify music genres. Music Genre Classification is an Audio Signal Processing project. <strong>Signal Processing</strong> is one of the sub-fields of Deep Learning apart from <em>Image Processing</em> and <em>Natural Language Processing</em>. The GTZAN dataset consists of "<strong>wav</strong>" audio files. The Librosa library was used to extract the features of these audio files (more on Preprocess section). Different architectures have been created to classification (NN, LSTM, CNN...).</p>

<h2 id="preprocess"> :floppy_disk: DATASET</h2>
<p>The [GTZAN] (https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification) dataset was used. Briefly, the data set consists of 10 classes and the CSV file contains many attributes such as MFCC, Chroma, RMS. . In addition, there are two different CSV in the dataset, whose attributes are extracted on the basis of 3 seconds and 30 seconds. </p>
<p align="center">   <img src="![Music Genre Classifier](https://user-images.githubusercontent.com/81585804/204538070-b036f85f-a95b-4a92-858c-d64687081f1a.png)" alt="Table1: 18 Activities" width="45%" height="45%">

  <em>The CLasses of GTZAN (Image by Author)</em>
  <p align="center">
  ![Music Genre Classifier](https://user-images.githubusercontent.com/81585804/204538070-b036f85f-a95b-4a92-858c-d64687081f1a.png)        
  <!--figcaption>The CLasses of GTZAN (Image by Author)</figcaption-->
</p>
</p>

![Music Genre Classifier](https://user-images.githubusercontent.com/81585804/204538070-b036f85f-a95b-4a92-858c-d64687081f1a.png)

<h2 id="preprocess"> :hammer_and_wrench: PREPROCESS</h2>
