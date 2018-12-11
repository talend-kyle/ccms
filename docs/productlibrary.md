# Products and libraries

We have two items under the product category: __On prem__ and __Cloud__. In our CCMS environment, you can think products as partitions of the repository. The __Cloud__ partion contains the libraries that contain objects related to the cloud release(s). The __On prem__ partition contains the libraries that contain the objects related to all other releases.

The libraries within each product contain the objects for a specific version within that product. CCMS libraries are meant to follow the architecture of the product documentation. This is why the libraries are named according to the specific product and product release cycle.

When you add new objects into the CCMS, you need to add it to the relevant product/library. How to read the table below:

- Find your the product area you are working on: cloud or on prem.
- Find the version your new topic or map needs corresponds to.
- Find the library version that you need to add the new topic or map to.

| Product | Version relation to product | Where to add topic? |
| ------------ | ------------- | ------------ |
| Cloud | Spring '19  | Spring '19 |
|           | Summer '19| 7.2 Summer '19              |
|           | Fall '19  | Fall '19              |
|           | Winter '20| 7.3 Winter '20              |
| On prem   | 7.2       |  7.2 - Summer '19             |
|           | 7.3       |  7.3 - Summer '20             |

!!! Note
There are more cloud releases that on prem release in a calendar year. This is the reason there are two combined libraries (7.2 - Summer '19 and 7.3 - Winter '20) which correspond to both cloud and on prem releases, and there are two unique libraries (Spring '19 and Fall '19) which correspond to unique cloud releases.  