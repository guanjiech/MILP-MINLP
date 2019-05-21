# MILP-MINLP

I am working on a highly complicated MINLP problem recently in a paper about mobile blockchain, which is my first paper here in ZJU. So I want to record some of my beneficial thoughts here. Besides, I will put all relevant materials used or which I think are precious in this repository.

For now, there mainly remains two kinds of algorithms to solve MINLP. One is ***deterministic optimization algorithm*** while another kind is ***evolution algorithm*** which is problem independent, such as GA, SA, PSO and so on. 

What's [mathmatic optimization](https://zhuanlan.zhihu.com/p/25579864)? This link is a detailed discussion on operational research(运筹学).

There is a [comparison](http://baijiahao.baidu.com/s?id=1600164518587031730&wfr=spider&for=pc) on performances between these two kinds of algorithms. 

The deterministic optimization algorithm to solve the problem of MINLP mainly includes **single-tree class** and **multi-tree class**. Singlg-tree class has a **Nonlinear Branch and Bound** method and **Nonlinear Branch and cut** method. Multi-tree class is mainly based on **outer approximation method** and **benders decomposition method**.

#### branch and bound algorithms: 
1. [principles and examples](https://imada.sdu.dk/~jbj/DM85/TSPtext.pdf)
2. [a latest work](http://web.tecnico.ulisboa.pt/mcasquilho/compute/_linpro/TaylorB_module_c.pdf)
3. [a easy-understanding slide from MIT](https://ocw.mit.edu/courses/sloan-school-of-management/15-053-optimization-methods-in-management-science-spring-2013/tutorials/MIT15_053S13_tut10.pdf)

---
1. There already remains some mature algorithms for solving **NLP(Non-linear programming)** and **ILP(Integer linear programming)** problems. If you want to catch up on the basics, you can go to [convex optimization](http://web.stanford.edu/class/ee364a/) from [Stephen P. Boyd](https://web.stanford.edu/~boyd/). There are superdetailed slides and videos here, which is quite beneficial.
2. other materials are directly included in this reository 
