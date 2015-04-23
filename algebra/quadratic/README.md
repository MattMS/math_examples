# Quadratic equation and formula

- `x` is the only unknown (univariate), a non-zero integer.

- `a`, `b` and `c` are constants.

- `a isnt 0`.


## General quadratic equation

```coffee
0 is (a * x * x) + (b * x) + c
```


## Formula

```coffee
f = (a, b, c)->
	ac4 = 4 * a * c
	bb = b * b
	bb_ac4 = bb - ac4
	n_sqrt = Math.sqrt bb_ac4

	a2 = 2 * a
	neg_b = -1 * b

	x1_top = neg_b + n_sqrt
	x1 = x1_top / a2

	x2_top = neg_b - n_sqrt
	x2 = x2_top / a2
```


## Factoring

```coffee
0 is ((p * x) + q) * ((r * x) + s)

neg_q = -1 * q
x1 = neg_q / p

neg_s = -1 * s
x2 = neg_s / r
```


## Golden ratio

The golden ratio is found as the solution of the quadratic equation:

```coffee
0 is (x * x) - x - 1

(x * x) is (x + 1)
```


## Links

- [Factorization (Wikipedia)](https://en.wikipedia.org/wiki/Factorization)

- [Quadratic equation (Wikipedia)](https://en.wikipedia.org/wiki/Quadratic_equation)

- [Quadratic formula (Wikipedia)](https://en.wikipedia.org/wiki/Quadratic_formula)

- [Univariate (Wikipedia)](https://en.wikipedia.org/wiki/Univariate)
