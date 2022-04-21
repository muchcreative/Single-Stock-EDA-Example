## Normalization Vs Standardization

"Two there should be. No more, no less."

**Let's Start with the Difference Between the Two**

Taken from [GeeksForGeeks: Normalization Vs Standardization](https://www.geeksforgeeks.org/normalization-vs-standardization/]).t



Normalization is used to transform features to be on a similar scale.

Standardization is the transofrmation of features by subtracting from mean and dividng by standard deviation

**Normalization:**

**Standardization:**

Standardization can be helpful in cases where the data follows a Gaussian distribution. 
However, this does not have to be necessarily true. Geometrically speaking, it translates the data to the mean vector of original data to the origin and squishes or expands the points if std is 1 respectively. 
We can see that we are just changing mean and standard deviation to a standard normal distribution which is still normal thus the shape of the distribution is not affected.

Standardization does not get affected by outliers because there is no predefined range of transformed features.
