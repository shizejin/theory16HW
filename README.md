# Advanced Economic Theory 2016 A1
##First topic: Equilibrium Computation for Two-Player Games in Strategic Form
### Part I [Support Enumeration](http://www.oyama.e.u-tokyo.ac.jp/theory16/vonStengel07_1.pdf)
Homework: write a homemade Python code to implement Support Enumeration Algorithm for computing the Nash Equilibra of Nondegenerate Two-Player Game. [Support Enumeration](http://nbviewer.jupyter.org/github/shizejin/theory16HW/blob/master/Support%20Enumeration%20%28for%20Nondegenerate%20Games%29.ipynb)
### Part II [Vertex Enumeration](http://www.oyama.e.u-tokyo.ac.jp/theory16/vonStengel07_3.pdf)
### Part III [Lemke Howson](http://www.oyama.e.u-tokyo.ac.jp/theory16/vonStengel07_3.pdf)
Homework: write a homemade Python code to implement Lemke Howson Algorithm for finding a Nash Equilibrium starting from atificial equilibrium (0,0).   
[lemke Howson](http://nbviewer.jupyter.org/github/shizejin/theory16HW/blob/master/Lemke%20Howson.ipynb)   
[lemke Howson (integer pivoting)](http://nbviewer.jupyter.org/github/shizejin/theory16HW/blob/master/Lemke%20Howson%20%28Integer%20Pivoting%29.ipynb)  
[lemke Howson (Enumeration)](http://nbviewer.jupyter.org/github/shizejin/theory16HW/blob/master/Lemke%20Howson%20%28find%20all%20NEs%20that%20can%20be%20reached%29.ipynb)  
[lemke Howson (degenerate game)](http://nbviewer.jupyter.org/github/shizejin/theory16HW/blob/master/Lemke%20Howson%20%28degenerate%20game%29.ipynb)
##Second topic: From Imitation Games to Kakutani  
[From Imitation Games to Kakutani](http://www.oyama.e.u-tokyo.ac.jp/theory16/McLennanTourky06.pdf)  
Homework: Write your own code for the McLennan-Tourky algorithm in Python or Julia (or both) using your Lemke-Howson implementation, and run it for several example functions on a Jupyter notebook.  
[ From Imitation to Kakutani](http://nbviewer.jupyter.org/github/shizejin/theory16HW/blob/master/From%20Imitation%20to%20Kakutani.ipynb)  
HW5 [Experimental Analysis of Lemke Howson Algorithm](https://github.com/shizejin/theory16HW/blob/master/Experimental%20Analysis%20of%20Lemke%20Howson%20Algorithm.ipynb)  
(see [reference](https://arxiv.org/pdf/0811.3247v1.pdf) here)  
In my codes, I use the lemke howson function from QuantEcon package by Oyama sensei. I change the source code in my computer so that the lemke howson function can return a bool variable that whether NE is achieved in limited steps and a integer variable that shows how many steps it use (if NE is not found, then the returned step number is exactly capping).  
The graph don't show significantly improvement in steps lemke howson use to find a NE when we limit the steps for each guess initial pivot. I think this is because I run too few simulations.
