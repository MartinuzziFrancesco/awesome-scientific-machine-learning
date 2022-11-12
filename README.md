# Awesome Scientific Machine Learning
A curated list of awesome Scientific Machine Learning (SciML) papers, resources and software

## Contents
- [Papers](#papers)
  - [Neural Differential Equations](#papers-neural-des)
  - [Physics Informed NNs](#papers-physics-informed-nns)
  - [Neural Operators](#papers-neural-operators)
  - [Model Discovery](#papers-model-discovery)
- [Software](#software)
  - [Julia](#software-julia)
  - [Python](#software-python)
    - [Pytorch based](#software-python-pytorch)
    - [Jax based](#software-python-jax)
    - [Tensorflow based](#software-python-tensorflow)
    - [Other](#software-python-other)
- [Books](#books)
- [Videos](#videos)
  - [Channels](#videos-channels)
  - [Playlists](#videos-playlists)
- [Conferences and Workshops](#conferences)
  - [Future](#conferences-future)
  - [Past](#conferences-past)
- [Contributions Guidelines](#contributions)
  - [Papers](#contributions-papers)
  - [Software](#contributions-software)
  - [Videos](#contributions-videos)
  - [Conferences and Workshops](#contributions-conferences)

<a name="papers"></a>
## Papers

<a name="papers-neural-des"></a>
### Neural Differential Equations
- Neural Ordinary Differential Equations [`pub`](https://papers.nips.cc/paper/2018/hash/69386f6bb1dfed68692a24c8686939b9-Abstract.html) [`arxiv`](https://arxiv.org/abs/1806.07366) <br> Chen, Ricky TQ, Yulia Rubanova, Jesse Bettencourt, and David K. Duvenaud <br> _Advances in neural information processing systems 31 (2018)_
- Universal Differential Equations for Scientific Machine Learning [[arxiv](https://arxiv.org/abs/2001.04385)] [[code](https://github.com/ChrisRackauckas/universal_differential_equations)]<br> Rackauckas, Christopher, Yingbo Ma, Julius Martensen, Collin Warner, Kirill Zubov, Rohit Supekar, Dominic Skinner, Ali Ramadhan, and Alan Edelman <br> _arXiv preprint arXiv:2001.04385 (2020)_
- Stiff neural ordinary differential equations [[pub](https://aip.scitation.org/doi/full/10.1063/5.0060697)] [[arxiv](https://arxiv.org/abs/2103.15341)] [[code](https://github.com/DENG-MIT/StiffNeuralODE)] <br> Kim, Suyong, Weiqi Ji, Sili Deng, Yingbo Ma, and Christopher Rackauckas <br> _Chaos: An Interdisciplinary Journal of Nonlinear Science 31, no. 9 (2021): 093122_
- Hamiltonian neural networks [[pub](https://papers.nips.cc/paper/2019/hash/26cd8ecadce0d4efd6cc8a8725cbd1f8-Abstract.html)] [[arxiv](https://arxiv.org/abs/1906.01563)] [[code](https://github.com/greydanus/hamiltonian-nn)] <br> Greydanus, Samuel, Misko Dzamba, and Jason Yosinski <br> _Advances in neural information processing systems 32 (2019)._
- Augmented neural odes [[pub](https://papers.nips.cc/paper/2019/hash/21be9a4bd4f81549a9d1d241981cec3c-Abstract.html)] [[arxiv](https://arxiv.org/abs/1904.01681)] [[code](https://github.com/EmilienDupont/augmented-neural-odes)] <br> Dupont, Emilien, Arnaud Doucet, and Yee Whye Teh <br> _Advances in Neural Information Processing Systems 32 (2019)._
- Fourier neural operator for parametric partial differential equations [[arxiv](https://arxiv.org/abs/2010.08895)] <br> Li, Zongyi, Nikola Kovachki, Kamyar Azizzadenesheli, Burigede Liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar <br> _arXiv preprint arXiv:2010.08895 (2020)._
- GRU-ODE-Bayes: Continuous modeling of sporadically-observed time series [[pub](https://proceedings.neurips.cc/paper/2019/hash/455cb2657aaa59e32fad80cb0b65b9dc-Abstract.html)] [[arxiv](https://arxiv.org/abs/1905.12374)] [[code](https://github.com/edebrouwer/gru_ode_bayes)] <br> De Brouwer, Edward, Jaak Simm, Adam Arany, and Yves Moreau. <br> _Advances in neural information processing systems 32 (2019)._
- Learning long-term dependencies in irregularly-sampled time series [[arxiv](https://arxiv.org/abs/2006.04418)] [[code](https://github.com/mlech26l/ode-lstms)] <br> Lechner, Mathias, and Ramin Hasani <br> _arXiv preprint arXiv:2006.04418 (2020)._
- Neural controlled differential equations for irregular time series [[pub](https://proceedings.neurips.cc/paper/2020/hash/4a5876b450b45371f6cfe5047ac8cd45-Abstract.html)] [[arxiv](https://arxiv.org/abs/2005.08926)] [[code](https://github.com/patrick-kidger/NeuralCDE)] <br> Kidger, Patrick, James Morrill, James Foster, and Terry Lyons <br> _Advances in Neural Information Processing Systems 33 (2020): 6696-6707._
- Neural stochastic differential equations: Deep latent gaussian models in the diffusion limit [[arxiv](https://arxiv.org/abs/1905.09883)] <br> Tzen, Belinda, and Maxim Raginsky <br> arXiv preprint arXiv:1905.09883 (2019).

<a name="papers-physics-informed-nns"></a>
### Physics Informed NNs
- Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations [[pub](https://www.sciencedirect.com/science/article/pii/S0021999118307125)] [[code](https://github.com/maziarraissi/PINNs)]<br> Raissi, Maziar, Paris Perdikaris, and George E. Karniadakis <br> _Journal of Computational physics 378 (2019): 686-707_
- Artificial neural networks for solving ordinary and partial differential equations. [[pub](https://ieeexplore.ieee.org/abstract/document/712178)] [[arxiv](https://arxiv.org/abs/physics/9705023)]<br> Lagaris, Isaac E., Aristidis Likas, and Dimitrios I. Fotiadis <br> _IEEE transactions on neural networks 9, no. 5 (1998): 987-1000._
- fPINNs: Fractional physics-informed neural networks [[pub](https://epubs.siam.org/doi/10.1137/18M1229845)] [[arxiv](https://arxiv.org/abs/1811.08967)]  <br> Pang, Guofei, Lu Lu, and George Em Karniadakis <br> _SIAM Journal on Scientific Computing 41, no. 4 (2019): A2603-A2626._
- Quantifying total uncertainty in physics-informed neural networks for solving forward and inverse stochastic problems [[pub](https://www.sciencedirect.com/science/article/pii/S0021999119305340?via%3Dihub)] [[arxiv](https://arxiv.org/abs/1809.08327v1)] <br> Zhang, Dongkun, Lu Lu, Ling Guo, and George Em Karniadakis <br> _Journal of Computational Physics 397 (2019): 108850._
- Physics-informed neural networks with hard constraints for inverse design [[pub](https://epubs.siam.org/doi/10.1137/21M1397908)] [[arxiv](https://arxiv.org/abs/2102.04626)] [[code](https://github.com/lululxvi/hpinn)] <br> Lu, Lu, Raphael Pestourie, Wenjie Yao, Zhicheng Wang, Francesc Verdugo, and Steven G. Johnson <br> _SIAM Journal on Scientific Computing 43, no. 6 (2021): B1105-B1132._
- On the eigenvector bias of fourier feature networks: From regression to solving multi-scale pdes with physics-informed neural networks [[pub](https://www.sciencedirect.com/science/article/abs/pii/S0045782521002759)] [[arxiv](https://arxiv.org/abs/2012.10047)] [[code](https://github.com/PredictiveIntelligenceLab/MultiscalePINNs)] <br> Wang, Sifan, Hanwen Wang, and Paris Perdikaris <br> _Computer Methods in Applied Mechanics and Engineering 384 (2021): 113938._

<a name="papers-neural-operators"></a>
### Neural Operators
- Deeponet: Learning nonlinear operators for identifying differential equations based on the universal approximation theorem of operators [[arxiv](https://arxiv.org/abs/1910.03193)] <br> Lu, Lu, Pengzhan Jin, and George Em Karniadakis <br> _arXiv preprint arXiv:1910.03193 (2019)._
- Learning nonlinear operators via DeepONet based on the universal approximation theorem of operators [[pub](https://www.nature.com/articles/s42256-021-00302-5)] [[code](https://github.com/lululxvi/deeponet)] <br> Lu, Lu, Pengzhan Jin, Guofei Pang, Zhongqiang Zhang, and George Em Karniadakis <br> _Nature Machine Intelligence 3, no. 3 (2021): 218-229._
- Learning the solution operator of parametric partial differential equations with physics-informed DeepONets [[pub](https://www.science.org/doi/full/10.1126/sciadv.abi8605)] [[code](https://github.com/PredictiveIntelligenceLab/Physics-informed-DeepONets)] <br> Wang, Sifan, Hanwen Wang, and Paris Perdikaris <br> _Science advances 7, no. 40 (2021): eabi8605._
- Fourier neural operator for parametric partial differential equations [[arxiv](https://arxiv.org/abs/2010.08895)] <br> Li, Zongyi, Nikola Kovachki, Kamyar Azizzadenesheli, Burigede Liu, Kaushik Bhattacharya, Andrew Stuart, and Anima Anandkumar <br> _arXiv preprint arXiv:2010.08895 (2020)._

<a name="papers-model-discovery"></a>
### Model Discovery
- Discovering governing equations from data by sparse identification of nonlinear dynamical systems [[pub](https://www.pnas.org/doi/full/10.1073/pnas.1517384113)] [[arxiv](https://arxiv.org/abs/1509.03580)] <br> Brunton, Steven L., Joshua L. Proctor, and J. Nathan Kutz. <br> _Proceedings of the national academy of sciences 113, no. 15 (2016): 3932-3937._


<a name="software"></a>
## Software

<a name="software-julia"></a>
### Julia
Julia has an entire organization called [Scientific Machine Learning (Sciml)](https://sciml.ai/) which provides software to do SciML with. The following list is a non-comprehensive list of the packages provided, for a full description please check out their website.
- DifferentialEquations.jl [[code](https://github.com/SciML/DifferentialEquations.jl)] [[docs](https://diffeq.sciml.ai/stable/)] <br> Differential equations solvers.
- DiffEqFlux.jl [[code](https://github.com/SciML/DiffEqFlux.jl)] [[docs](https://docs.sciml.ai/DiffEqFlux/stable/)] <br> Interface to build all variaties of neural differential equations.
- NeuralPDEs.jl [[code](https://github.com/SciML/NeuralPDE.jl)] [[docs](https://docs.sciml.ai/NeuralPDE/stable/)] <br> Interface to build Physics Informed Neural Networks.

<a name="software-python"></a>
### Python

<a name="software-python-pytorch"></a>
#### [Pythorch](https://pytorch.org/) based
- torchdiffeq [[code](https://github.com/rtqichen/torchdiffeq)] <br> Differential equations solvers.
- torchdyn [[code](https://github.com/DiffEqML/torchdyn)] [[docs](https://torchdyn.readthedocs.io/en/latest/)] <br> Library for neural differential equations and implicit models.

<a name="software-python-jax"></a>
#### [Jax](https://jax.readthedocs.io/en/latest/) based
- diffrax [[code](https://github.com/patrick-kidger/diffrax)] [[docs](https://docs.kidger.site/diffrax/)] <br> Differential equations solvers.

<a name="software-python-tensorflow"></a>
#### [Tensorflow](https://www.tensorflow.org/) based

<a name="software-python-other"></a>
#### Other
- pysindy [[code](https://github.com/dynamicslab/pysindy)] [[docs](https://pysindy.readthedocs.io/en/latest/)] <br> Sparse Identification of Nonlinear Dynamical systems (SINDy).
- DeepXDE [[code](https://github.com/lululxvi/deepxde)] [[docs](https://deepxde.readthedocs.io/en/latest/)] <br> Multi-platform (Pytorch, Jax, Tensorflow) library for scientific machine learning and physics-informed learning.

<a name="books"></a>
## Books

<a name="videos"></a>
## Videos

<a name="videos-channels"></a>
### Channels
- Physics Informed Machine Learning [[profile](https://www.youtube.com/c/PhysicsInformedMachineLearning)] <br> From the channel description: _This channel hosts videos from workshops at UW on Data-Driven Science and Engineering, and Physics Informed Machine Learning._
- Parallel Computing and Scientific Machine Learning [[profile](https://www.youtube.com/channel/UCDtsHjkOEMHYPGgpKX8VOPg)] <br> Lecture videos for MIT's 18.337J/6.338J: Parallel Computing and Scientific Machine Learning course of Fall 2020 and Spring 2021.
- Steve Brunton [[profile](https://www.youtube.com/c/Eigensteve)] <br> Lectures ranging from Linear Algebra basis to SciML theory and applications.

<a name="videos-playlists"></a>
### Playlists
- SciMLCon 2022 [[list](https://www.youtube.com/playlist?list=PLP8iPy9hna6QglWLQM02jcVjEBjaamzvw)]

<a name="conferences"></a>
### Conferences and Workshops

<a name="conferences-future"></a>
#### Future
- The Symbiosis of Deep Learning and Differential Equations - NeurIPS 2022 Workshop [[page](https://dlde-2022.github.io/)] <br> Online <br> 2022/12/14

<a name="conferences-past"></a>
#### Past
- SciMLCon 2022 [[page](https://scimlcon.org/2022/)] <br> Online <br> 2022/03/23
- The Symbiosis of Deep Learning and Differential Equations - NeurIPS 2021 Workshop [[page](https://dl-de.github.io/)] <br> Online <br> 2021/12/14
- Scientific Machine Learning - Workshop [[page](https://icerm.brown.edu/events/ht19-1-sml/)] <br> ICERM, Brown University <br> 2019/01/28 - 2019/01/30

<a name="contributions"></a>
## Contributions Guidelines
Contributions are very welcomed and encouraged! Please open a pull request with the indication of the type of contributions ([PAPER] for papers entries, [SOFTWARE] for software entries and so on), the entry itself and a few lines on why the contribution belongs to Awesome Scientific Machine Learning. Below are listed a few guidelines for each entry type. Please make sure to follow them to ensure a quick merge and an easier experience altogheter. Be aware that the guidelines themselves are subject to change, if you have ideas on how to improve the repo through them make sure to open a pr and tag it [GUIDELINES].

All of the guidelines given here are based on elements and resources already indexed, so if there is any confusion about them please make sure to check the raw version of the README.md before opening a pr.
<a name="contributions-papers"></a>
### Papers
Papers should have title, author list and pubblication venue separeted by break elements. The author's name are to be fully spelled out (following the Chicago entry on Google scholar) and the pubblication venue is to be written in _italic_.  Please provide the link of the source of the pubblication in [pub], and the [arxiv](https://arxiv.org/) abstract as [arxiv] when applicable. Additionally the code used for the paper can be linked in [code] (this only applies when the code is linked in the paper itself or written by the author(s). For third party implementations look at [Papers with Code](https://paperswithcode.com/)).

<a name="contributions-software"></a>
### Software
Software should have the full name of the library and they have to be indexed under the appropriate language (Julia, Pytho, R...). If the language index for the software you want to add to the list is not present please make sure to add it. Please provide the source of the code in [code] (it can be a GitHub link, GitLab link or you favourite version control host) and the link to the documentation in [docs]. In the next line please provide a couple of sentences with reference to what the software is doing. Please refrain from linking general deep learning libraries, in most cases they should be indexed already under their language.

<a name="contributions-videos"></a>
### Videos
Videos should have the title, speaker and host separated by break elements. After the title please provide the link to the video in [video] and the slides in [slides] if applicable. Entire channels dedicated to SciML can be linked providing the source in [profile]. Playlists of SciML videos should be linked as [list]. Please try to minimize the intersection of playlists and channels.


<a name="contributions-conferences"></a>
### Conferences and Workshops
Events should be indexed in chronological order, with the latest on top. Link to the main page should be done in [page]. Please be mindful of the distinction between past events and future events. Nome of the event, location and date(s) should be separeted by break elements. Dates follow the format YYYY/MM/DD. If the event spanned more days please indicate starting day and ending day separated with the following symbol: -. Example: YYYY/MM/DD-YYYY/MM/DD.

An event can be added in the future section without date or location as long as there is a web page with the description of the event. The missing date or location line should be filled in as TBD. When the date is known please make sure to update the entry.
