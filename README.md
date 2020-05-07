# Streaming data sets

This repository contains a collection of datasets. While some data sets are used for batch learning they can be also be used in the streaming setting. On the other hand, some data sets have characteristics that make them better suited for the stream learning setting, e.g., they contain non-stationary data.

* **Agrawal-abrupt and Agrawal-gradual** (agr_a.csv, agr_g)

  *Type: Binary classification*
  
  Based on the Agrawal generator, represent a data stream with six nominal and three numerical features. Different functions map instances into two different classes. Three abrupt drifts are simulated for `AGRa` and three gradual drifts for `AGRg`.
  > Heitor Murilo Gomes, Albert Bifet, Jesse Read, Jean Paul Barddal, Fabricio Enembreck, Bernhard Pfharinger, Geoff Holmes, Talel Abdessalem. Adaptive random forests for evolving data stream classification. In Machine Learning, DOI: 10.1007/s10994-017-5642-8, Springer, 2017.

* **Airlines** (airlines.csv)

  *Type: Binary classification*
  
  Real world data containing information from scheduled departures of commercial flights within the US. The objective is to predict if a flight will be delayed.
  > Heitor Murilo Gomes, Albert Bifet, Jesse Read, Jean Paul Barddal, Fabricio Enembreck, Bernhard Pfharinger, Geoff Holmes, Talel Abdessalem. Adaptive random forests for evolving data stream classification. In Machine Learning, DOI: 10.1007/s10994-017-5642-8, Springer, 2017.

  *Note:* Variation of the [airlines dataset](http://kt.ijs.si/elena_ikonomovska/data.html) from Ikonomovska.

* **Covertype** (covtype.csv)

  *Type: Multi-class classification*
  
  This data set contains data collected over time by the US Forest Service. Classes correspond to cover type in forest on squares of 30×30 meters.
  > Blackard, Jock A. and Denis J. Dean. 2000. "Comparative Accuracies of Artificial Neural Networks and Discriminant Analysis in Predicting Forest Cover Types from Cartographic Variables." Computers and Electronics in Agriculture 24(3):131-151.

* **Electricity Market** (elec.csv)

  *Type: Binary classification*
  
  Data from the Australian New South Wales electricity market where prices are not fixed but change based on offer and demand. The 2 target classes represent changes in the price (1=up or 0=down).
  > M. Harries, N.S. Wales, Splice-2 comparative evaluation: Electricity pricing, 1999.

  *Notes:* This version does not include the attributes 'date' and 'day'.

* **Hyperplane-fast** (hyper_f.csv)

  *Type: Binary classification*

  A data stream with fast incremental drifts where a d-dimensional hyperplane changes position and orientation. Created with the random hyperplane generator.
  > Heitor Murilo Gomes, Albert Bifet, Jesse Read, Jean Paul Barddal, Fabricio Enembreck, Bernhard Pfharinger, Geoff Holmes, Talel Abdessalem. Adaptive random forests for evolving data stream classification. In Machine Learning, DOI: 10.1007/s10994-017-5642-8, Springer, 2017.

* **Iris (with artificial timestamps)** (iris_timestamp.csv)

  *Type: Multi-class classification*
  
  Description of the original dataset from the UCI repository: "The data set contains 3 classes of 50 instances each, where each class refers to a type of iris plant. One class is linearly separable from the other 2; the latter are NOT linearly separable from each other."

  > Fisher, Rory A. "The use of multiple measurements in taxonimic problems." (1936).

* **Moving Squares** (moving_squares.csv)

  *Type: Multi-class classification*
  
  Four equidistantly separated, squared uniform distributions are moving in horizontal direction with constant speed. The direction is inverted whenever the leading square reaches a predefined boundary. Each square represents a different class. The added value of this dataset is the predefined time horizon of 120 examples before old instances may start to overlap current ones. This is especially useful for dynamic sliding window approaches, allowing to test whether the size is adjusted accordingly.
  > Losing, V., Hammer, B. and Wersing, H., 2016, December. Knn classifier with self adjusting memory for heterogeneous concept drift. In Data Mining (ICDM), 2016 IEEE 16th International Conference on (pp. 291-300). IEEE.

* **Music (emotions)** (music.csv)

  *Type: Multi-label classification*
  
  593 songs with 6 clusters of music emotions based on the Tellegen-Watson-Clark model.
  > Read, J., Reutemann, P., Pfahringer, B. and Holmes, G., 2016. Meka: a multi-label/multi-target extension to weka. The Journal of Machine Learning Research, 17(1), pp.667-671.
  
  > K. Trohidis, G. Tsoumakas, G. Kalliris, I. Vlahavas. "Multilabel Classification of Music into Emotions". Proc. 2008 International Conference on Music Information Retrieval (ISMIR 2008), pp. 325-330, Philadelphia, PA, USA, 2008.

* **SEA-abrupt and SEA-gradual** (sea_a.csv, sea_g.csv)
  
  *Type: Binary classification*

  A data stream with three numerical features where only two attributes are related to the target class. Created using the SEA generator. Three abrupt drifts are simulated for `SEAa` and three gradual drifts for `SEAg`.
  > Heitor Murilo Gomes, Albert Bifet, Jesse Read, Jean Paul Barddal, Fabricio Enembreck, Bernhard Pfharinger, Geoff Holmes, Talel Abdessalem. Adaptive random forests for evolving data stream classification. In Machine Learning, DOI: 10.1007/s10994-017-5642-8, Springer, 2017.


* **Weather** (weather.csv)

  *Type: Binary classification*
  
  Contains weather information collected between 1949 and 1999 in Bellevue, Nebraska. The objective is to predict if it will rain or not on a given date.
  > R. Elwell, R. Polikar, "Incremental learning of concept drift in nonstationary environments", IEEE Transactions on Neural Networks, vol. 22, no. 10, pp. 1517-1531, Oct 2011.
  
---

## Deprecated

SEA datasets (sea_big.csv, sea_stream.csv) were created using the `SEAGenerator`. The recommended approach is to use the `SEAGenerator` directly.
