# Matrix addition

Addition is commutative, so `A + B == B + A`.


## Variables

Input matrices.

	A = [
		[1, 2, 3]
		[4, 5, 6]
	]

	B = [
		[10, 20, 30]
		[40, 50, 60]
	]

Expected output matrix.

	expected = [
		[11, 22, 33]
		[44, 55, 66]
	]

Matrix from the input matrices.

	result = []

Number of rows.

	row_count = Math.min A.length, B.length


## Main loop

Loop and save a reference to each of the rows.
`i in [0...n]` works like `0 <= i < n`.
For last value: `..` is inclusive and `...` is exclusive.

	for j in [0...row_count]
		A_row = A[j]
		B_row = B[j]

		result_row = []

Get the number of columns.

		column_count = Math.min A_row.length, B_row.length

		for i in [0...column_count]
			value = A_row[i] + B_row[i]

			result_row.push value

		result.push result_row


## Results

	console.log result
	console.log expected
	#console.log `result == expected`