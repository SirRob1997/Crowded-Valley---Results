# Descending through a Crowded Valley - Benchmarking Deep Learning Optimizers

[Robin M. Schmidt](https://scholar.google.de/citations?user=20vb63kAAAAJ&hl=de), [Frank Schneider](https://scholar.google.com/citations?user=znq-WkAAAAAJ&hl=en), and [Philipp Hennig](https://scholar.google.de/citations?user=UeG5w08AAAAJ&hl=en)

**Paper**: http://arxiv.org/abs/2007.01547

> **Abstract:** *Choosing the optimizer is considered to be among the most crucial design decisions in deep learning, and it is not an easy one. The growing literature now lists hundreds of optimization methods. In the absence of clear theoretical guidance and conclusive empirical evidence, the decision is often made based on anecdotes. In this work, we aim to replace these anecdotes, if not with a conclusive ranking, then at least with evidence-backed heuristics. To do so, we perform an extensive, standardized benchmark of more than a dozen particularly popular deep learning optimizers while giving a concise overview of the wide range of possible choices. Analyzing almost 35,000 individual runs, we contribute the following three points: (i) Optimizer performance varies greatly across tasks. (ii) We observe that evaluating multiple optimizers with default parameters works approximately as well as tuning the hyperparameters of a single, fixed optimizer. (iii) While we can not discern an optimization method clearly dominating across all tested tasks, we identify a significantly reduced subset of specific algorithms and parameter choices that generally lead to competitive results in our experiments. This subset includes popular favorites and some lesser-known contenders. We have open-sourced all our experimental results, making them directly available as challenging and well-tuned baselines. This allows for more meaningful comparisons when evaluating novel optimization methods without requiring any further computational efforts.*


## Evaluation

For a full evaluation with all our plots and explanations, please look at the paper.

<img src = "https://i.imgur.com/450YoFl.png" >

<img src = "https://i.imgur.com/Yu96SyP.png" >

## List of Optimizers
We keep a somewhat updated list of optimizers which can be used for Deep Learning, if you want to add any method, please create a pull request:
* ACClip, *2019* (https://arxiv.org/abs/1912.01823)
* ADAHESSIAN, *2020* (https://arxiv.org/abs/2006.00719)
* ALI-G, *2020* (https://arxiv.org/abs/1906.05661)
* AMSBound, *2019* (https://arxiv.org/abs/1902.09843)
* AMSGrad, *2018* (https://arxiv.org/abs/1904.09237)
* ARSG, *2019* (https://arxiv.org/abs/1905.01422)
* AcceleGrad, *2018* (https://arxiv.org/abs/1809.02864)
* AdaAlter, *2019* (https://arxiv.org/abs/1911.09030)
* AdaBatch, *2017* (https://arxiv.org/abs/1712.02029)
* AdaBayes, *2018* (https://arxiv.org/abs/1807.07540v4)
* AdaBayes-SS, *2018* (https://arxiv.org/abs/1807.07540v4)
* AdaBlock, *2019* ("https://arxiv.org/abs/1905.10757)
* AdaBound, *2019* (https://arxiv.org/abs/1902.09843)
* AdaComp, *2018* (https://arxiv.org/abs/1712.02679)
* AdaFTRL, *2015* (https://arxiv.org/abs/1502.05744)
* AdaFix, *2019* (https://arxiv.org/abs/1911.00289)
* AdaFom, *2019* (https://arxiv.org/abs/1808.02941)
* AdaLoss, *2019* (https://arxiv.org/abs/1908.01070)
* AdaMax, *2015* (https://arxiv.org/abs/1412.6980)
* AdaMod, *2019* (https://arxiv.org/abs/1910.12249)
* AdaSGD, *2020* (https://arxiv.org/abs/2006.16541)
* AdaShift, *2019* (https://arxiv.org/abs/1810.00143)
* AdaSqrt, *2019* (https://arxiv.org/abs/1912.09926)
* AdaX, *2020* (https://arxiv.org/abs/2004.09740)
* AdaX-W, *2020* (https://arxiv.org/abs/2004.09740)
* Adadelta, *2012* (https://arxiv.org/abs/1212.5701)
* Adagrad, *2011* (http://jmlr.org/papers/v12/duchi11a.html)
* Adam, *2015* (https://arxiv.org/abs/1412.6980)
* AdamAL, *2019* (https://openreview.net/forum?id=SyxM51BYPB)
* AdamBS, *2020* (https://arxiv.org/abs/2010.12986)
* AdamNC, *2018* (https://arxiv.org/abs/1904.09237)
* AdamT, *2020* (https://arxiv.org/abs/2001.06130)
* AdamW, *2019* (https://arxiv.org/abs/1711.05101)
* AdamX, *2019* (https://arxiv.org/abs/1904.03590)
* Adathm, *2019* (https://ieeexplore.ieee.org/abstract/document/8923615)
* ArmijoLS, *2019* (https://arxiv.org/abs/1905.09997)
* AvaGrad, *2019* (https://arxiv.org/abs/1912.01823)
* BAdam, *2018* (https://arxiv.org/abs/1811.03679)
* BGAdam, *2019* (https://arxiv.org/abs/1908.08015)
* BRMSProp, *2018* (https://arxiv.org/abs/1807.07540v2)
* BSGD, *2020* (https://arxiv.org/abs/2002.10790)
* C-ADAM, *2020* (https://arxiv.org/abs/2002.03755)
* CProp, *2019* (https://arxiv.org/abs/1912.11493)
* CoolMomentum, *2020* (https://arxiv.org/abs/2005.14605)
* Curveball, *2019* (https://arxiv.org/abs/1805.08095)
* Dadam, *2019* (https://arxiv.org/abs/1901.09109v6)
* DeepMemory, *2020* (https://forums.fast.ai/t/new-optimizer-deepmemory/60983)
* DiffGrad, *2020* (https://arxiv.org/abs/1909.11015)
* Eve, *2017* (https://arxiv.org/abs/1611.0150)
* Gadam, *2018* (https://arxiv.org/abs/1805.07500)
* GOLS-I, *2019* (https://arxiv.org/abs/1903.09383)
* Gravilon, *2020* (https://arxiv.org/abs/2008.11370)
* HAdam, *2019* (https://arxiv.org/abs/1910.06878)
* HyperAdam, *2019* (https://arxiv.org/abs/1811.08996)
* K-BFGS, *2020* (https://arxiv.org/abs/2006.08877)
* K-BFGS(L), *2020* (https://arxiv.org/abs/2006.08877)
* KFAC, *2015* (https://arxiv.org/abs/1503.05671)
* KFLR, *2017* (https://arxiv.org/abs/1706.03662)
* KFRA, *2017* (https://arxiv.org/abs/1706.03662)
* L4Adam, *2018* (https://arxiv.org/abs/1802.05074)
* L4Momentum, *2018* (https://arxiv.org/abs/1802.05074)
* LAMB, *2020* (https://arxiv.org/abs/1904.00962)
* LaProp, *2020* (https://arxiv.org/abs/2002.04839)
* LARS, *2017* (https://arxiv.org/abs/1708.03888)
* LookAhead, *2019* (https://arxiv.org/abs/1907.08610)
* M-SVAG, *2018* (https://arxiv.org/abs/1705.07774)
* MTAdam, *2020* (https://arxiv.org/abs/2006.14683)
* Momentum Nesterov, *1983* (http://mpawankumar.info/teaching/cdt-big-data/nesterov83.pdf)
* Momentum Polyak, *1964* (https://vsokolov.org/courses/750/2018/files/polyak64.pdf)
* MVRC-1, *2020* (https://arxiv.org/abs/2005.07755)
* MVRC-2, *2020* (https://arxiv.org/abs/2005.07755)
* NAMSB, *2019* (https://arxiv.org/abs/1905.01422v4)
* NAMSG, *2019* (https://arxiv.org/abs/1905.01422v4)
* ND-Adam, *2017* (https://arxiv.org/abs/1709.04546)
* Nadam, *2016* (https://openreview.net/forum?id=OM0jvwB8jIp57ZJjtNEZ)
* Noisy Adam, *2018* (https://arxiv.org/abs/1712.02390)
* Noisy K-FAC, *2018* (https://arxiv.org/abs/1712.02390)
* NosAdam, *2019* (https://arxiv.org/abs/1805.07557)
* Novograd, *2019* (https://arxiv.org/abs/1905.11286)
* PAGE, *2020* (https://arxiv.org/abs/2008.10898)
* PAL, *2019* (https://arxiv.org/abs/1903.11991v2)
* Padam, *2020* (https://arxiv.org/abs/1806.06763)
* PolyAdam, *2019* (https://arxiv.org/abs/1907.01678)
* PowerSGD, *2019* (https://arxiv.org/abs/1905.13727)
* PowerSGDM, *2019* (https://arxiv.org/abs/1905.13727)
* ProbLS, *2018* (https://arxiv.org/abs/1502.02846)
* PStorm, *2020* (https://arxiv.org/abs/2006.00425)
* QHAdam, *2019* (https://arxiv.org/abs/1810.06801)
* QHM, *2019* (https://arxiv.org/abs/1810.06801)
* RAdam, *2020* (https://arxiv.org/abs/1908.03265)
* RMSProp, *2012* (https://www.cs.toronto.edu/~tijmen/csc321/slides/lecture_slides_lec6.pdf)
* RMSterov, *2019* (https://arxiv.org/abs/1910.05446)
* Ranger, *2020* (https://medium.com/@lessw/new-deep-learning-optimizer-ranger-synergistic-combination-of-radam-lookahead-for-the-best-of-2dc83f79a48d)
* RangerLars, *2020* (https://github.com/mgrankin/over9000)
* SAMSGrad, *2019* (https://arxiv.org/abs/1908.00700)
* SAdam, *2020* (https://arxiv.org/abs/1905.02957)
* SC-Adagrad, *2017* (https://arxiv.org/abs/1706.05507)
* SC-RMSProp, *2017* (https://arxiv.org/abs/1706.05507)
* SDProp, *2017* (https://arxiv.org/abs/1605.09593)
* SGD, *1951* (https://projecteuclid.org/download/pdf_1/euclid.aoms/1177729586)
* SGD-BB, *2016* (https://arxiv.org/abs/1605.04131)
* SGD-G2, *2020* (https://arxiv.org/abs/2002.09304)
* SGDM, *2020* (https://arxiv.org/abs/2006.00423)
* SGDP, , *2020* (https://arxiv.org/abs/2006.08217)
* SGDR, *2017* (https://arxiv.org/abs/1608.03983)
* SHAdagrad, *2020* (https://arxiv.org/abs/2006.07037)
* SKQN, *2020* (https://arxiv.org/abs/2006.09606)
* S4QN, *2020* (https://arxiv.org/abs/2006.09606)
* SNGM, *2020* (https://arxiv.org/abs/2007.13985)
* SRSGD, *2020* (https://arxiv.org/abs/2002.10583)
* SWATS, *2017* (https://arxiv.org/abs/1712.07628)
* SWNTS, *2019* (https://arxiv.org/abs/1905.01422v4)
* Sadam, *2019* (https://arxiv.org/abs/1908.00700)
* Shampoo, *2018* (https://arxiv.org/abs/1802.09568)
* SignAdam++, *2019* (https://arxiv.org/abs/1907.09008)
* SignSGD, *2018* (https://arxiv.org/abs/1802.04434)
* SoftAdam, *2019* (https://openreview.net/forum?id=Skgfr1rYDH)
* TAdam, *2020* (https://arxiv.org/abs/2003.00179)
* VAdam, *2018* (https://arxiv.org/abs/1806.04854)
* VR-SGD, *2020* (https://arxiv.org/abs/1802.09932)
* WNGrad, *2018* (https://arxiv.org/abs/1803.02865)
* YellowFin, *2019* (https://arxiv.org/abs/1706.03471)
* Yogi, *2018* (http://papers.nips.cc/paper/8186-adaptive-methods-for-nonconvex-optimization.pdf)
* vSGD-b, *2013* (https://arxiv.org/abs/1206.1106)
* vSGD-fd, *2013* (https://arxiv.org/abs/1301.3764)
* vSGD-g, *2013* (https://arxiv.org/abs/1206.1106)
* vSGD-l, *2013* (https://arxiv.org/abs/1206.1106)    


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
