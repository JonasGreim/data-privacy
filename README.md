# K-Anonymity, L-Diversity, T-Closeness on numerical or categorial Data
Look into this jupyther notebook [data-privacy-methods.ipynb](./data-privacy-methods.ipynb) -> results are pre-rendered

## own setup
- install conda 
- conda create --name myenv python=3.7
- conda activate myenv
- conda install pandas==0.25
- conda install matplotlib
#
- set the python  interpreter/kernel = myenv    in your favourite IDE (in which should run jupyter notebook)
- run the jupyter notebook
#
- change privacy methods parameter (kAnonym, lDivers, tClose)
- you can choose if your numeric data partitions should be displayed as a range or as an average
- categorial data are always displayed as unique sets
#
#### You can also add another display function like suppression 
- in "Enter dataset & privacy parameters"
    - add dataColumnDisplayedDifferently = set(('YourChosenColumn',))
- in the "Generating anonymous Dataset" section:
    - add your custom function there
- in build_anonymized_dataset() function:
    - add an ifel condition for your dataColumnDisplayedDifferently set
