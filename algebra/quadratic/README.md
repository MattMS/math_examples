# Quadratic equation and formula

- `x` is the only unknown (univariate), a non-zero integer.

- `a`, `b` and `c` are constants and `a isnt 0`.


## Quadratic equation

```coffee
y = (a * x * x) + (b * x) + c
```


## Quadratic formula

```coffee
square_root = (value)->
	Math.sqrt value

when_y_is_zero = (a, b, c)->
	ac4 = 4 * a * c
	bb = b * b
	bb_ac4 = bb - ac4

	n_sqrt = square_root bb_ac4

	a2 = 2 * a
	neg_b = -1 * b

	x1_top = neg_b + n_sqrt
	x1 = x1_top / a2

	x2_top = neg_b - n_sqrt
	x2 = x2_top / a2

	[x1, x2]
```


## Factoring

```coffee
y = ((p * x) + q) * ((r * x) + s)
```

```coffee
when_y_is_zero = (p, q, r, s)->
	neg_q = -1 * q
	x1 = neg_q / p

	neg_s = -1 * s
	x2 = neg_s / r

	[x1, x2]
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
