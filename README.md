# NMF-using-GradientDescent-from-scratch
Implementing Non-negative Matrix Factorization  using Gradient Descent from the scratch


Code Flow:

   ![ScreenShot](https://github.com/saikarthikcheedella/NMF-using-GradientDescent-from-scratch/blob/master/NMF_using_GD_tob.PNG)

NMF approximates a matrix 'R' with a low-rank matrix approximation such that,

**R = B.C**

**(n*m) = (n*d).(d*m)**
    
where, R = orginal matrix [ratings matrix (or) any sparse matrix]

   B,C = non-negative matrices factors of R
       
Product of B and C gives a matrix of shape equvivalent to R. So, using B.C we can fill the sparsity of R.
Therefore, task lies in finding optimal B & C, in such a way that the our **"LOSS = argmin ||R-B.C'||^2"** should be minimised.

steps:
  1) Initialize B, C (randomly
  2) Converge to local minima(i.e. point where our Loss is minimal, through out the feature space)  
  3) Calculate partial derivatives of "Loss function" with respect to B and C.
      
      **B = B-d(Loss)/dB = B-(B.C.C' - R.C')**
      
      **C = C-d(Loss)/dC = C-(B'.B.C - B'.R)**
   
   
