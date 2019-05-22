# MILP-MINLP

I am working on a highly complicated MINLP problem recently in a paper about mobile blockchain, which is my first paper here in ZJU. So I want to record some of my beneficial thoughts here. Besides, I will put all relevant materials used or which I think are precious in this repository.

Firstly, I think it's worth noting the difference between **MILP** and **ILP**. In MILP problems, there are not only continuous variables but also integer variables, while the decision variables are all integer in ILP problems. 

For now, there mainly remain two kinds of algorithms to solve MINLP problems. One is ***deterministic optimization algorithm*** while another kind is ***evolution algorithm*** which is problem-independent, such as GA, SA, PSO and so on. 

What's [mathmatic optimization](https://zhuanlan.zhihu.com/p/25579864)? This link is a detailed discussion on operational research(运筹学).

There is a [comparison](http://baijiahao.baidu.com/s?id=1600164518587031730&wfr=spider&for=pc) on performances between these two kinds of algorithms. 

The deterministic optimization algorithm to solve the problem of MINLP mainly includes **single-tree class** and **multi-tree class**. Single-tree class has a **Nonlinear Branch and Bound** method and **Nonlinear Branch and cut** method. Multi-tree class is mainly based on **outer approximation method** and **benders decomposition method**.

---
#### Branch and Bound algorithms: 
1. [a classic on B&B principles and examples](https://imada.sdu.dk/~jbj/DM85/TSPtext.pdf)
2. [a simple example](http://web.tecnico.ulisboa.pt/mcasquilho/compute/_linpro/TaylorB_module_c.pdf)  
- Notes: 
  * relax the integer constraint to a LP model and then get the optimal relaxed solution, the **Z** value for the relaxed solution is the upper bound while the **Z** value for the rounded-down solution is the lower bound. The optimal integer solution will be between these two bounds. 
  * observe the relaxed solution value for each variable and choose the variable with the greatest fractional part for branching
  * add new constraint to the initial model, calculate the optimal solution for this model with integer restrictions relaxed and then get the upper bound, the existing maximum integer solution(at any node) is the lower bound
  * Next, always branch from the node with the maximum upper bound
  * repeat the steps, the optimal integer solution is reached when a feasible integer solution is generated at a node and the upper bound of that node is greater than or equal to any other ending nodes(i.e., a node at the end of a branch)
  * **For a minimization model, relaxed solutions are rounded-up, and upper and lower bounds are reversed.**
3. [easy-understanding slides from MIT](https://ocw.mit.edu/courses/sloan-school-of-management/15-053-optimization-methods-in-management-science-spring-2013/tutorials/MIT15_053S13_tut10.pdf)
4. [youtube video: What's branch and bound method?](https://www.youtube.com/watch?v=WNRRmXZkRi0)
5. [youtube video: How to solve a ILP problem using branch and bound](https://www.youtube.com/watch?v=upcsrgqdeNQ)

---
While learning Integer Programming problems, we always encounter **LP Relaxation** somewhere. So what's LP Relaxation?

LP Relaxation is a model created by **dropping** integer(or binary) constraints of a ILP model. We relax a constraint means we ignore that constraint. 

Here is a four-minute video on this issue:[LP Relaxation](https://www.youtube.com/watch?v=P_-0YyQUgAs) 


---
1. There already remain some mature algorithms for solving **NLP(Non-linear programming)** and **ILP(Integer linear programming)** problems. If you want to catch up on the basics, you can go to [convex optimization](http://web.stanford.edu/class/ee364a/) from [Stephen P. Boyd](https://web.stanford.edu/~boyd/). There are superdetailed slides and videos here, which is quite beneficial.
2. other materials are directly included in this reository 
