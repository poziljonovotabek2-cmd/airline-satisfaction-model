# Airline Passenger Satisfaction Model

A locally trained Random Forest classifier for predicting airline passenger satisfaction. The serialized model was produced by the `Airline Module.ipynb` notebook in the author's Scikit project.

## Model file

`airline_passanger_satisfaction.joblib` is stored with Git LFS because it is larger than GitHub's regular Git file limit. Install Git LFS before cloning or pulling the model:

```bash
git lfs install
git clone https://github.com/poziljonovotabek2-cmd/airline-satisfaction-model.git
cd airline-satisfaction-model
git lfs pull
```

## Important

The notebook encoded categorical columns with `LabelEncoder` before fitting the classifier. Inference code must reproduce those same category-to-integer mappings and use the same feature order. The fitted preprocessing encoders were not saved as part of this model artifact, so the `.joblib` file alone is not a complete prediction pipeline.

Only load this file if you trust its source: Joblib uses Python pickle serialization, which can execute code while loading.

The training CSV and notebook are not included. Check the original dataset's usage terms before redistributing it or derived artifacts. No model license is specified yet.
