[![License][license-shield]][license-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/github_username/repo">
    <img src="https://images.unsplash.com/photo-1523995462485-3d171b5c8fa9?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&w=1000&q=80" alt="Logo" width="150" height="250">
  </a>

  <h3 align="center">Document Classifier (20 NewsSet)</h3>

  <p align="justify">
  In this project, we'll be identifying the document and classifying it into one of the available 20 classes of documents.
    <br /></p>
  <p align="center">
    <a href="https://github.com/decodrtechnologies/Data-Science/tree/master/Document-Classification"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/decodrtechnologies/Data-Science/tree/master/Document-Classification">View Demo</a>
    ·
    <a href="https://github.com/decodrtechnologies/Data-Science/issues">Report Bug</a>
    ·
    <a href="https://github.com/decodrtechnologies/Data-Science/issues">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#built-with)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Dataset](#Dataset)
  * [Context](#context)
  * [Organization](#Organization)
  * [Data](#data)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Dataset owner](#Dataset-Owner)



<!-- ABOUT THE PROJECT -->
## About The Project

  In this project, we'll be identifying the documents and classifing them into one of the 20 available classes. The main task will be to load the dataset, remove stopwords and identify most occuring words per class and later for test set predict the class of document. We will later use this trained model to classify  manually entered sentences that belong to those 20 classes.

### Built With
The entire coding part is done using:
* [Jupyter Notebook](https://jupyter.org/)

Important python libraries to be used:
* [numpy](https://anaconda.org/anaconda/numpy)
* [pandas](https://anaconda.org/anaconda/pandas)
* [sklearn](https://anaconda.org/anaconda/sklearn)
* [sklearn](https://anaconda.org/anaconda/sklearn)
* [nltk](https://anaconda.org/anaconda/nltk)






<!-- GETTING STARTED -->
## Getting Started



### Prerequisites

Basic knowledge of python, data visualtisation libraries, NLP and naive bayes technique is required.

### Installation
 
1. Clone the repo
```sh
git clone https://github.com/github_username/repo.git
```
2. Install Jupyter notebook
3. Install Python packages

<!-- DATASET -->

## Dataset

### Context

The 20 Newsgroups data set is a collection of approximately 20,000 newsgroup documents, partitioned (nearly) evenly across 20 different newsgroups. To the best of my knowledge, it was originally collected by Ken Lang, probably for his Newsweeder: Learning to filter netnews paper, though he does not explicitly mention this collection. The 20 newsgroups collection has become a popular data set for experiments in text applications of machine learning techniques, such as text classification and text clustering.

### Organization

The data is organized into 20 different newsgroups, each corresponding to a different topic. Some of the newsgroups are very closely related to each other (e.g. comp.sys.ibm.pc.hardware / comp.sys.mac.hardware), while others are highly unrelated (e.g misc.forsale / soc.religion.christian). Here is a list of the 20 newsgroups, partitioned (more or less) according to subject matter:

  comp.graphics<br>
  comp.os.ms-windows.misc<br>
  comp.sys.ibm.pc.hardware<br>
  comp.sys.mac.hardware<br>
  comp.windows.x<br>
  rec.autos<br>
  rec.motorcycles<br>
  rec.sport.baseball<br>
  rec.sport.hockey<br>
  sci.crypt<br>
  sci.electronics<br>
  sci.med<br>
  sci.space<br>
  misc.forsale<br>
  talk.politics.misc<br>
  talk.politics.guns<br>
  talk.politics.mideast<br>
  talk.religion.misc<br>
  alt.atheism<br>
  soc.religion.christian<br>

### Data

The data available <a href = "http://qwone.com/~jason/20Newsgroups/">here</a> are in .tar.gz bundles. You will need tar and gunzip to open them. Each subdirectory in the bundle represents a newsgroup; each file in a subdirectory is the text of some newsgroup document that was posted to that newsgroup.

Below are three versions of the data set. The first ("19997") is the original, unmodified version. The second ("bydate") is sorted by date into training(60%) and test(40%) sets, does not include cross-posts (duplicates) and does not include newsgroup-identifying headers (Xref, Newsgroups, Path, Followup-To, Date). The third ("18828") does not include cross-posts and includes only the "From" and "Subject" headers.

    20news-19997.tar.gz - Original 20 Newsgroups data set
    20news-bydate.tar.gz - 20 Newsgroups sorted by date; duplicates and some headers removed (18846 documents)
    20news-18828.tar.gz - 20 Newsgroups; duplicates removed, only "From" and "Subject" headers (18828 documents) 

I recommend the "bydate" version since cross-experiment comparison is easier (no randomness in train/test set selection), newsgroup-identifying information has been removed and it's more realistic because the train and test sets are separated in time. 

<!-- ROADMAP -->
## Roadmap

We'll follow OSEMN Pipeline: 

    O - Obtaining our data
    S - Scrubbing / Cleaning our data
    E - Exploring / Visualizing our data will allow us to find patterns and trends
    M - Modeling our data will give us our predictive power as a wizard
    N - INterpreting our data

After we are able to complete above steps and we have the model, the task at the end will be to tune hyperparameter to optimise our model's performance.

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Dataset used in the problem is available open source on <a href = "http://archive.ics.uci.edu/ml/datasets/Twenty+Newsgroups">UCI Machine Learning</a> and the Original Owner and Donor is Tom Mitchell.

<!-- CONTACT -->
## Dataset Owner
<br>
Tom Mitchell<br>
School of Computer Science<br>
Carnegie Mellon University<br>
tom.mitchell '@' cmu.edu<br>
http://www.cs.cmu.edu/~tom/<br>



Project Link: [https://github.com/decodrtechnologies/Data-Science](https://github.com/decodrtechnologies/Data-Science)



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/decodrtechnologies/Data-Science.svg?style=flat-square
[contributors-url]: https://github.com/decodrtechnologies/Data-Science/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/decodrtechnologies/Data-Science.svg?style=flat-square
[forks-url]: https://github.com/decodrtechnologies/Data-Science/network/members
[stars-shield]: https://img.shields.io/github/stars/decodrtechnologies/Data-Science.svg?style=flat-square
[stars-url]: https://github.com/decodrtechnologies/Data-Science/stargazers
[issues-shield]: https://img.shields.io/github/issues/decodrtechnologies/Data-Science.svg?style=flat-square
[issues-url]: https://github.com/decodrtechnologies/Data-Science/issues
[license-shield]: https://img.shields.io/github/license/decodrtechnologies/Data-Science.svg?style=flat-square
[license-url]: https://github.com/decodrtechnologies/Data-Science/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[product-screenshot]: images/screenshot.png
