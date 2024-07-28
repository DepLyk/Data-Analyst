# Cluster dendogram

dat=mtcars

pmatrix =  scale(dat)

d = dist(pmatrix)

c = hclust(d, method="ward.D2")

plot(c, main="Cluster dendrogram of mtcars", xlab="", sub="")

rect.hclust(c, k=4)
