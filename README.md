# Predicting properties of materials

The purpose of this project was to explore different Machine Learning algorithms for predicting
the formation energy of atoms using only the geometric configuration. The data used were
exported from the [Materials Projects](https://materialsproject.org/) library. For computational
matters, all the models developed are at most limited on predicting the formation energy for 
atoms that contain Carbon atoms and whose atomic number is less than 40.  
\
The file `Predictors` contains notebooks and needed files for the prediction:
- `atoms.npy` : Contains the list of vectorized atoms that will be used in the prediction
- `dataFormEnCif_with_Carbone.txt`: The information about the geometric configuration of atoms that we got
from the materials library.
- `Materials_energy.csv`: Data about the formation energy of concerned atoms
- `Prediction_Carbone.npy` : Predicting the formation energy for atoms that are formed uniquely 
from Carbon atoms (smaller  dataset).
- `Prediction_Coulomb.npy` : Prediction models that uses all the data available. Coulomb matrix is the representation 
of atoms is used here .
- `Prediction_Soap.npy`: Prediction models that uses all the data available but using the soap vector of the atom rather
than the Coulomb matrix