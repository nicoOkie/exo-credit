# Exercire en binôme sur la prédiction de crédit

## 1er test

- Modèle DeepNet
- Split Full-train -> 80% Training data, 20% Validation data
- Seuil : 0.5
- FN : 1655
- FP : 357

## 2e test

- Ajout d'une feature Ratio *MonthlyIncome*/*NumberOfDependents*
  - TrainFull -> Split Train/Val
    - Si opti => Ne pas oublier de le faire sur **Test Dataset**
- Remplacer NA dans *MonthlyIncome* et *NumberOfDependents*

- Modèle DeeptNet
  - FN : 1755
  - FP : 198 => amélioration

## 3e Test

- ajouter colones
  - IsOld (>= 70)
  - Calcul MonthlyDebt et MonthlyBalance
  - NumberOfTimeLate30DaysOrMore

## 4e test

- modif colone `MonthlyDebt` => si `MonthlyIncome` = 0 pour avoir une *debt* dans `MonthlyDebt`
- modif du `IncomePerPersone` basé sur `MonthlyBalance` plutôt que sur `MonthlyIncome`
