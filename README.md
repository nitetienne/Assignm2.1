# Assignm2.1
====================================
-#tapply() is used to apply a function over subsets of a vector. 
-#It can be thought of as a combination of split() and sapply() for vectors only
+x<-c(rnorm(20),runif(20),rnorm(20,1))
+f<-gl(3,20)
+tapply(x,f,mean)
+      1         2         3 
+0.1826816 0.4013027 1.2849144 

-#Here’s an example of finding the range of each sub-group:
+tapply(x,f,range)
+$`1`
+[1] -1.062859  1.290395

+$`2`
+[1] 0.04749428 0.93141368

+$`3`
+[1] -0.3890658  3.3022838

-#vapply() is similar to sapply(), but has a pre-specified type of return value.

-#Thank you! 
