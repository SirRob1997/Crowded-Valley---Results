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
* ACClip (https://arxiv.org/abs/1912.01823)
* ADAHESSIAN (https://arxiv.org/abs/2006.00719)
* ALI-G (https://arxiv.org/abs/1906.05661)
* AMSBound (https://arxiv.org/abs/1902.09843)
* AMSGrad (https://arxiv.org/abs/1904.09237)
* ARSG (https://arxiv.org/abs/1905.01422)
* AcceleGrad (https://arxiv.org/abs/1809.02864)
* AdaAlter (https://arxiv.org/abs/1911.09030)
* AdaBatch (https://arxiv.org/abs/1712.02029)
* AdaBayes (https://arxiv.org/abs/1807.07540v4)
* AdaBayes-SS (https://arxiv.org/abs/1807.07540v4)
* AdaBlock ("https://arxiv.org/abs/1905.10757)
* AdaBound (https://arxiv.org/abs/1902.09843)
* AdaComp (https://arxiv.org/abs/1712.02679)
* AdaFTRL (https://arxiv.org/abs/1502.05744)
* AdaFix (https://arxiv.org/abs/1911.00289)
* AdaFom (https://arxiv.org/abs/1808.02941)
* AdaLoss (https://arxiv.org/abs/1908.01070)
* AdaMax (https://arxiv.org/abs/1412.6980)
* AdaMod (https://arxiv.org/abs/1910.12249)
* AdaSGD (https://arxiv.org/abs/2006.16541)
* AdaShift (https://arxiv.org/abs/1810.00143)
* AdaSqrt (https://arxiv.org/abs/1912.09926)
* AdaX (https://arxiv.org/abs/2004.09740)
* AdaX-W (https://arxiv.org/abs/2004.09740)
* Adadelta (https://arxiv.org/abs/1212.5701)
* Adagrad (http://jmlr.org/papers/v12/duchi11a.html)
* Adam (https://arxiv.org/abs/1412.6980)
* AdamAL (https://openreview.net/forum?id=SyxM51BYPB)
* AdamBS (https://arxiv.org/pdf/2010.12986.pdf)
* AdamNC (https://arxiv.org/abs/1904.09237)
* AdamT (https://arxiv.org/abs/2001.06130)
* AdamW (https://arxiv.org/abs/1711.05101)
* AdamX (https://arxiv.org/abs/1904.03590)
* Adathm (https://ieeexplore.ieee.org/abstract/document/8923615)
* ArmijoLS (https://arxiv.org/abs/1905.09997)
* AvaGrad (https://arxiv.org/abs/1912.01823)
* BAdam (https://arxiv.org/abs/1811.03679)
* BGAdam (https://arxiv.org/abs/1908.08015)
* BRMSProp (https://arxiv.org/abs/1807.07540v2)
* BSGD (https://arxiv.org/abs/2002.10790)
* C-ADAM (https://arxiv.org/abs/2002.03755)
* CProp (https://arxiv.org/abs/1912.11493)
* Curveball (https://arxiv.org/abs/1805.08095)
* Dadam (https://arxiv.org/abs/1901.09109v6)
* DeepMemory (https://forums.fast.ai/t/new-optimizer-deepmemory/60983)
* DiffGrad (https://arxiv.org/abs/1909.11015)
* Eve (https://arxiv.org/abs/1611.0150)
* Gadam (https://arxiv.org/abs/1805.07500)
* GOLS-I (https://arxiv.org/abs/1903.09383)
* Gravilon (https://arxiv.org/abs/2008.11370)
* HAdam (https://arxiv.org/abs/1910.06878)
* HyperAdam (https://arxiv.org/abs/1811.08996)
* K-BFGS (https://arxiv.org/abs/2006.08877)
* K-BFGS(L) (https://arxiv.org/abs/2006.08877)
* KFAC (https://arxiv.org/abs/1503.05671)
* KFLR (https://arxiv.org/abs/1706.03662)
* KFRA (https://arxiv.org/abs/1706.03662)
* L4Adam (https://arxiv.org/abs/1802.05074)
* L4Momentum (https://arxiv.org/abs/1802.05074)
* LAMB (https://arxiv.org/abs/1904.00962)
* LaProp (https://arxiv.org/abs/2002.04839)
* LARS (https://arxiv.org/abs/1708.03888)
* LookAhead (https://arxiv.org/abs/1907.08610)
* M-SVAG (https://arxiv.org/abs/1705.07774)
* MTAdam (https://arxiv.org/abs/2006.14683)
* Momentum Nesterov (http://mpawankumar.info/teaching/cdt-big-data/nesterov83.pdf)
* Momentum Polyak (https://vsokolov.org/courses/750/2018/files/polyak64.pdf)
* MVRC-1 (https://arxiv.org/abs/2005.07755)
* MVRC-2 (https://arxiv.org/abs/2005.07755)
* NAMSB (https://arxiv.org/abs/1905.01422v4)
* NAMSG (https://arxiv.org/abs/1905.01422v4)
* ND-Adam (https://arxiv.org/abs/1709.04546)
* NDadam (https://arxiv.org/abs/1709.04546)
* Nadam (https://openreview.net/forum?id=OM0jvwB8jIp57ZJjtNEZ)
* Noisy Adam (https://arxiv.org/abs/1712.02390)
* Noisy K-FAC (https://arxiv.org/abs/1712.02390)
* NosAdam (https://arxiv.org/abs/1805.07557)
* Novograd (https://arxiv.org/abs/1905.11286)
* PAL (https://arxiv.org/abs/1903.11991v2)
* Padam (https://arxiv.org/abs/1806.06763)
* PolyAdam (https://arxiv.org/abs/1907.01678)
* PowerSGD (https://arxiv.org/abs/1905.13727)
* PowerSGDM (https://arxiv.org/abs/1905.13727)
* ProbLS (https://arxiv.org/abs/1502.02846)
* PStorm (https://arxiv.org/abs/2006.00425)
* QHAdam (https://arxiv.org/abs/1810.06801)
* QHM (https://arxiv.org/abs/1810.06801)
* RAdam (https://arxiv.org/abs/1908.03265)
* RMSProp (https://www.cs.toronto.edu/~tijmen/csc321/slides/lecture_slides_lec6.pdf)
* RMSterov (https://arxiv.org/abs/1910.05446)
* Ranger (https://medium.com/@lessw/new-deep-learning-optimizer-ranger-synergistic-combination-of-radam-lookahead-for-the-best-of-2dc83f79a48d)
* RangerLars (https://github.com/mgrankin/over9000)
* SAMSGrad (https://arxiv.org/abs/1908.00700)
* SAdam (https://arxiv.org/abs/1905.02957)
* SC-Adagrad (https://arxiv.org/abs/1706.05507)
* SC-RMSProp (https://arxiv.org/abs/1706.05507)
* SDProp (https://arxiv.org/abs/1605.09593)
* SGD (https://projecteuclid.org/download/pdf_1/euclid.aoms/1177729586)
* SGD-BB (https://arxiv.org/abs/1605.04131)
* SGD-G2 (https://arxiv.org/abs/2002.09304)
* SGDM (https://arxiv.org/abs/2006.00423)
* SGDP (https://arxiv.org/abs/2006.08217)
* SGDR (https://arxiv.org/abs/1608.03983)
* SHAdagrad (https://arxiv.org/abs/2006.07037)
* SKQN (https://arxiv.org/abs/2006.09606)
* S4QN (https://arxiv.org/abs/2006.09606)
* SNGM (https://arxiv.org/abs/2007.13985)
* SRSGD (https://arxiv.org/abs/2002.10583)
* SWATS (https://arxiv.org/abs/1712.07628)
* SWNTS (https://arxiv.org/abs/1905.01422v4)
* Sadam (https://arxiv.org/abs/1908.00700)
* Shampoo (https://arxiv.org/abs/1802.09568)
* SignAdam++ (https://arxiv.org/abs/1907.09008)
* SignSGD (https://arxiv.org/abs/1802.04434)
* SoftAdam (https://openreview.net/forum?id=Skgfr1rYDH)
* TAdam (https://arxiv.org/abs/2003.00179)
* VAdam (https://arxiv.org/abs/1806.04854)
* VR-SGD (https://arxiv.org/abs/1802.09932)
* WNGrad (https://arxiv.org/abs/1803.02865)
* YellowFin (https://arxiv.org/abs/1706.03471)
* Yogi (http://papers.nips.cc/paper/8186-adaptive-methods-for-nonconvex-optimization.pdf)
* vSGD-b (https://arxiv.org/abs/1206.1106)
* vSGD-fd (https://arxiv.org/abs/1301.3764)
* vSGD-g (https://arxiv.org/abs/1206.1106)
* vSGD-l (https://arxiv.org/abs/1206.1106)    


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
