# Quadratic equation and formula

- x is the only unknown (univariate), a non-zero integer.

- a, b and c are constants.

- a != 0.


## General quadratic equation

```coffee
(a * x * x) + (b * x) + c = 0
```


## Formula

```coffee
n_sqrt = (a, b, c)->
	ac4 = 4 * a * c
	bb = b * b
	bb_ac4 = bb - ac4
	Math.sqrt bb_ac4

a2 = 2 * a

x1 = (a, b, c)->
	n = -b + n_sqrt a, b, c
	n / a2

x2 = (a, b, c)->
	n = -b - n_sqrt a, b, c
	n / a2
```


## Factoring

```coffee
(px + q)(rx + s) == 0

x1 = -q / p

x2 = -s / r
```


## Golden ratio

The golden ratio is found as the solution of the quadratic equation:

```coffee
(x * x) - x - 1 is 0
(x * x) is (x + 1)
```


## Links

- [Factorization (Wikipedia)](https://en.wikipedia.org/wiki/Factorization)

- [Quadratic equation (Wikipedia)](https://en.wikipedia.org/wiki/Quadratic_equation)

- [Quadratic formula (Wikipedia)](https://en.wikipedia.org/wiki/Quadratic_formula)

- [Univariate (Wikipedia)](https://en.wikipedia.org/wiki/Univariate)
