# Descending through a Crowded Valley - Benchmarking Deep Learning Optimizers

[Robin M. Schmidt](https://scholar.google.de/citations?user=20vb63kAAAAJ&hl=de), [Frank Schneider](https://scholar.google.com/citations?user=znq-WkAAAAAJ&hl=en), and [Philipp Hennig](https://scholar.google.de/citations?user=UeG5w08AAAAJ&hl=en)

**Paper**: [[ICML 2021]](http://proceedings.mlr.press/v139/schmidt21a)

> **Abstract:** *Choosing the optimizer is considered to be among the most crucial design decisions in deep learning, and it is not an easy one. The growing literature now lists hundreds of optimization methods. In the absence of clear theoretical guidance and conclusive empirical evidence, the decision is often made based on anecdotes. In this work, we aim to replace these anecdotes, if not with a conclusive ranking, then at least with evidence-backed heuristics. To do so, we perform an extensive, standardized benchmark of fifteen particularly popular deep learning optimizers while giving a concise overview of the wide range of possible choices. Analyzing more than 50,000 individual runs, we contribute the following three points: (i) Optimizer performance varies greatly across tasks. (ii) We observe that evaluating multiple optimizers with default parameters works approximately as well as tuning the hyperparameters of a single, fixed optimizer. (iii) While we cannot discern an optimization method clearly dominating across all tested tasks, we identify a significantly reduced subset of specific optimizers and parameter choices that generally lead to competitive results in our experiments: Adam remains a strong contender, with newer methods failing to significantly and consistently outperform it. Our open-sourced results are available as challenging and well-tuned baselines for more meaningful evaluations of novel optimization methods without requiring any further computational efforts.*

## Results

This repository provides the full log files of all our benchmarking results.
They are organized into:

- **Main results:** Comparison of fifteen popular deep learning optimizers on eight problems, using four different tuning budgets and four different learning rate schedules. The main results amount to more than 50,000 individual runs.
- **Tuning validation:** In order to test the stability of our benchmark, we re-tuned two optimizers (RMSProp and AdaDelta) on all problems a second time. The results of this evaluation are shown in Appendix D in our paper.
- **Seed robustness:** An optimizer's performance can be sensitive to the random seed. In this analysis, we performed an extensive grid search on the learning rate for SGD, using ten different seeds throughout. This identifies a “danger zone” of learning rates, that can be sensitive to the random seed. The full analysis can be found in Appendix C of our paper.

Everyone is invited to use those results, for example, to evaluate the performance of newly developed optimizers or as training data for meta-learned optimizers.

We are happy to extend our results with additional optimizers, provided they are generated using the same process described in the paper, to assure a fair comparison.

Below we highlight two figures summarizing our evaluation of those results. For the full evaluation with all our plots and explanations, please check out [our paper](http://arxiv.org/abs/2007.01547).

![Parallel Coordinates Plot](https://i.imgur.com/NJbDFkH.png)

![Heatmap](https://i.imgur.com/XsRude4.png)

## List of Optimizers

Our paper lists over hundred optimizers that have been proposed for deep learning applications. Here, we keep a digital version that gets updated regularly. If you want to add a method or find an out-of-date reference, please feel free to open a pull request.

- **AcceleGrad** *(Levy et al., 2018)* [[NeurIPS]](https://proceedings.neurips.cc/paper/2018/hash/b0169350cd35566c47ba83c6ec1d6f82-Abstract.html)
- **ACClip** *(Zhang et al., 2020)* [[NeurIPS]](https://papers.nips.cc/paper/2020/hash/b05b57f6add810d3b7490866d74c0053-Abstract.html)
- **AdaAlter** *(Xie et al., 2019)* [[arXiv]](https://arxiv.org/abs/1911.09030)
- **AdaBatch** *(Devarakonda et al., 2017)* [[arXiv]](https://arxiv.org/abs/1712.02029)
- **AdaBayes/AdaBayes-SS** *(Aitchison, 2020)* [[NeurIPS]](https://papers.nips.cc/paper/2020/hash/d33174c464c877fb03e77efdab4ae804-Abstract.html)
- **AdaBelief** *(Zhuang et al., 2020)* [[NeurIPS]](https://proceedings.neurips.cc/paper/2020/hash/d9d4f495e875a2e075a1a4a6e1b9770f-Abstract.html)
- **AdaBlock** *(Yun et al., 2019)* [[arXiv]](http://arxiv.org/abs/1905.10757)
- **AdaBound/AMSBound** *(Luo et al., 2019)* [[ICLR]](https://openreview.net/forum?id=Bkg3g2R9FX)
- **AdaComp** *(Chen et al., 2018)* [[AAAI]](https://aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/16859)
- **Adadelta** *(Zeiler, 2012)* [[arXiv]](https://arxiv.org/abs/1212.5701)
- **Adafactor** *(Shazeer & Stern, 2018)* [[ICML]](http://proceedings.mlr.press/v80/shazeer18a.html)
- **AdaFix** *(Bae et al., 2019)* [[arXiv]](http://arxiv.org/abs/1911.00289)
- **AdaFom** *(Chen et al., 2019)* [[ICLR]](https://openreview.net/forum?id=H1x-x309tm)
- **AdaFTRL** *(Orabona & Pál, 2015)* [[ALT]](https://arxiv.org/abs/1502.05744)
- **Adagrad** *(Duchi et al., 2011)* [[JMLR]](https://jmlr.org/papers/v12/duchi11a.html)
- **ADAHESSIAN** *(Yao et al., 2020)* [[arXiv]](https://arxiv.org/abs/2006.00719)
- **Adai** *(Xie et al., 2020)* [[arXiv]](http://arxiv.org/abs/2006.15815)
- **AdaLoss** *(Teixeira et al., 2019)* [[arXiv]](http://arxiv.org/abs/1908.01070)
- **Adam** *(Kingma & Ba, 2015)* [[ICLR]](https://arxiv.org/abs/1412.6980)
- **Adam+** *(Liu et al., 2020)* [[arXiv]](http://arxiv.org/abs/2011.11985)
- **AdamAL** *(Tao et al., 2019)* [[OpenReview]](https://openreview.net/forum?id=SyxM51BYPB)
- **AdaMax** *(Kingma & Ba, 2015)* [[ICLR]](https://arxiv.org/abs/1412.6980)
- **AdamBS** *(Liu et al., 2020)* [[arXiv]](http://arxiv.org/abs/2010.12986)
- **AdamNC** *(Reddi et al., 2018)* [[ICLR]](https://openreview.net/forum?id=ryQu7f-RZ)
- **AdaMod** *(Ding et al., 2019)* [[arXiv]](http://arxiv.org/abs/1910.12249)
- **AdamP** *(Heo et al., 2020)* [[arXiv]](http://arxiv.org/abs/2006.08217)
- **AdamT** *(Zhou et al., 2020)* [[arXiv]](http://arxiv.org/abs/2001.06130)
- **AdamW** *(Loshchilov & Hutter, 2019)* [[ICLR]](https://openreview.net/forum?id=Bkg6RiCqY7)
- **AdamX** *(Tran & Phong et al., 2019)* [[IEEE Access]](https://ieeexplore.ieee.org/document/8713445?source=authoralert)
- **ADAS** *(Eliyahu, 2020)* [[Github]](https://github.com/YanaiEliyahu/AdasOptimizer)
- **AdaS** *(Hosseini & Plataniotis, 2020)* [[arXiv]](http://arxiv.org/abs/2006.06587)
- **AdaScale** *(Johnson et al., 2020)* [[ICML]](http://proceedings.mlr.press/v119/johnson20a.html)
- **AdaSGD** *(Wang & Wiens, 2020)* [[arXiv]](http://arxiv.org/abs/2006.16541)
- **AdaShift** *(Zhou et al., 2019)* [[ICLR]](https://openreview.net/forum?id=HkgTkhRcKQ)
- **AdaSqrt** *(Hu et al., 2019)* [[arXiv]](http://arxiv.org/abs/1912.09926)
- **Adathm** *(Sun et al., 2019)* [[IEEE DSC]](https://ieeexplore.ieee.org/document/8923615)
- **AdaX/AdaX-W** *(Li et al., 2020)* [[arXiv]](http://arxiv.org/abs/2004.09740)
- **AEGD** *(Liu & Tian, 2020)* [[arXiv]](http://arxiv.org/abs/2010.05109)
- **ALI-G** *(Berrada et al., 2020)* [[ICML]](http://proceedings.mlr.press/v119/berrada20a.html)
- **AMSGrad** *(Reddi et al., 2018)* [[ICLR]](https://openreview.net/forum?id=ryQu7f-RZ)
- **AngularGrad** *(Roy et al., 2021)* [[arXiv]](http://arxiv.org/abs/2105.10190)
- **ArmijoLS** *(Vaswani et al., 2019)* [[NeurIPS]](https://proceedings.neurips.cc/paper/2019/hash/2557911c1bf75c2b643afb4ecbfc8ec2-Abstract.html)
- **ARSG** *(Chen et al., 2019)* [[arXiv]](http://arxiv.org/abs/1905.01422)
- **ASAM** *(Kwon et al., 2021)* [[arXiv]](https://arxiv.org/abs/2102.11600)
- **AutoLRS** *(Jin et al., 2021)* [[ICLR]](https://openreview.net/forum?id=SlrqM9_lyju)
- **AvaGrad** *(Savarese et al., 2019)* [[arXiv]](http://arxiv.org/abs/1912.01823)
- **BAdam** *(Salas et al., 2018)* [[arXiv]](http://arxiv.org/abs/1811.03679)
- **BGAdam** *(Bai & Zhang, 2019)* [[arXiv]](http://arxiv.org/abs/1908.08015)
- **BPGrad** *(Zhang et al., 2017)* [[arXiv]](https://arxiv.org/abs/1711.06959)
- **BRMSProp** *(Aitchison, 2020)* [[NeurIPS]](https://papers.nips.cc/paper/2020/hash/d33174c464c877fb03e77efdab4ae804-Abstract.html)
- **BSGD** *(Hu et al., 2020)* [[NeurIPS]](https://papers.nips.cc/paper/2020/hash/1cdf14d1e3699d61d237cf76ce1c2dca-Abstract.html)
- **C-ADAM** *(Tutunov et al., 2020)* [[arXiv]](http://arxiv.org/abs/2002.03755)
- **CADA** *(Chen et al., 2020)* [[arXiv]](http://arxiv.org/abs/2012.15469)
- **COCOB** *(Orabona & Tommasi, 2017)* [[NeurIPS]](https://proceedings.neurips.cc/paper/2017/hash/7c82fab8c8f89124e2ce92984e04fb40-Abstract.html)
- **Cool Momentum** *(Borysenko & Byshkin, 2020)* [[arXiv]](http://arxiv.org/abs/2005.14605)
- **CProp** *(Preechakul & Kijsirikul et al., 2019)* [[arXiv]](http://arxiv.org/abs/1912.11493)
- **Curveball** *(Henriques et al., 2019)* [[ICCV]](https://openaccess.thecvf.com/content_ICCV_2019/html/Henriques_Small_Steps_and_Giant_Leaps_Minimal_Newton_Solvers_for_Deep_ICCV_2019_paper.html)
- **Dadam** *(Nazari et al., 2019)* [[arXiv]](http://arxiv.org/abs/1901.09109)
- **DeepMemory** *(Wright, 2020)* [[Github]](https://github.com/lessw2020/Best-Deep-Learning-Optimizers/tree/master/DeepMemory)
- **DGNOpt** *(Liu et al., 2021)* [[ICML]](https://arxiv.org/abs/2105.03788)
- **DiffGrad** *(Dubey et al., 2020)* [[IEEE Transactions on Neural Networks and Learning Systems]](https://ieeexplore.ieee.org/document/8939562)
- **EAdam** *(Yuan & Gao, 2020)* [[arXiv]](http://arxiv.org/abs/2011.02150)
- **EKFAC** *(George et al., 2018)* [[NeurIPS]](https://proceedings.neurips.cc/paper/2018/hash/48000647b315f6f00f913caa757a70b3-Abstract.html)
- **Eve** *(Hayashi, 2016)* [[arXiv]](https://arxiv.org/abs/1611.01505)
- **Expectigrad** *(Daley & Amato, 2020)* [[arXiv]](http://arxiv.org/abs/2010.01356)
- **FastAdaBelief** *(Zhou et al., 2021)* [[arXiv]](http://arxiv.org/abs/2104.13790)
- **FRSGD** *(Wang & Ye, 2020)* [[arXiv]](http://arxiv.org/abs/2012.02188)
- **G-AdaGrad** *(Chakrabarti & Chopra, 2021)* [[arXiv]](http://arxiv.org/abs/2106.00092)
- **GADAM** *(Zhang & Gouza et al., 2018)* [[arXiv]](http://arxiv.org/abs/1805.07500)
- **Gadam** *(Granziol et al., 2020)* [[arXiv]](http://arxiv.org/abs/2003.01247)
- **GOALS** *(Chae et al., 2021)* [[arXiv]](http://arxiv.org/abs/2105.10915)
- **GOLS-I** *(Kafka & Wilke, 2019)* [[arXiv]](http://arxiv.org/abs/1903.09383)
- **Grad-Avg** *(Purkayastha & Purkayastha, 2020)* [[arXiv]](http://arxiv.org/abs/2012.02387)
- **GRAPES** *(Dellaferrera et al., 2021)* [[arXiv]](http://arxiv.org/abs/2104.11604)
- **Gravilon** *(Kelterobrn et al., 2020)* [[arXiv]](http://arxiv.org/abs/2008.11370)
- **Gravity** *(Bahrami & Zadeh, 2021)* [[arXiv]](http://arxiv.org/abs/2101.09192)
- **HAdam** *(Jiang et al., 2019)* [[arXiv]](http://arxiv.org/abs/1910.06878)
- **HyperAdam** *(Wang et al., 2019)* [[AAAI]](https://ojs.aaai.org//index.php/AAAI/article/view/4466)
- **K-BFGS/K-BFGS(L)** *(Goldfarb et al., 2020)* [[NeurIPS]](https://proceedings.neurips.cc/paper/2020/hash/192fc044e74dffea144f9ac5dc9f3395-Abstract.html)
- **K-FAC** *(Martens & Grosse, 2015)* [[ICML]](http://proceedings.mlr.press/v37/martens15.html)
- **KF-QN-CNN** *(Ren & Goldfarb, 2021)* [[arXiv]](https://arxiv.org/abs/2102.06737)
- **KFLR/KFRA** *(Botev et al., 2017)* [[ICML]](http://proceedings.mlr.press/v70/botev17a.html)
- **L4Adam/L4Momentum** *(Rolínek & Martius, 2018)* [[NeurIPS]](https://proceedings.neurips.cc/paper/2018/hash/98b17f068d5d9b7668e19fb8ae470841-Abstract.html)
- **LAMB** *(You et al., 2020)* [[ICLR]](https://openreview.net/forum?id=Syx4wnEtvH)
- **LaProp** *(Ziyin et al., 2020)* [[arXiv]](http://arxiv.org/abs/2002.04839)
- **LARS** *(You et al., 2017)* [[ICLR]](https://openreview.net/forum?id=Syx4wnEtvH)
- **LHOPT** *(Almeida et al., 2021)* [[arXiv]](https://arxiv.org/abs/2106.00958)
- **LookAhead** *(Zhang et al., 2019)* [[NeurIPS]](https://papers.nips.cc/paper/2019/hash/90fd4f88f588ae64038134f1eeaa023f-Abstract.html)
- **M-SVAG** *(Balles & Hennig, 2018)* [[ICML]](http://proceedings.mlr.press/v80/balles18a.html)
- **MADGRAD** *(Defazio & Jelassi, 2021)* [[arXiv]](https://arxiv.org/abs/2101.11075)
- **MAS** *(Landro et al., 2020)* [[arXiv]](http://arxiv.org/abs/2011.08042)
- **MEKA** *(Chen et al., 2020)* [[arXiv]](http://arxiv.org/abs/2011.04803)
- **MTAdam** *(Malkiel & Wolf, 2020)* [[arXiv]](http://arxiv.org/abs/2006.14683)
- **MVRC-1/MVRC-2** *(Chen & Zhou, 2020)* [[arXiv]](http://arxiv.org/abs/2005.07755)
- **Nadam** *(Dozat, 2016)* [[ICLR]](https://openreview.net/forum?id=OM0jvwB8jIp57ZJjtNEZ)
- **NAMSB/NAMSG** *(Chen et al., 2019)* [[arXiv]](http://arxiv.org/abs/1905.01422)
- **ND-Adam** *(Zhang et al., 2017)* [[arXiv]](http://arxiv.org/abs/1709.04546)
- **Nero** *(Liu et al., 2021)* [[arXiv]](https://arxiv.org/abs/2102.07227)
- **Nesterov Accelerated Momentum** *(Nesterov, 1983)* [[Soviet Mathematics Doklady]](http://mpawankumar.info/teaching/cdt-big-data/nesterov83.pdf)
- **Noisy Adam/Noisy K-FAC** *(Zhang et al., 2018)* [[ICML]](http://proceedings.mlr.press/v80/zhang18l.html)
- **NosAdam** *(Huang et al., 2019)* [[IJCAI]](https://www.ijcai.org/Proceedings/2019/355)
- **Novograd** *(Ginsburg et al., 2019)* [[arXiv]](http://arxiv.org/abs/1905.11286)
- **NT-SGD** *(Zhou et al., 2021)* [[arXiv]](http://arxiv.org/abs/2103.00075)
- **Padam** *(Chen et al., 2020)* [[IJCAI]](https://www.ijcai.org/Proceedings/2020/452)
- **PAGE** *(Li et al., 2020)* [[arXiv]](http://arxiv.org/abs/2008.10898)
- **PAL** *(Mutschler & Zell, 2020)* [[NeurIPS]](https://papers.nips.cc/paper/2020/hash/3a30be93eb45566a90f4e95ee72a089a-Abstract.html)
- **PolyAdam** *(Orvieto et al., 2019)* [[UAI]](http://proceedings.mlr.press/v115/orvieto20a.html)
- **Polyak Momentum** *(Polyak, 1964)* [[USSR Computational Mathematics and Mathematical Physics]](https://www.sciencedirect.com/science/article/abs/pii/0041555364901375)
- **PowerSGD/PowerSGDM** *(Vogels et al., 2019)* [[NeurIPS]](https://proceedings.neurips.cc/paper/2019/hash/d9fbed9da256e344c1fa46bb46c34c5f-Abstract.html)
- **Probabilistic Polyak** *(de Roos et al., 2021)* [[arXiv]](https://arxiv.org/abs/2102.10880)
- **ProbLS** *(Mahsereci & Hennig, 2017)* [[JMLR]](https://jmlr.org/papers/v18/17-049.html)
- **PSTorm** *(Xu, 2020)* [[arXiv]](http://arxiv.org/abs/2006.00425)
- **QHAdam/QHM** *(Ma & Yarats, 2019)* [[ICLR]](https://openreview.net/forum?id=S1fUpoR5FQ)
- **RAdam** *(Liu et al., 2020)* [[ICLR]](https://openreview.net/forum?id=rkgz2aEKDr)
- **Ranger** *(Wright, 2020)* [[Github]](https://github.com/lessw2020/Ranger-Deep-Learning-Optimizer)
- **RangerLars** *(Grankin et al., 2020)* [[Github]](https://github.com/mgrankin/over9000)
- **RecursiveOptimizer** *(Cutkosky & Sarlos, 2019)* [[ICML]](http://proceedings.mlr.press/v97/cutkosky19b.html)
- **RescaledExp** *(Cutkosky & Boahen, 2019)* [[NeurIPS]](https://proceedings.neurips.cc/paper/2016/hash/550a141f12de6341fba65b0ad0433500-Abstract.html)
- **RMSProp** *(Tieleman & Hinton, 2012)* [[Coursera]](http://www.cs.toronto.edu/~hinton/coursera/lecture6/lec6.pdf)
- **RMSterov** *(Choi et al., 2019)* [[arXiv]](http://arxiv.org/abs/1910.05446)
- **S-SGD** *(Sung et al., 2020)* [[arXiv]](http://arxiv.org/abs/2009.02479)
- **SAdam** *(Wang et al., 2020)* [[ICLR]](https://openreview.net/forum?id=rye5YaEtPr)
- **Sadam/SAMSGrad** *(Tong et al., 2019)* [[arXiv]](http://arxiv.org/abs/1908.00700)
- **SALR** *(Yue et al., 2020)* [[arXiv]](http://arxiv.org/abs/2011.05348)
- **SAM** *(Foret et al., 2021)* [[ICLR]](https://openreview.net/forum?id=6Tm1mposlrM)
- **SC-Adagrad/SC-RMSProp** *(Mukkamala & Hein, 2017)* [[ICML]](http://proceedings.mlr.press/v70/mukkamala17a.html)
- **SDProp** *(Ida et al., 2017)* [[IJCAI]](https://www.ijcai.org/Proceedings/2017/267)
- **SGD** *(Robbins & Monro, 1951)* [[Annals of Mathematical Statistics]](https://projecteuclid.org/euclid.aoms/1177729586)
- **SGD-BB** *(Tan et al., 2016)* [[NeurIPS]](https://papers.nips.cc/paper/2016/hash/c86a7ee3d8ef0b551ed58e354a836f2b-Abstract.html)
- **SGD-G2** *(Ayadi & Turinici, 2020)* [[arXiv]](http://arxiv.org/abs/2002.09304)
- **SGDEM** *(Ramezani-Kebrya et al., 2021)* [[arXiv]](https://arxiv.org/abs/2102.13653)
- **SGDHess** *(Tran & Cutkosky, 2021)* [[arXiv]](https://arxiv.org/abs/2103.03265)
- **SGDM** *(Liu & Luo, 2020)* [[arXiv]](http://arxiv.org/abs/2006.00423)
- **SGDP** *(Heo et al., 2020)* [[arXiv]](http://arxiv.org/abs/2006.08217)
- **SGDR** *(Loshchilov & Hutter, 2017)* [[ICLR]](https://openreview.net/forum?id=Skq89Scxx)
- **SHAdagrad** *(Huang et al., 2020)* [[arXiv]](http://arxiv.org/abs/2006.07037)
- **Shampoo** *(Gupta et al., 2018)* [[ICML]](http://proceedings.mlr.press/v80/gupta18a.html)
- **SignAdam++** *(Wang et al., 2019)* [[ICDMW]](https://ieeexplore.ieee.org/document/8955622)
- **SignSGD** *(Bernstein et al., 2018)* [[ICML]](http://proceedings.mlr.press/v80/bernstein18a.html)
- **SKQN/S4QN** *(Yang et al., 2020)* [[arXiv]](http://arxiv.org/abs/2006.09606)
- **SM3** *(Anil et al., 2019)* [[NeurIPS]](https://proceedings.neurips.cc/paper/2019/hash/8f1fa0193ca2b5d2fa0695827d8270e9-Abstract.html)
- **SMG** *(Tran et al., 2020)* [[arXiv]](http://arxiv.org/abs/2011.11884)
- **SNGM** *(Zhao et al., 2020* [[arXiv]](http://arxiv.org/abs/2007.13985)
- **SoftAdam** *(Fetterman et al., 2019)* [[OpenReview]](https://openreview.net/forum?id=Skgfr1rYDH)
- **SRSGD** *(Wang et al., 2020)* [[arXiv]](http://arxiv.org/abs/2002)
- **Step-Tuned SGD** *(Castera et al., 2021)* [[arXiv]](https://arxiv.org/abs/2103.03570)
- **STORM** *(Cutkosky & Orabona, 2019)* [[NeurIPS]](https://papers.nips.cc/paper/2019/hash/b8002139cdde66b87638f7f91d169d96-Abstract.html)
- **SWATS** *(Keskar & Socher, 2017)* [[arXiv]](http://arxiv.org/abs/1712.07628)
- **SWNTS** *(Chen et al., 2019)* [[arXiv]](http://arxiv.org/abs/1905.01422)
- **TAdam** *(Ilboudo et al., 2020)* [[arXiv]](http://arxiv.org/abs/2003.00179)
- **TEKFAC** *(Gao et al., 2020)* [[arXiv]](http://arxiv.org/abs/2011.13609)
- **VAdam** *(Khan et al., 2018)* [[ICML]](http://proceedings.mlr.press/v80/khan18a.html)
- **VR-SGD** *(Shang et al., 2020)* [[IEEE Trans. Knowl. Data Eng.]](https://ieeexplore.ieee.org/document/8515112)
- **vSGD-b/vSGD-g/vSGD-l** *(Schaul et al., 2013)* [[ICML]](http://proceedings.mlr.press/v28/schaul13.html)
- **vSGD-fd** *(Schaul & LeCun, 2013)* [[ICLR]](https://openreview.net/forum?id=7IOAIAx1AiEYC)
- **WNGrad** *(Wu et al., 2018)* [[arXiv]](http://arxiv.org/abs/1803.02865)
- **YellowFin** *(Zhang & Mitliagkas, 2019)* [[MLSys]](https://proceedings.mlsys.org/paper/2019/hash/b3e3e393c77e35a4a3f3cbd1e429b5dc-Abstract.html)
- **Yogi** *(Zaheer et al., 2018)* [[NeurIPS]](https://papers.nips.cc/paper/2018/hash/90365351ccc7437a1309dc64e4db32a3-Abstract.html)

## Citation

If you use our results, please consider citing:

> [Robin M. Schmidt, Frank Schneider, Philipp Hennig<br/>
> **Descending through a Crowded Valley - Benchmarking Deep Learning Optimizers**<br/>
> *ICML 2021*](http://proceedings.mlr.press/v139/schmidt21a)

```bibtex
@InProceedings{pmlr-v139-schmidt21a,
  title = 	 {Descending through a Crowded Valley - Benchmarking Deep Learning Optimizers},
  author =       {Schmidt, Robin M and Schneider, Frank and Hennig, Philipp},
  booktitle = 	 {Proceedings of the 38th International Conference on Machine Learning},
  pages = 	 {9367--9376},
  year = 	 {2021},
  editor = 	 {Meila, Marina and Zhang, Tong},
  volume = 	 {139},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {18--24 Jul},
  publisher =    {PMLR},
  pdf = 	 {http://proceedings.mlr.press/v139/schmidt21a/schmidt21a.pdf},
  url = 	 {http://proceedings.mlr.press/v139/schmidt21a.html}
}
```

## Contact

Should you have any questions, please feel free to contact the authors.
