# Spkie Sorting using Klusta 

This is a short tutorial for using Klusta (Rossant et al., 2016) 

## Getting Started

[Install miniconda](https://docs.conda.io/en/latest/miniconda.html)

[Download yml file](https://raw.githubusercontent.com/kwikteam/klusta/master/installer/environment.yml)

[Download sample raw data and sample parameter file](https://klusta.readthedocs.io/en/latest/#installation)

In your terminal (cmd for windows), cd to the directory where you stored your files, and enter the following command
```
conda env create -n klusta -f environment.yml
```

After successful installation, try running the sample spike sorting 
```
source activate klusta  # omit the `source` on Windows
klusta hybrid_10sec.prm  # spikesort your data with a PRM file
```

After seeing "Clustering done!", you can visualize the results
```
phy kwik-gui hybrid_10sec.kwik # open the GUI to see results
```

Now you can modify the prm and dat files for our data and try sorting the spikes.



## See also

* [Klusta github](https://github.com/kwikteam/klusta)
* [Hanyu's notes from last year](https://gist.github.com/Hanyu-Li/37012b812c967c6381397b98c667faaf)
