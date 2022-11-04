# Cycling desire line analysis

This is the source code for the scientific paper [*Computational desire line analysis of cyclists on the Dybbølsbro intersection in Copenhagen*](https://arxiv.org/abs/2211.01301) by S. Breum, B. Kostic, and [M. Szell](http://michael.szell.net/). The code applies DBSCAN and Dynamic Time Warping to analyze
patterns in cyclist behaviour with a data set of 11,553 cyclist trajectories, which had been extracted via a custom-trained YOLO from a high-resolution 1h video from June 2021 of the [https://www.openstreetmap.org/#map=19/55.66524/12.55843](Dybbølsbro intersection).

**Paper (preprint)**: [https://arxiv.org/abs/2211.01301](https://arxiv.org/abs/2211.01301)  


## Setting up code environment
The code environment has been successfully tested on the following operating system: 
`Ubuntu 20.04.3 LTS (GNU/Linux 4.4.0-19041-Microsoft x86_64)`

To set up the code environment, run:


```
conda env create -f=environment.yml
conda activate desirelines
conda install -c conda-forge ipywidgets
pip install --user ipykernel
python -m ipykernel install --user --name=desirelines
```
Download and unpack data folder from [https://zenodo.org/record/7288616](https://zenodo.org/record/7288616)

Then, run Jupyter Notebook with kernel desirelines (Kernel > Change Kernel > desirelines)
