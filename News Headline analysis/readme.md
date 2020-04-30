
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![License][license-shield]][license-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/github_username/repo">
    <img src="https://images.unsplash.com/photo-1523995462485-3d171b5c8fa9?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&w=1000&q=80" alt="Logo" width="150" height="250">
  </a>

  <h3 align="center">News Headline Analysis</h3>

  <p align="justify">
  In this project, we'll be identifying topics of national discussion in past 10 years in Australlia. Our basic task will be to analyse the headlines present in dataset and find out topics that prevail in news.
    <br /></p>
  <p align="center">
    <a href="https://github.com/decodrtechnologies/Data-Science/tree/master/News Headline analysis"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/decodrtechnologies/Data-Science/tree/master/News Headline analysis">View Demo</a>
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
  * [Content](#content)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Dataset owner](#Dataset-Owner)



<!-- ABOUT THE PROJECT -->
## About The Project

  In this project, we'll be identifying topics of national discussion in past 10 years in Australlia. Our basic task will be to analyse the headlines present in dataset and find out topics that prevail in news. The news headlines are taken from 'A million news' dataset available on Kaggle. The main task will be to load the dataset, remove stopwords and identify most occuring words and later doing LDA to identify most prevailing topics of national interest.

### Built With
The entire coding part is done using:
* [Jupyter Notebook](https://jupyter.org/)

Important python libraries to be used:
* [numpy](https://anaconda.org/anaconda/numpy)
* [pandas](https://anaconda.org/anaconda/pandas)
* [matplotlib](https://anaconda.org/anaconda/matplotlib)
* [seaborn](https://anaconda.org/anaconda/seaborn)
* [scipy](https://anaconda.org/anaconda/scipy)
* [tqdm](https://anaconda.org/anaconda/tqdm)
* [sklearn](https://anaconda.org/anaconda/sklearn)
* [nltk](https://anaconda.org/anaconda/nltk)






<!-- GETTING STARTED -->
## Getting Started



### Prerequisites

Basic knowledge of python, data visualtisation libraries, NLP and K-nearest neighbour technique is required.

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

The  dataset contains data of news headlines published over a period of seventeen years.

Sourced from the reputable Australian news source ABC (Australian Broadcasting Corp.)

Agency Site: (http://www.abc.net.au)

### Content

Format: CSV ; Single File

    publish_date: Date of publishing for the article in yyyyMMdd format
    headline_text: Text of the headline in Ascii , English , lowercase

Start Date: 2003-02-19 ; End Date: 2019-12-31

This includes the entire corpus of articles published by the abcnews website in the given time range.
With a volume of two hundred articles per day and a good focus on international news, we can be fairly certain that every event of significance has been captured here.

Digging into the keywords, one can see all the important episodes shaping the last decade and how they evolved over time.
Ex: afghanistan war, financial crisis, multiple elections, ecological disasters, terrorism, famous people, criminal activity et cetera.

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

A Million News Headlines Dataset used in the problem is available open source on <a href = "https://www.kaggle.com/therohk/million-headlines/">Kaggle</a> and the license is available at this <a href = "https://creativecommons.org/publicdomain/zero/1.0/"> link </a>.



<!-- CONTACT -->
## Dataset Owner

Rohk (@ https://www.kaggle.com/therohk)

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
[linkedin-url]: https://www.linkedin.com/in/suraj-tiwari-9867a7164/
[product-screenshot]: images/screenshot.png
