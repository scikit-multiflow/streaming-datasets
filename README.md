# Streaming data sets

This repository contains a collection of datasets. While some data sets are used for batch learning they can be also be used in the streaming setting. On the other hand, some data sets have characteristics that make them better suited for the stream learning setting, e.g., they contain non-stationary data.

*  **Covertype Dataset** (covtype.csv)

   *Type: Multi-class classification*
   
   This data set contains data collected over time by the US Forest Service. Classes correspond to cover type in forest on squares of 30×30 meters.
   > Blackard, Jock A. and Denis J. Dean. 2000. "Comparative Accuracies of Artificial Neural Networks and Discriminant Analysis in Predicting Forest Cover Types from Cartographic Variables." Computers and Electronics in Agriculture 24(3):131-151.

* **Electricity Market Dataset** (elec.csv)

  *Type: Binary classification*
  
  Data from the Australian New South Wales electricity market where prices are not fixed but change based on offer and demand. The 2 target classes represent changes in the price (1=up or 0=down).
  > M. Harries, N.S. Wales, Splice-2 comparative evaluation: Electricity pricing, 1999.

  *Notes:* This version does not include the attributes 'date' and 'day'.

* **Moving Squares Dataset** (moving_squares.csv)

  *Type: Multi-class classification*
  
  Four equidistantly separated, squared uniform distributions are moving in horizontal direction with constant speed. The direction is inverted whenever the leading square reaches a predefined boundary. Each square represents a different class. The added value of this dataset is the predefined time horizon of 120 examples before old instances may start to overlap current ones. This is especially useful for dynamic sliding window approaches, allowing to test whether the size is adjusted accordingly.
  > Losing, V., Hammer, B. and Wersing, H., 2016, December. Knn classifier with self adjusting memory for heterogeneous concept drift. In Data Mining (ICDM), 2016 IEEE 16th International Conference on (pp. 291-300). IEEE.

* **Music (emotions) Dataset** (music.csv)

  *Type: Multi-label classification*
  
  593 songs with 6 clusters of music emotions based on the Tellegen-Watson-Clark model.
  > Read, J., Reutemann, P., Pfahringer, B. and Holmes, G., 2016. Meka: a multi-label/multi-target extension to weka. The Journal of Machine Learning Research, 17(1), pp.667-671.
  
  > K. Trohidis, G. Tsoumakas, G. Kalliris, I. Vlahavas. "Multilabel Classification of Music into Emotions". Proc. 2008 International Conference on Music Information Retrieval (ISMIR 2008), pp. 325-330, Philadelphia, PA, USA, 2008.

* **Weather Dataset** (weather.csv)

  *Type: Binary classification*
  
  Contains weather information collected between 1949 and 1999 in Bellevue, Nebraska. The objective is to predict if it will rain or not on a given date.
  > R. Elwell, R. Polikar, "Incremental learning of concept drift in nonstationary environments", IEEE Transactions on Neural Networks, vol. 22, no. 10, pp. 1517-1531, Oct 2011.

* **Iris Dataset (with artificial timestamps)** (iris_dataset.csv)

  *Type: Multi-class classification*
  
  Description of the original dataset from the UCI repository: "The data set contains 3 classes of 50 instances each, where each class refers to a type of iris plant. One class is linearly separable from the other 2; the latter are NOT linearly separable from each other."

  > Fisher, Rory A. "The use of multiple measurements in taxonimic problems." (1936).
  
---

## Deprecated

SEA datasets (sea_big.csv, sea_stream.csv) were created using the `SEAGenerator`. The recommended approach is to use the `SEAGenerator` directly.
