# Fractal-Clustering

### Objective:

To find hotspots where prices are high for traveling same distance in comparison to other pickup locations. The goal being better fleet management.

### Business Objective:

To provide better fare prices to customers in this location by increasing the supply of drivers. This might essentially give a competitive edge over the competitors.

We can use this metric to look for clusters where the fare to haversine ratio is greater than 3.9 which is approximately 30% greater than the average fare to km ratio. (as 3.03 is the point of reference for the calculations)

https://www.timeout.com/newyork/news/nyc-is-home-to-the-most-expensive-uber-rides-in-the-u-s-071522 as per this article the Average cost for uber in New York is $34.74 for 6.2 mile, which is equivalent to $3.47 per km, considering a 2% consumer inflation the same would have costed on an average $3.03 for the year range 2009 to 2015 (Which is the timeline of the available data)

### Objective Function:

First objective function is to find trips with minimum haversine distance.

Second objective function is to find trips with maximal fare value.

Based on the two objective fuctions, we define the combined objective function as the ratio of fare price to haversine distance.

The fare to haversine ratio is nothing but the cost per km.

We ought to maximize this ratio to find the golden cluster.
