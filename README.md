Run it in your browser here: [https://repl.it/@tmkadamcz/conversions-for-hypothesis-tests](https://repl.it/@tmkadamcz/conversions-for-hypothesis-tests)

# Example usage
## Input:
```python
################################
### Enter values below ===> ####
################################

# Estimated quantity
estimate = None

# Value of estimate under null hypothesis. Typically 0.
# Example: estimate_null_value = 42
estimate_null_value = 0

# 95% confidence interval. Two values separated by commas (a tuple).
# Example: ci95 = 0.3,2
ci95 = 0.13,2.3

# p-value for the hypothesis that estimate=estimate_null_value
# Example: p = 0.01
p = None

# Standard error of estimated quantity
# Example: standard_error = 1
standard_error = None

# Set to True if your estimate is a ratio.
is_ratio = False
# This will cause everything to be evaluated on the log scale,
# and exponentiated back before being returned by the program.
# Although the estimate of the ratio has an asymptotically normal
# distribution around the true ratio (via central limit theorem),
# the log of a ratio converges to normality much faster.


################################
### <=== Enter values above ####
################################
```
## Output
```
estimate             1.2149999999999999
estimate_null_value  0
ci95_left            0.13
ci95_right           2.3
p                    0.028175169634599
z                    2.194838709677419
standard_error       0.5535714285714286
```