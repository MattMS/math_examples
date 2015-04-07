# Matrix scalar multiplication

## Variables

Input matrix.

	A = [
		[1, 2, 3]
		[4, 5, 6]
	]

Multiplication value.

	scalar_value = 10

Expected output matrix.

	expected = [
		[10, 20, 30]
		[40, 50, 60]
	]

Multiplied matrix from the input matrix.

	result = []

Number of rows.

	row_count = A.length


## Main loop

Loop and save a reference to each of the rows.

	for j in [0...row_count]
		A_row = A[j]

		result_row = []

Get the number of columns.

		column_count = A_row.length

		for i in [0...column_count]
			value = A_row[i] * scalar_value

			result_row.push value

		result.push result_row


## Results

Display the results.

	console.log result
	console.log expected
	#console.log `result == expected`