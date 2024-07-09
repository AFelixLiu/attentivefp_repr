# README

This repo is a local reproduction of AttentiveFP, with code and data from [OpenDrugAI/AttentiveFP (github.com)](https://github.com/OpenDrugAI/AttentiveFP)



**Notice**

There are some modifications in File `Feature_visualization_of_Learning_aromaticity.ipynb` Cell 8.

* The first change is as follows,

  ```python
  # if test_MSE < 0.5:  # modified by AFelixLiu on 10 July 2024
  if test_MSE < 1.1:    # modified by AFelixLiu on 10 July 2024
  ```

* The second change is as follows,

  ```py
  # if (epoch - best_param["train_epoch"] >2) and (epoch - best_param["test_epoch"] >8):  # modified by AFelixLiu on 10 July 2024
  if (epoch - best_param["train_epoch"] >2) and (epoch - best_param["test_epoch"] >18):   # modified by AFelixLiu on 10 July 2024
  ```



**How to run this repo**

1. Configure the environment according to file `requirements.txt`.

2. Enter the following code at the terminal and run it,

   ```bash
   bash ./run
   ```

   *You can run the part of the tasks by modifying the `run` file*



> AttentiveFP were introduced in the publication [Pushing the Boundaries of Molecular Representation for Drug Discovery with the Graph Attention Mechanism | Journal of Medicinal Chemistry (acs.org)](https://pubs.acs.org/doi/abs/10.1021/acs.jmedchem.9b00959).

