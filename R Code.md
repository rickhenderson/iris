```R

# select 1 through 9th row, all columns
iris[1:9,]
# select 1st column through 4th column, all rows
iris[,1:4]
# calculate column sums 
colSums(iris[,1:4])
rowSums(iris[1:2,1:4])
dim(iris) #150R x 5C

iris[c('Sepal.Length','Petal.Length')]
#iris$Sepal.Length<5 creates a vector of TRUE & FALSES
iris[iris$Sepal.Length<5,]

#redo  -- Same as previous code snippet
tf <- iris$Sepal.Length<5
iris[tf,]
str(th)
#redo with subset
subset(iris,Sepal.Length<5)

#random selection of sample
x <- sample(1:nrow(iris), 0.33 * nrow(iris),replace=F)
iris[x,]
```

