# Matrix transposition

Transposition is commutative, so `transpose(transpose(A)) is A`.

	A = [
		[1, 2, 3]
		[4, 5, 6]
	]

	expected = [
		[1, 4]
		[2, 5]
		[3, 6]
	]

Store the transposed matrix.

	result = []
	
Index of the current column.

	i = 0

Flag to show if there are more columns to transpose.

	more_columns = yes

Store the number of rows.

	row_count = A.length

Keep looping while there are more columns to transpose.

	while more_columns
		result_row = []

Loop each of the rows on the same column.

		for j in [0...row_count]
			if A[j].length <= i
				more_columns = no
				break

			result_row.push A[j][i]

Only add the row if the column was complete.

		if more_columns
			result.push result_row

Move to the next column.

		i += 1

	console.log result
	console.log expected
	#console.log `result == expected`