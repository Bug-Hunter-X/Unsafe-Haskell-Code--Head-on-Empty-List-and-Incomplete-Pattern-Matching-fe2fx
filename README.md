# Haskell Bug: Unsafe List Operations and Incomplete Pattern Matching

This repository demonstrates a common error in Haskell: using `head` on an empty list and incomplete pattern matching.  This results in runtime exceptions and unpredictable behavior.

The `bug.hs` file contains the erroneous code. The `bugSolution.hs` file provides a corrected version.

**Problem:**

The original code attempts to access the head of a potentially empty list without checking for emptiness, and it has incomplete pattern matching in the `case` statement.

**Solution:**

The solution involves robust error handling.  It uses safe functions like `maybe` or pattern matching to avoid runtime errors.