# Data Folder

This folder contains the tabular datasets used in Assignment 4.

---

## 1. `classification_DATA.csv`

This dataset is a loan classification dataset.

Shape:

```text
44,993 rows × 38 columns
```

Main columns:

* Applicant information
* Income information
* Loan amount
* Loan interest rate
* Credit score
* Loan intent
* Home ownership
* Engineered features
* Target column: `loan_status`

Target:

```text
loan_status
```

This column is used for binary classification.

Possible meaning:

* `0`: loan is not approved or low-risk class
* `1`: loan is approved or high-risk class

This dataset is used in:

* ML Pipeline notebook
* Optional End-to-End Workflow notebook

There are no missing values and no duplicate rows in this file.

---

## 2. `Data.csv`

This dataset is a real estate rental dataset.

Shape:

```text
12,383 rows × 9 columns
```

Columns:

* `total_value`
* `neighborhood`
* `area`
* `year`
* `deposit`
* `rent`
* `elavator`
* `parking`
* `warehouse`

This dataset contains information about rental houses or apartments.

Main features:

* Location
* Area
* Building year
* Deposit
* Rent
* Elevator availability
* Parking availability
* Warehouse availability

This dataset is used in the imbalanced data notebook.

In that notebook, the `parking` column is used to create an imbalanced target:

```text
no_parking = 1 - parking
```

There are no missing values and no duplicate rows in this file.

---

## Notes

* Both datasets are already cleaned.
* Some categorical columns are already encoded in `classification_DATA.csv`.
* `Data.csv` still has one text column: `neighborhood`.
* The CSV files should stay inside the `data/` folder.
