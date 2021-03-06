# leiden
_cluster graph(s) with the leiden algorithm_

## Usage

This is a wrapper script around `vtraag's` [Leiden Algorithm](https://github.com/vtraag/leidenalg). Put this script in your path, and then you can call from anywhere!

```bash

# get a graph
wget https://github.com/twesleyb/leiden/raw/master/data/adjm.zip

unzip adjm.zip && cd adjm/

# cluster the graph with the leiden algorithm and surprise
leiden adjm.csv -q Surprise 

# or try the CPM algorithm
leiden adjm.csv -q CPM -g 1

# NOTE: currently only supports a single resolution!
```

## Dependencies
I recommend using a virtual environment such as conda:
* leidenalg -- `conda install -c conda-forge leidenalg`
* igraph -- `conda install -c conda-forge leidenalg`
