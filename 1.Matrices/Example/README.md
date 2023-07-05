# A Motivating example.

In this topic we'll explore the machine learning task of feature extraction in linear algebraic terms. We'll discuss the conversion of these operations into math problems we can work with, so that we can ultimately be informed of what our data is doing.

Let us look at a specific case of a specific dataset and how you are going to extract feature from it. We can see how definition works out in that case.

## Example
Suppose you want to compute the total number of families that can live in Seattle given the number of buildings that hold k families for 
k = 1,2,...1000.

We would like to understand the above example in such a way that, we are given a vector consisting of number of buildings that can hold a certain number of families.
```
v = 
[
    v1
    v2
    v3
    .
    .
    .
    v1000
]

where v is represented as a vector.
```

**Total number of families** = `1.v1 + 2.v2 + 3.v3 + ... + 1000.v1000`
                             = `Sigma (1..1000) i.vi`

Now, if you observe along side the values of v1,v2...v1000 there are numbers 1,2,3...1000.
So, lets extract those numbers in a vector of their own. 

```
w = [ w1 w2 w3 ... w1000 ]

nothing but the weights...

w = [ 1 2 3 ... 1000 ]
```

So, the **Total number of families** = `Sigma (1..1000) wi.vi`

And this is the thing we are going to abstract away into our definition. This allows us to define a matrix product in case of row and column vectors.

```
where v & w are the column and row vectors respectively.

v = 
[
    v1
    v2
    v3
    .
    .
    .
    v1000
]

w = [ w1 w2 w3 ... w1000 ]

w.v = Sigma (1..1000) wi.vi = w1.v1 + w2.v2 + ... + w1000.v1000

```
**Total number of families** = `w.v` (. indicates the Dot Product between these two matrices w and v)

The row vector gives the vector of weights, we are using a weighted sum to extract the feature that comes out of the product.