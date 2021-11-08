### Problem Statement
Classification analysis of the late Kobe Bryant's shot selection details. Can an analysis of Kobe Bryant's shot selection details predict whether he made a shot?

---

### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**data.csv**|*float,integer,objects*|Kaggle - Kobe Bryant Shot Selection|A collection of location and circumstances of every field goal attempted by Kobe Bryant took during his 20-year career. | 

---

### Brief summary of analysis

* EDA

* Random Forest

* Neural Network (Baseline) - feed forward - 47,1

* Neural Network (30 neuron layer) - feed forward - 47,30,1

---

### Findings

#### RF/ETC baseline model

* RF training accuracy - 0.6028584217472226

* ETC training accuracy - 0.6077666778923299

#### RF grid search model

* RF best score (0.6324387611773175) 

* best params {'max_depth': 7, 'min_samples_split': 3, 'n_estimators': 150})


* RF train/test accuracy - (0.6385196768308574, 0.6297068403908794)


* RF R^2 - -0.5823782534283344

#### NN baseline model

* NN train/test accuracy -(0.6480756163597107,0.649422025680542)


* NN R^2 score - -0.5057041362421109

#### NN w/ one layer model

* NN train/test accuracy w/ layers - (0.6459035873413086,0.637263834476471)


* NN R^2 score w/ layers - -0.5178602797273681


#### EDA

* The years he made most of his shots had many nulls

* The nulls seem to match the number of games he played. 


### Future anlysis

* Would like to use groupby sum and count to see if there were any 

* Conduct a variable correlation