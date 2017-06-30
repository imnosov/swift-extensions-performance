# Benchmark of Swift extensions compilation times

This benchmark compares compilation time of class with N method vs. time to compile class and N single-method extensions in Swift.

## Usage

```
rake benchmark
```

## Results

On my machine it produces the following results:

![Benchmark results](results_chart.png?raw=true "Compilation times")

| n | methods | extensions |
| ---: | ---: | ---: |
|100 | 0,3033 | 0,27 |
|1000 | 2,2733 | 1,96 |
|2000 | 5,02 | 4,1267 |
|3000 | 8,22 | 6,52 |
|5000 | 15,9 | 13,95 |
|10000| 41,3 | 35,43 |
