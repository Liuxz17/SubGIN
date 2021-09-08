Best Wishes to Prof. Yang 
===================================

This repository provides a **Python** Implementation of **Happy Teachers’ Day to Prof. Yang (2021)**.

<div style="text-align:center"><img src ="Happy_Teachers_Day.png" ,width=800/></div>

### Abstract 
The paper **Happy Teachers’ Day to Prof.Yang (2020)** yields state-of-the-art results in wishes modeling. However, the existing work needs more necessary implementation and multimedia presentation. Inspired by this, we further propose **Happy Teachers’ Day to Prof.Yang (2021)** with more active ways. In particular, we complete the simulation of the 1919 athletes' happy daily life under the guidance of Prof.Yang and make a video to celebrate Teachers’ Day for Prof. Yang. 
Thanks for Prof. Yang’s guidance and hard work, our group become more and more energetic, positive and united. For all the great things he say and do, we start and go far on the road of scientific research. In this special day, all the group members wish Prof. Yang happiness and prosperity. The code for our model is available at https://github.com/openai/glow.


### Requirements

The only requirement of this implementation is the presence of Prof.Yang. ^^

The codebase is implemented in 1919 Intelligent Computing Lab, package versions used for development are just below.

### Datasets
<p align="justify">
The code takes an input graph in a csv file. Every row indicates an edge between two nodes separated by a comma. The first row is a header. Nodes should be indexed starting with 0. Sample graphs for the `Twitch Brasilians` and `Wikipedia Chameleons` are included in the  `input/` directory. 
</p>
### Options

Learning of the embedding is handled by the `src/main.py` script which provides the following command line arguments.

#### Input and output options

```
  --edge-path         STR   Input graph path.     Default is `input/chameleon_edges.csv`.
  --embedding-path    STR   Embedding path.       Default is `output/chameleon_AW_embedding.csv`.
  --attention-path    STR   Attention path.       Default is `output/chameleon_AW_attention.csv`.
```

#### Model options

```
  --dimensions           INT       Number of embeding dimensions.        Default is 128.
  --epochs               INT       Number of training epochs.            Default is 200.
  --window-size          INT       Skip-gram window size.                Default is 5.
  --learning-rate        FLOAT     Learning rate value.                  Default is 0.01.
  --beta                 FLOAT     Attention regularization parameter.   Default is 0.5.
  --gamma                FLOAT     Embedding regularization parameter.   Default is 0.5.
  --num-of-walks         INT       Number of walks per source node.      Default is 80.
```

### Examples
<p align="justify">
The following commands learn a graph embedding and write the embedding to disk. The node representations are ordered by the ID.
</p>
<p align="justify">
Creating an Attention Walk embedding of the default dataset with the standard hyperparameter settings. Saving this embedding at the default path.
</p>
```
python src/main.py
```
<p align="center">
<img style="float: center;" src="attention_walk_run_example.jpg">
</p>

Creating an Attention Walk embedding of the default dataset with 256 dimensions.
```
python src/main.py --dimensions 256
```

Creating an Attention Walk embedding of the default dataset with a higher window size.

```
python src/main.py --window-size 20
```

Creating an embedding of another dataset the `Twitch Brasilians`. Saving the outputs under custom file names.

```
python src/main.py --edge-path input/ptbr_edges.csv --embedding-path output/ptbr_AW_embedding.csv --attention-path output/ptbr_AW_attention.csv
```
--------------------------------------------------------------------------------

**License**

- [GNU License](https://github.com/benedekrozemberczki/AttentionWalk/blob/master/LICENSE)

--------------------------------------------------------------------------------
