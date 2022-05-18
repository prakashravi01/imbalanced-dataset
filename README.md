# imbalanced-dataset

# Introduction

This project attempts to solve the problems caused in fuctioning of machine/models while dealing imbalanced classes od data.

# Problem Statement

When a data with huge gap among the possible classes is fed into a machine, after passing through a lot of **monotic** data samples, the machine/model behaves in a
biased way, yielding motnotonic results, without even testing the samples. Which was never observed while training the model.
Hence, the training and testing results of the model yiels a huge mismatch which can be termed as **Malfunctioning**

# Possible Solutions :
The following methods can be applied for solving the above stated :
-       Over Sampling
-       Under Sampling
-       Focal Loss Under Sampling
-       Ensemble Over Sampling
-       K - wieghted classification

# Failures of the Approaches :

-       Over Sampling (or Random Over Sampling) asks for generating a huge number of samples for the minority class(es) which wastes a lot of memory unnecessarily
-       Under Sampling ignores a lot of **potential** information which might be of use to the model
-       Focal Loss is another statistical approach towards Over Sampling which again associates to the requirement of unnecessary wastage of the device's memory
-       Ensemble method is another approach towards Over Sampling where one creates a synthetic sample of the minority samples and the **nearby** majority samples

# Resolution

In stead of created new or ignring available samples, we can deal with the same available dataset by delivering a **virtual** input to the model which is **weighted sample**
of the original data

# Achivements

Going ahead with the **K-weighted** approach we obtain the maximum accuracy/effieciency during the test of the model, while other approaches failed to yield.
