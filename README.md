# MILP-MINLP
I am working on a highly complicated MINLP problem recently in a paper about mobile blockchain, which is my first paper here in ZJU. So I want to record some of my beneficial thoughts here. Besides, I will put all relevant materials used or which I think are precious in this repository.

For now, there mainly remains two kinds of algorithms to solve MINLP. One is *deterministic optimization algorithm* while another kind is *evolution algorithm* which is problem independent. 
The deterministic optimization algorithm to solve the problem of MINLP mainly includes **single-tree class** and **multi-tree class**. Singlg-tree class has a **Nonlinear Branch and Bound**method and **Nonlinear Branch and cut**method. Multi-tree class is mainly based on **outer approximation method** and **benders decomposition method**.

---
NLP（Non-linear programming）和ILP（Integer linear programming)问题都有成熟的求解算法。如果想补一补基础可以学习Stephen P. Boyd的[convex optimization](http://web.stanford.edu/class/ee364a/)，有详细的slides，电子书，以及视频教程。
