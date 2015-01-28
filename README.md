<p align="center">
  <a href="https://github.com/joelpurra/jqnpm"><img src="https://rawgit.com/joelpurra/jqnpm/master/resources/logotype/penrose-triangle.svg" alt="jqnpm logotype, a Penrose triangle" width="100" border="0" /></a>
</p>

# [jq-bigint](https://github.com/joelpurra/jq-bigint)

A [big integer library](https://gist.github.com/pkoppstein/d06a123f30c033195841) for working with possibly-signed arbitrarily long decimal strings. Written by Peter Koppstein ([@pkoppstein](https://github.com/pkoppstein)) and released under the MIT license.

This is a package for the command-line JSON processor [`jq`](https://stedolan.github.io/jq/). Install the package in your jq project/package directory with [`jqnpm`](https://github.com/joelpurra/jqnpm):

```bash
jqnpm install joelpurra/jq-bigint
```



## Usage


```jq
import "joelpurra/jq-bigint" as BigInt;

# BigInt::negate:                # . * -1
# BigInt::lessOrEqual(x; y):     # x <= y
# BigInt::long_add(x;y):         # x+y
# BigInt::long_minus(x;y):       # x-y
# BigInt::long_power(i):         # .^i
# BigInt::long_multiply(x;y):    # x*y
# BigInt::long_divide(x;y):      # x/y => [q,r]
# BigInt::long_div(x;y):         # integer division
# BigInt::long_mod(x;y):         # %

# In all cases, x and y must be strings; . and i should be an integer or a string.
```



---

## License
Copyright (c) 2014, 2015 Peter Koppstein <https://github.com/pkoppstein> and Joel Purra <http://joelpurra.com/>
All rights reserved.

When using **jq-bigint**, comply to the MIT license. Please see the LICENSE file for details.
