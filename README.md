# StochasticGhost
Algorithm for Solving Empirical Risk Minimization Problems with Constraints.
The module will be an installable dependency which is backend agnostic and can take an objective and any number of constraints.
The objective and constraints should be continuously differentiable functions.
The package has a series of notebooks which show the algorithm's performance on benchmark datasets like: Propublica COMPAS, Adult Income.
Unit tests are also performed over MNIST and CIFAR-10 datasets which are available as python scripts in the test folder.
The ojective can be the loss of a ML model such as Neural Net and constraints can be some empirical risk measure.

<br>
NOTE:As a matter of civic responsibility, the authors of the ghostFair software package wish to declare that any use of the package to enforce demographic parity or any fairness metric oriented towards active discrimination for the sake of social engineering, as espoused by the ideology of DEI is fundamentally nefarious and declare their firm opposition to such policy. Furthermore, as it will inevitably lead to only disastrous outcomes, the purveyors of ghostFair will not actively cooperate or support any entity who wishes to use this software for such destructive purposes.

## Setup Instructions

To install and use this package, follow these steps:

# 1. Clone this repository to your local machine:

   $git clone project_url
   $cd your_project

# 2. Create a virtual environment with python 3.10
  ### using python venv
   
   $python3.10 -m venv myenv

   Activate the virtual environment
   
   $source myenv/bin/activate

  ### using conda environments

   $conda create -n myenv python=3.10

   Activate the conda environment
   
   $source activate myenv

# 3. To build manually (installs all dependencies)

   $cd StochasticGhost
   
   $pip install wheel
   
   $python setup.py bdist_wheel
   
   $pip install dist/StochasticGhost-0.1.0-py3-none-any.whl
