[![Build Status](https://travis-ci.com/sbohora/Somya.svg?token=shyYTzvvbsLRHsRAWXTg)](https://travis-ci.com/sbohora/Somya)

# Somya: Some outstanding magics you'd appreciate
This package provides some outstanding magical tricks/functions which are very useful in research, statistics and data science. This is a special package for me since this is named under my daughter `Somya`.

## Installation

``` r
# This package has not been submitted to CRAN yet. You can install its development version from GitHub:

# install.packages("devtools")
devtools::install_github("sbohora/Somya")
```

If any bug is encountered, please raise an issue with a minimal reproducible example on [GitHub](https://github.com/sbohora/Somya/issues).

## Few Examples

**`capitalize_each_word`**

```r
capitalize_each_word("make each letter in this string capitalized.", pattern = NULL)
[1] "Make Each Letter In This String Capitalized."
capitalize_each_word("make_each _etter_in_this_string_capitalized.", pattern = "[_]")
[1] "Make Each  Etter In This String Capitalized."
capitalize_each_word("make.each.letter.in.this.string.cpitalized.", pattern = "[.]")
[1] "Make Each Letter In This String Cpitalized "
```

**`compute_fibonacci`**

```r
compute_fibonacci(5)
[1] 5
> n = 10
> for (i in 0:(n-1)) {
+   print(compute_fibonacci(i))
+ }
[1] 0
[1] 1
[1] 1
[1] 2
[1] 3
[1] 5
[1] 8
[1] 13
[1] 21
[1] 34
```
**`is_palindrome`**

```r
is_palindrome("Was It A Rat I Saw?")
[1] TRUE
```

**`calculate_postfix`**

```r
calculate_postfix("2 3 1 * + 9 - ")
[1] "The result is: -4"
```