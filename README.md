# NMF-using-GradientDescent-from-scratch
Implementing Non-negative Matrix Factorization  using Gradient Descent from the scratch


Implementation flow:

   ![ScreenShot](https://github.com/saikarthikcheedella/NMF-using-GradientDescent-from-scratch/blob/master/NMF_using_GD_tob.PNG)

NMF approximates a matrix 'R' with a low-rank matrix approximation such that,
        R = B.C
    n*m = (n*d).(d*m) 
    
where, R = orginal matrix [ratings matrix (or) any sparse matrix]
       B,C = non-negative matrices factors of R
       
Product of B and C gives a matrix of shape equvivalent to R. So, using B.C we can fill the sparsity of R.
Therefore, task lies in finding optimal B & C, so that the #LOSS = argmin ||R-B.C.T||^2 should be minimised.

steps:
  1) Initialize B, C 
  2)
  3)
