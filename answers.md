# CMPS 6610 Problem Set 03
## Answers

**Name:<u>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Rob Hartley</u>___________


Place all written answers from `problemset-03.md` here for easier grading.




- **1b.**  
$W(n) =W(n -1) +1$

    Level 1  
  $W(n) = (W(n -1 -1) + 1) + 1$  
  $W(n) = W(n -2) + 2$

  Level 2  
  $W(n) = (W(n-2 - 1) + 1) + 2$  
  $W(n) = W(n - 3) + 3$

  Generalized Equation  
    $W(n) = W(n - k) + k$

  Recursion Depth  
  $n - k = 0$
  $k = n$

  Substitute  
  $W(n) = W(n - n) + n$  
  $W(n) = W(0) + n$

  $\boxed{W(n) \in \Theta(n)}$

  $\boxed{S(n) \in \Theta(n)}$
  




- **1d.**  
  $W(n) = 2W(\frac{n}{2}) + 1$  

  Level 1  
  $W(n) = 2 \cdot (2W(\frac{n}{4} + 1) + 1$  
  $W(n) = 4W(\frac{n}{4}) + 3$  

  Level 2  
  $W(n) = 4 \cdot (2W(\frac{n}{8} + 1) + 3$  
  $W(n) = 8W(\frac{n}{8}) + 7$  

  Generalized Equation    
  $W(n) = 2^kW(\frac{n}{2^k}) + (2^k - 1)$

  Recursion Depth    
  $\frac{n}{2^k} = 1$  
  $n = 2^k$   
  $k = \lg n$  

  Substitute  
  $W(n) = 2^{\lg n}W(\frac{n}{2^k}) + (2^{\lg n} - 1)$  
  $W(n) = nW(1) + n - 1$

  $\boxed{W(n) \in \Theta(n)}$

  $S(n) = S(\frac{n}{2}) + 1$

  Level 1  
  $S(n) = S(\frac{n}{4}) + 1 + 1$  
  $S(n) = S(\frac{n}{4}) + 2$

  Level 2  
  $S(n) = S(\frac{n}{8}) + 1 + 2$  
  $S(n) = S(\frac{n}{8}) + 3$

  Generalized Equation  
  $S(n) = S(\frac{n}{2^k}) + k$

  Recursion Depth  
  $\frac{n}{2^k} = 1$  
  $n = 2^k$  
  $k = \lg n$  

  Substitute  
  $S(n) = S(\frac{n}{2^{\lg n}}) + \lg n$  
  $S(n) = S(1) + \lg n$

  $\boxed{S(n) \in \Theta(\log n)}$

  
  





- **1e.**  
  $W(n) = W(\frac{n}{3}) + W(\frac{2n}{3}) + 1$

    Level 1  
  $W(n) = [W(\frac{n}{9}) + W(\frac{2n}{9}) + 1] + [W(\frac{2n}{9}) +  W(\frac{4n}{9}) + 1] + 1$  
  $W(n) = W(\frac{n}{9}) + 2W(\frac{2n}{9}) + W(\frac{4n}{9}) + 3$

  Observations  
  $\frac{n}{9} + \frac{2n}{9} \frac{2n}{9} + \frac{4n}{9} = n$  
  Subproblem sizes sum to n.  
  Changes to parallelism do not affect total work. The ureduce algorithm performs the same overall computation as the reduce algorithm with different parallelism.  
  Both of these algorithms should therefore require the same work.  
  Because these algorithms are both asymptotically dominant when used
  in the implementation of rsearch, the work of both implementations should be the same.

  $\boxed{W(n) \in \Theta(n)}$

  $S(n) = S(\frac{2n}{3}) + \Theta(1)$  

  Level 1  
  $S(n) =  S(\frac{2}{3} \cdot \frac{2}{3} \cdot n) + 2\Theta(1)$

  Generalized Equation  
  $S(n) = S((\frac{2}{3})^kn) + k\Theta(1)$

  Recursion Depth  
  $(\frac{2}{3})^kn = 1$  
  $(\frac{2}{3})^k = \frac{1}{n}$  
  $k\log\frac{2}{3} = \log\frac{1}{n}$  
  $k\log\frac{2}{3} = -\log n$  
  $k = -\frac{\log n}{\log\frac{2}{3}}$  
  $k = \frac{\log n}{\log\frac{3}{2}}$  
  $k = \log_{3/2} n$

  Substitute  
  $S(n) = S((\frac{2}{3})^{\log_{3/2} n}n) + \log_{3/2} n\Theta(1)$  
  $S(n) = S((\frac{3}{2})^{-1 \cdot \log_{3/2} n}n) + \log_{3/2} n\Theta(1)$  
  $S(n) = S(\frac{1}{(\frac{3}{2})^{log_{3/2} n}}n) + \log_{3/2} n\Theta(1)$  
  $S(n) = S(1) + \log_{3/2} n\Theta(1)$

  $\boxed{S(n) \in \Theta(\log n)}$
  
  





- **2a.**





- **2b.**





- **2c.**






- **3b.**





- **3d.**





- **3f.**




