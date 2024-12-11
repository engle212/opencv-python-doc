---
title: Linear Discriminant Analysis
layout: default
parent: Operations on Arrays
grand_parent: Core
nav_order: 1
---
# Linear Discriminant Analysis
## Constructors
### cv2.LDA(num_components)
> Initializes a LDA with num_components (default 0).

#### Parameters:
> *num_components*: int, optional, default: 0

### cv2.LDA(src, labels, num_components)
> Initializes and performs a Discriminant Analysis with Fisher's Optimization Criterion on given data in src and corresponding labels in labels. If 0 (or less) number of components are given, they are automatically determined for given data in computation.

#### Parameters:
> *src*: 2-dimensional array

> *labels*: 1-dimensional array

> *num_components*: int, optional, default: 0

## Member Functions
### cv2.LDA.compute(src, labels)
> Compute the discriminants for data in src (row aligned) and labels. Calls cv2.LDA.lda(src, labels).

#### Parameters
> *src*: 2-dimensional array

> *labels*: 1-dimensional array

### cv2.LDA.eigenvalues()
> Returns the eigenvalues of this LDA.

### cv2.LDA.eigenvectors()
> Returns the eigenvectors of this LDA.

### cv2.LDA.lda(src, labels)
> Compute the discriminants for data in src (row aligned) and labels.

#### Parameters
> *src*: 2-dimensional array

> *labels*: 1-dimensional array

### cv2.LDA.load(file)
> Deserializes this object from a given file or file path.

#### Parameters
> *file*: cv2.FileStorage or str

### cv2.LDA.project(src)
> Projects samples into the LDA subspace. src may be one or more row aligned samples.

#### Parameters
> *src*: 1-dimensional array

### cv2.LDA.reconstruct(src)

### cv2.LDA.save(file)
> Serializes this object to a given file.

#### Parameters
> *file*: cv2.FileStorage or str

### cv2.LDA.subspaceProject(W, mean, src)
>

#### Parameters
> *W*: 

> *mean*: 

> *src*: 

## Member Variables
### cv2.LDA._eigenvalues
> array

### cv2.LDA._eigenvectors
> array

### cv2.LDA._num_components
> int