# wiki4HE Dataset

In this project we are going to perform clustering on the above given dataset. The clustering algorithm used while implementation is K-Means Clustering.

## License:-

The above mentioned dataset is an opensource dataset from UCI Machine Learning.

### Citation:-

Meseguer, A., Aibar, E., LladÃ³s, J., MinguillÃ³n, J., Lerga, M. (2015). â€œFactors that influence the teaching use of Wikipedia in Higher Educationâ€. JASIST, Journal of the Association for Information Science and Technology. ISSN: 2330-1635. doi: 10.1002/asi.23488.

Source: https://archive.ics.uci.edu/ml/datasets/wiki4HE

## Dataset Information:-

The dataset has been taken from: https://archive.ics.uci.edu/ml/datasets/wiki4HE
 
The dataset is having 913 instances and 53 different attributes.

## Attribute Information:-

AGE: numeric

GENDER: 0=Male; 1=Female

DOMAIN: 1=Arts & Humanities; 2=Sciences; 3=Health Sciences; 4=Engineering & Architecture; 5=Law & Politics

PhD: 0=No; 1=Yes

YEARSEXP (years of university teaching experience): numeric

UNIVERSITY: 1=UOC; 2=UPF

UOC_POSITION (academic position of UOC members): 1=Professor; 2=Associate; 3=Assistant; 4=Lecturer; 5=Instructor; 6=Adjunct

OTHER (main job in another university for part-time members): 1=Yes; 2=No

OTHER_POSITION (work as part-time in another university and UPF members): 1=Professor; 2=Associate; 3=Assistant; 4=Lecturer; 5=Instructor; 6=Adjunct

USERWIKI (Wikipedia registered user): 0=No; 1=Yes

The following survey items are Likert scale (1-5) ranging from strongly disagree / never (1) to strongly agree / always (5)

Perceived Usefulness:-

PU1: The use of Wikipedia makes it easier for students to develop new skills

PU2: The use of Wikipedia improves students' learning

PU3: Wikipedia is useful for teaching

Perceived Ease of Use:-
PEU1: Wikipedia is user-friendly

PEU2: It is easy to find in Wikipedia the information you seek

PEU3: It is easy to add or edit information in Wikipedia

Perceived Enjoyment:-

ENJ1: The use of Wikipedia stimulates curiosity

ENJ2: The use of Wikipedia is entertaining

Quality:-

QU1: Articles in Wikipedia are reliable

QU2: Articles in Wikipedia are updated

QU3: Articles in Wikipedia are comprehensive

QU4: In my area of expertise, Wikipedia has a lower quality than other educational resources

QU5: I trust in the editing system of Wikipedia

Visibility:-

VIS1: Wikipedia improves visibility of students' work

VIS2: It is easy to have a record of the contributions made in Wikipedia

VIS3: I cite Wikipedia in my academic papers

Social Image:-

IM1: The use of Wikipedia is well considered among colleagues

IM2: In academia, sharing open educational resources is appreciated

IM3: My colleagues use Wikipedia

Sharing attitude:-

SA1: It is important to share academic content in open platforms

SA2: It is important to publish research results in other media than academic journals or books

SA3: It is important that students become familiar with online collaborative environments

Use behaviour:-

USE1: I use Wikipedia to develop my teaching materials

USE2: I use Wikipedia as a platform to develop educational activities with students

USE3: I recommend my students to use Wikipedia

USE4: I recommend my colleagues to use Wikipedia

USE5: I agree my students use Wikipedia in my courses

Profile 2.0:-

PF1: I contribute to blogs

PF2: I actively participate in social networks

PF3: I publish academic content in open platforms

Job relevance:-

JR1: My university promotes the use of open collaborative environments in the Internet

JR2: My university considers the use of open collaborative environments in the Internet as a teaching merit

Behavioral intention:-

BI1: In the future I will recommend the use of Wikipedia to my colleagues and students

BI2: In the future I will use Wikipedia in my teaching activity

Incentives:-

INC1: To design educational activities using Wikipedia, it would be helpful: a best practices guide

INC2: To design educational activities using Wikipedia, it would be helpful: getting instruction from a colleague

INC3: To design educational activities using Wikipedia, it would be helpful: getting specific training

INC4: To design educational activities using Wikipedia, it would be helpfull: greater institutional recognition

Experience:-

EXP1: I consult Wikipedia for issues related to my field of expertise

EXP2: I consult Wikipedia for other academic related issues

EXP3: I consult Wikipedia for personal issues

EXP4: I contribute to Wikipedia (editions, revisions, articles improvement...)

EXP5: I use wikis to work with my students

## Libraries Used:-

1. Numpy
2. Pandas 
3. Matplotlib
4. Seaborn
5. Sklearn

## Feature Engineering:-

Feature engineering is the process of transforming raw data into features that better represent the underlying problem to the predictive models, resulting in improved model accuracy on unseen data. Feature engineering turn your inputs into things the algorithm can understand.

## Clustering Algorithm Used:-

In the above problem statement we have used K-Means Clustering Algorithm.

K means clustering algorithm is a very common unsupervised learning algorithm. This algorithm clusters n objects into k clusters, where each object belongs to a cluster with the nearest mean.

K-means clustering is a method of vector quantization, originally from signal processing, that aims to partition n observations into k clusters in which each observation belongs to the cluster with the nearest mean (cluster centers or cluster centroid), serving as a prototype of the cluster. This results in a partitioning of the data space into Voronoi cells. It is popular for cluster analysis in data mining. k-means clustering minimizes within-cluster variances (squared Euclidean distances), but not regular Euclidean distances, which would be the more difficult Weber problem: the mean optimizes squared errors, whereas only the geometric median minimizes Euclidean distances.

<img src ="https://thatware.co/wp-content/uploads/2019/03/k-mean-clustering.png" height="800" width="800">
<br>src:https://thatware.co/</img>
