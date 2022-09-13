# Objective
I am learning about Knowledge Graphs and how this can be cohesively integrated with Recommender Systems (Personalization).  At this year's academic conference RecSys, there is a tutorial on explainable recommender systems using Knowledge Graphs.  The goal is to replicate what I learn in terms of the recent advances on the development and evaluation of explainable recommender systems with knowledge graphs.

# Knowledge Graphs @ RecSys 2022
* ExpRecSys -> [Explainable RecSys](https://explainablerecsys.github.io/recsys2022/)
* KaRS -> [Knowledge-aware and Conversational Recommender Systems](https://kars-workshop.github.io/2022/]

# Prereqs
* ExpRecSys (tutorial)
  * Download the following data sources and store their respective files under /data/{source_name}/ (e.g. source_name=movielens-1m):
    * [MovieLens-1M (ML1M)](https://grouplens.org/datasets/movielens/1m/)
    * [music (LastFM-1B (LASTFM))](www.cp.jku.at/datasets/LFM-1b) # NOTE: It is 8GB
      * Paper outlining how to obtain the data using Python: [PDF Link](http://www.cp.jku.at/people/schedl/Research/Publications/pdf/schedl_icmr_2016.pdf)
    * [e-commerce (Amazon-Cellphones)](https://www.kaggle.com/datasets/grikomsn/amazon-cell-phones-reviews) # Source Link to be confirmed at the conference
* KARS (workshop)
  * none


# Textual explanations using PGPR and CAFE

## What is PGPR?
* Yikun Xian (et al) proposed a method called Policy-Guided Path Reasoning (PGPR)
* This method couples recommendation and interpretability by providing actual paths in a knowledge graph.
* Paper and GitHub source located [HERE](https://github.com/orcax/PGPR)

## What is CAFE?
* Agustín Borrego (et al) proposed a method called Completion using Neighborhood-Aware Features
* CAFE helps generate feature vectors using context-aware features as well as the datasets downloaded in the pre-req
* Paper and GitHub source located [HERE](https://github.com/DEAL-US/CAFE)
```
@article{borrego2021CAFE,
  author = {Borrego, Agust{\'i}n and Ayala, Daniel and Hern{\'a}ndez, Inma and Rivero, Carlos R. and Ruiz, David},
  title = {{CAFE}: Knowledge graph completion using neighborhood-aware features},
  journal = {Engineering Applications of Artificial Intelligence},
  volume = {103},
  pages = {104302},
  year = {2021},
  issn = {0952-1976},
  doi = {10.1016/j.engappai.2021.104302},
  url = {https://www.sciencedirect.com/science/article/pii/S0952197621001500}
}
```