# Credit Risk Model
Binary classification problem that used tree-based models and ensemble learning. The dataset is from a [Data mining course](https://www.cs.upc.edu/~belanche/Docencia/mineria/mineria.html) through Polytechnic University of Catalonia with the original csv located at [CreditScoring github project](https://github.com/gastonstat/CreditScoring/).

### Data
The initial dataset has the following schema:
  - status: whether the customer managed to pay back the loan (1) or not (2)
  - seniority: job experience in years
  - home: type of homeownership: renting (1), a homeowner (2), and others
  - time: period planned for the loan (in months)
  - age: age of the client
  - marital [status]: single (1), married (2), and others
  - records: whether the client has any previous records: no (1), yes (2) (It’s not clear from the dataset description what kind of records we have in this column. For the purposes of this project, we may assume that it’s about records in the bank’s database.)
  - job: type of job: full-time (1), part-time (2), and others
  - expenses: how much the client spends per month
  - income: how much the client earns per month
  - assets: total worth of all the assets of the client
  - debt: amount of credit debt
  - amount: requested amount of the loan
  - price: price of an item the client wants to buy

### Technologies used
  - Python 3.10
  - Scikit-learn
  - Pandas
  - Numpy
  - Seaborn
  - Matplotlib

### Techniques used
**One-Hot Encoding**: Instead of using Pandas `get_dummies()` method to create the one-hot columns in the dataset. I instead used `scikit-learn's` `DictVectorizer` method