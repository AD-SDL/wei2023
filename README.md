# Towards a Modular Architecture for Science Factories
## Accelerate 2023 
<div align="center">

[[Website]]()
[[arXiv]]()
[[PDF]]()
______________________________________________________________________
</div>

Advances in robotic automation, high-performance computing (HPC), and artificial intelligence
(AI) encourage us to conceive of science factories: large, general-purpose computation- and AI-
enabled self-driving laboratories (SDLs) with the generality and scale required both to tackle
large discovery problems and to support the concurrent work of thousands of scientists. Like
modern conventional factories, science factories require modular hardware and software that can
easily be replicated for scale and (re)configured to support many concurrent applications. Here we
propose a prototype modular science factory architecture in which modules (each encapsulating
a scientific instrument or other apparatus with a simple, six-function software interface plus an
optional common hardware form factor) are coupled to form workcells (sets of modules linked
with a manipulator) on which are run workflows (series of actions on modules in a workcell) by
applications (one or more workflow runs plus computational and data manipulation steps). We
describe applications of these methods in experiments involving 15 different robotic apparatus,
five applications (one in education, two in biology, two in materials), and a variety of workflows,
across four labs. We report on successes reusing modules, workcells, and workflows in different
applications and with migrating applications between workcells, and suggest directions for future
work aimed at yet more generality and scalability. Code and data are available at [https:/github.com/AD-SDL/rpl_wei] (https://github.com/AD-SDL/rpl_wei) and in the Supplementary Information.


![multiworkcell](images/multiworkcell.png)
*Figure 1: An example of how our framework can connect multiple workcells*
\
\
![Entities](images/Entities2.png)
*Figure 2: A diagram of the layout of our software infrastructure and all of its components*
# Installation
## Installation
 1. Clone the repository into the desired location. This tutorial will assume it is installed in a folder called `~/workspace/rpl_wei`
 2. within `~/workspace/rpl_wei` run the following code block: 

```
conda create -n rpl-wei python=3.9
conda activate rpl-wei
pip3 install --upgrade pip setuptools wheel
pip3 install -r requirements/dev.txt
pip3 install -r requirements/requirements.txt
pip3 install -e .

```


# Demo
In a linux terminal, go to `~/workspace/rpl_wei/examples`. from within the folder run `./run_wei_server.sh`. in a new terminal tab in the same folder, run `./run_example.py`. This will show a text-only simulation of the workflow execution
# Paper and Citation

Our paper is posted on [arXiv](). If you find our work useful, please consider citing us! 

```bibtex
@inproceedings{}
```
