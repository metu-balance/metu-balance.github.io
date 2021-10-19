Project webpage for the project entitled "Addressing Class Imbalance in Visual Recognition Problems by Measuring Class Imbalance and Using Epistemic Uncertainty" with acronym BALANCE (DENGE), supported by [TUBITAK](http://tubitak.gov.tr/) 1001 (no 120E494).

<style>
.aS {
  display: block;
  list-style-type: disc;
  margin-left: 15px;
  margin-right: 15px;
  float: left;
  
}

.divS{
  display: block;
  list-style-type: disc;
  overflow: auto;
  padding-left: 60px;
  padding-right: 60px;
  margin:auto;
}

/* By Dominik Biedebach @domobch */

/* NAVIGATION */
nav {
  width: 100%;
  margin: 0 auto;
  padding: auto;
}

/* By Dominik Biedebach @domobch */
nav ul {
  list-style: none;
  text-align: center;
}
nav ul li {
  display: inline-block;
}
nav ul li a {
  display: block;
  padding: 1px;
  text-decoration: none;
  color: #5d5d5d;
  font-weight: 800;
  text-transform: uppercase;
  margin: 1px 1px;
  margin-top: 15px;
}
nav ul li a,
nav ul li a:after,
nav ul li a:before {
  transition: all .5s;
}
nav ul li a:hover {
  color: #555;
}

/* By Dominik Biedebach @domobch */


/* stroke */
nav.stroke ul li a,
nav.fill ul li a {
  position: relative;
}
nav.stroke ul li a:after,
nav.fill ul li a:after {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  margin: auto;
  width: 0%;
  content: '.';
  color: transparent;
  background: #333;
  height: 1px;
}
nav.stroke ul li a:hover:after {
  width: 100%;
}

nav.fill ul li a {
  transition: all 2s;
}


}
</style>


  <nav class="stroke">
    <ul>
      <li><a class="aS" href="#wid">What is DENGE?</a></li>
      <li><a class="aS" href="#summary">Summary</a></li>
      <li><a class="aS" href="#publications">Publications</a></li>
      <li><a class="aS" href="#contact">Contact</a></li>
    </ul>
  </nav>


------

<p align="center">
    <img src="./visuals/dengesizlik_plot.png" width="100%">
    <i>Figure 1: Many problems in practice exhibit strong imbalance towards certain classes or categories, which can severely impact learning performance. (a) Foreground-background imbalance problem in object detection. (b) Imbalance problem among object categories. (Figure source: [Oksuz et al., 2021](https://arxiv.org/abs/1909.00169)).</i>
</p>

-----
### <tag id="wid">What is DENGE?</tag>

DENGE is a project supported by [TUBITAK](http://tubitak.gov.tr/) as a two-year project (2021-2023) for developing better methods for addressing imbalance problems. The project is being conducted at [METU Image Lab, Dept. of Computer Eng., METU](https://image.ceng.metu.edu.tr). It builds on the team's experience on and extends the results of the team's previous project entitled "Object Detection in Videos with Deep Neural Networks" (funded by [TUBITAK](http://tubitak.gov.tr/) with no 117E054).

| <!-- -->      | <!-- --> |
| ------------- | -------- |
| Project No    | 120E494     |
| Project Type | [ARDEB-1001](https://www.tubitak.gov.tr/tr/destekler/akademik/ulusal-destek-programlari/icerik-1001-bilimsel-ve-teknolojik-arastirma-projelerini-destekleme-pr) | 
| Budget          | ~ TRY 340K (~ $ 45K) |
| Dates           | 1 March 2021 - 1 March 2023 | 
| Coordinators | Emre Akbas](http://ceng.metu.edu.tr/~emre/) [METU Image Lab, Dept. of Computer Eng., METU] and [Sinan Kalkan](http://ceng.metu.edu.tr/~skalkan/) [METU Image Lab, Dept. of Computer Eng., METU]  |
| Researchers | [Kemal Oksuz](https://kemaloksuz.github.io/) [METU Image Lab, Dept. of Computer Eng., METU] |
| Students    | Zeynep Sonat Baltaci, Baris Can Cam, Gunes Cepic, Sinem Donmez, Cagri Eser, Ece Gokcay, Baran Gulmez, Ertugrul Gungor, Fehmi Kahraman, Berkin Kerim Konar, Selim Kuzucu, Alpay Ozkan, Kivanc Tezoren, Feyza Yavuz |


### <tag id="summary">Summary</tag> 

Class imbalance (CI) is an important problem affecting the generalization performance of machine learning methods. CI can basically be defined as the problem that some classes contain fewer samples than others in the dataset. According to this definition and the general opinion in the literature, this unbalanced distribution between classes causes machine learning methods to perform better on classes containing a large number of samples, while being insufficient for classes containing a small number of samples.

Many methods have been developed against CI problems in recent years. These methods generally suggest (i) correcting bias by over-sampling or sub-sampling, or (ii) attaching more importance to “hard” samples. These methods are known to alleviate the CI problem and improve performance.

The proposed project will focus on improving existing methods in the following ways:

* Observation 1: Having relatively fewer samples for one class does not mean that the classification performance of that class will be poor.

* Observation 2: Sample hardness may not be an indicator of imbalance, although it has shown promising results.

### <tag id=publications>Publications</tag> 

The list of publications (from DENGE and its precursor project):

* K. Oksuz, B. C. Cam, S. Kalkan*, E. Akbas*, "One Metric to Measure them All: Localisation Recall Precision (LRP) for Evaluating Visual Detection Tasks", IEEE Transactions on Pattern Analysis and Machine Intelligence (PAMI), under review, 2021. [Arxiv](https://arxiv.org/abs/2011.10772), [Code](https://github.com/kemaloksuz/LRP-Error).
* K. Oksuz, B. C. Cam, E. Akbas*, S. Kalkan*, "Rank & Sort Loss for Object Detection and Instance Segmentation", International Conference on Computer Vision (ICCV), oral presentation, 2021. [Arxiv](https://arxiv.org/abs/2107.11669), [Code](https://github.com/kemaloksuz/RankSortLoss).
* K. Oksuz, B. C. Cam, S. Kalkan*, E. Akbas*, "Imbalance Problems in Object Detection: A Review", IEEE Transactions on Pattern Analysis and Machine Intelligence (PAMI), 43(10):3388-3415, 2021. [Arxiv](https://arxiv.org/abs/1909.00169), [Publisher](https://ieeexplore.ieee.org/document/9042296), [Repo](https://github.com/kemaloksuz/ObjectDetectionImbalance).
* K. Oksuz, B. C. Cam, E. Akbas*, S. Kalkan*, "A Ranking-based, Balanced Loss Function Unifying Classification and Localisation in Object Detection", Thirty-fourth Conference on Neural Information Processing Systems (NeurIPS), spotlight paper, 2020. [Arxiv](https://arxiv.org/abs/2009.13592), [NeurIPS](https://proceedings.neurips.cc/paper/2020/hash/b2eeb7362ef83deff5c7813a67e14f0a-Abstract.html), [Code](https://github.com/kemaloksuz/aLRPLoss).
* K. Oksuz, B. C. Cam, E. Akbas*, S. Kalkan*, "Generating Positive Bounding Boxes for Balanced Training of Object Detectors", IEEE Winter Conference on Applications of Computer Vision (WACV), 2020. [Arxiv](https://arxiv.org/abs/1909.09777), [Publisher](https://www.computer.org/csdl/proceedings-article/wacv/2020/09093503/1jPbqXS57W0), [Code](https://github.com/kemaloksuz/BoundingBoxGenerator).
* 



### <tag id=contact>Contact</tag> 

Please use the following email address for course related issues: metu-denge [@] googlegroups [dot] com
