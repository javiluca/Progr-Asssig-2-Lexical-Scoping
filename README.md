
Programming Assignment 2: Lexical Scoping

# read the R script
# A "square" matrix has to be created as `solve` only handles this kind of matrix.
# create the matrix during the call of makeCacheMatrix()


a <- makeCacheMatrix( matrix(c(1,2,12,13), nrow = 2, ncol = 2) )

> summary(a)
             Length Class  Mode    
setMatrix    1      -none- function
getMatrix    1      -none- function
cacheInverse 1      -none- function
getInverse   1      -none- function

 > a$getMatrix()
     [,1] [,2]
[1,]    1   12
[2,]    2   13

cacheSolve(a)
           [,1]        [,2]
[1,] -1.1818182  1.09090909
[2,]  0.1818182 -0.09090909

cacheSolve(a)
#when run the second time, we obtain the cached data
getting cached data
           [,1]        [,2]
[1,] -1.1818182  1.09090909
[2,]  0.1818182 -0.09090909


