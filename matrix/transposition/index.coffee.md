# Matrix transposition

Transposition is commutative, so `transpose(transpose(A)) is A`.


## Variables

Input matrix.

	A = [
		[1, 2, 3]
		[4, 5, 6]
	]

Expected output matrix.

	expected = [
		[1, 4]
		[2, 5]
		[3, 6]
	]

Transposed matrix from the input matrix.

	result = []
	
Index of the current column.

	i = 0

Flag to show if there are more columns to transpose.

	more_columns = yes

Number of rows.

	row_count = A.length


## Main loop

Keep looping while there are more columns to transpose.

	while more_columns

While looping the input columns, the result rows are added.

		result_row = []

Loop each of the rows on the same column.

		for j in [0...row_count]

Make sure this row has the column value.

			if A[j].length <= i
				more_columns = no
				break

Add the column value to the result row.

			result_row.push A[j][i]

Only add the row if the column was complete.

		if more_columns
			result.push result_row

Move to the next column index.

		i += 1


## Results

Display the results.

	console.log result
	console.log expected
	#console.log `result == expected`