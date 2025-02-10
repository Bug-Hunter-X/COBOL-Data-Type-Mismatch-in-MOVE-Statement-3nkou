# COBOL Data Type Mismatch Bug
This example demonstrates a common error in COBOL programs: attempting to move data between fields of incompatible data types. Specifically, it showcases moving an alphanumeric field to a numeric field without proper conversion.

## Bug Description
The bug lies in the MOVE statement where an alphanumeric field (`WS-AREA-1`) is moved to a numeric field (`WS-AREA-2`).  COBOL's strict type checking will result in unpredictable behavior, possibly generating runtime errors or incorrect data values.

## Solution
The solution involves adding explicit data type conversion before the MOVE operation or using a temporary numeric field for data transfer. Refer to `bugSolution.cob` for the corrected code.