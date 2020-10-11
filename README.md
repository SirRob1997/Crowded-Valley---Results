# Descending through a Crowded Valley - Benchmarking Deep Learning Optimizers

[Robin M. Schmidt](https://scholar.google.de/citations?user=20vb63kAAAAJ&hl=de), [Frank Schneider](https://scholar.google.com/citations?user=znq-WkAAAAAJ&hl=en), and [Philipp Hennig](https://scholar.google.de/citations?user=UeG5w08AAAAJ&hl=en)

**Paper**: http://arxiv.org/abs/2007.01547

> **Abstract:** *Choosing the optimizer is considered to be among the most crucial decisions of deep learning engineers, and it is not an easy one. The growing literature now lists hundreds of optimization methods. In the absence of clear theoretical guidance and conclusive empirical evidence, the decision is often made based on personal anecdotes. In this work, we aim to replace these anecdotes, if not with a conclusive ranking, then at least with evidence-backed heuristics. To do so, we perform an extensive, standardized benchmark of more than a dozen particularly popular deep learning optimizers while giving a concise overview of the wide range of possible choices. Analyzing almost 35,000 individual runs, we contribute the following three points: (i) Optimizer performance varies greatly across tasks. (ii) We observe that evaluating multiple optimizers with default parameters works approximately as well as tuning the hyperparameters of a single, fixed optimizer. (iii) While we can not discern an optimization method clearly dominating across all tested tasks, we identify a significantly reduced subset of specific algorithms and parameter choices that generally lead to competitive results in our experiments. This subset includes popular favorites and some lesser-known contenders. We have open-sourced all our experimental results, making them directly available as challenging and well-tuned baselines. This allows for more meaningful comparisons when evaluating novel optimization methods without requiring any further computational efforts.*


## Evaluation

For a full evaluation with all our plots and explanations, please look at the paper.

<img src = "https://i.imgur.com/450YoFl.png" >

<img src = "https://i.imgur.com/Yu96SyP.png" >

## Citation
If you use our results, please consider citing:

```bibtex
@misc{schmidt2020descending,
    title={Descending through a Crowded Valley - Benchmarking Deep Learning Optimizers},
    author={Robin M. Schmidt and Frank Schneider and Philipp Hennig},
    year={2020},
    eprint={2007.01547},
    archivePrefix={arXiv},
    primaryClass={cs.LG}
}
```
    
## Contact
Should you have any question, please feel free to contact the authors.
