# Off-by-One Error in COBOL Loop

This repository demonstrates a common off-by-one error that can occur in COBOL loops. The program intends to count from 1 to 10, but due to an incorrect loop condition, it might produce unexpected results.

## Bug Description
The `PERFORM VARYING` statement, which is a fundamental looping construct in COBOL, can sometimes lead to off-by-one errors if the loop termination condition is not carefully constructed. In this example, we want to iterate ten times, but a subtle error in the comparison causes the loop to iterate either one time too few or one time too many.

## Bug Solution
The solution involves carefully examining the loop condition and ensuring it accurately reflects the intended number of iterations. Often, the mistake is in the comparison operator (e.g., using '<=' instead of '<', or vice versa).