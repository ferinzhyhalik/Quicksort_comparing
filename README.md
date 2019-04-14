# Quicksort_comparing

Operation System UPH 2017/2018 Parallel vs Singular Quicksort Comparison

## What is needed

* GCC

## installing
1. Download quicksort.c and quicksort_parallel.c
2. Make sure the file is can be compiled 
3. Execute file using  "./quicksort (samplesize).txt" or "./quicksort_parallel (samplesize).txt"

## Running the tests

Test is done with both sequential and parallel quicksort programs to find the time taken to finish quicksorting with a sample size of 10, 100, 1000 and 10000.

### Sequential 

| Sample Size | Test 1 Time | Test 2 Time | Test3 Time | Average Time |
|---|---|---|---|---|
| 10 | 0.00 ms | 0.001 ms | 0.002 ms | 0.002 ms|
| 100 | 0.01 ms | 0.043 ms | 0.017 ms | 0.021 ms |
| 1000 | 0.543 ms | 0.0504 ms | 0.487 ms | 0.509 ms |
| 10000 | 31.954 ms | 34.133 ms | 32.917 ms | 33.004 ms |

### Parallel

| Sample Size | Test 1 Time | Test 2 Time | Test3 Time| Average Time |
|---|---|---|---|---|
| 10 | 1.055 ms | 2.501 ms | 2.545 ms | 2.533 ms |
| 100 | 7.801 ms | 8.449 ms | 7.755 ms | 8.0647 ms |
| 1000 | 291.631 ms | 192.32 ms | 182.317 ms | 556.949 ms |
| 10000 | 17156.478 ms | 15086.526 ms | 13648.908 ms | 14294.512 ms |
## Result

### Result Comparison

| Sample Size | Sequence | Parallel |
|---|---|---|
|10| 0.001 ms | 1.675 ms |
|100| 0.031 ms | 8.752 ms |
|1000| 0.624 ms | 251.625 ms | 
|10000| 33.637 ms | 17560.684 ms |

### Line Graph Comparison

![Comparison Graph](https://github.com/ferinzhyhalik/Quicksort_comparing/blob/master/quicksort%20chart.PNG)

### Result analysis

From the result we can conclude that sequential quicksort is faster than parallel quicksort. But may be vary if the sample data have more datas etc. Another thing that have a significant impact of a program runtime are the hardware that the user used. In the end , the time for each user may be vary.
Parallel quicksort have so much work to do in so little time (racing against sequential).

## Authors

* **Ferinzhy Halik** - TIF UPH 2017


## Acknowledgments

* Quicksort program used are taken from [markwkm quicksort repository](https://github.com/markwkm/quicksort)
* Template README.md used are taken from [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
