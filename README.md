# MySQL Functions Overview

MySQL functions are built-in routines that perform specific operations on data. They are powerful tools that help data managers perform complex calculations and data manipulation with a simple call.

## Functions Categories

### Numeric Functions
These functions handle numerical calculations and operations.
- **Examples**: `ROUND()`, `FLOOR()`, `CEIL()`, `ABS()`, `POW()`, `RAND()`, `SQRT()`

### String Functions
These functions perform operations on string data types.
- **Examples**: `CONCAT()`, `SUBSTRING()`, `LENGTH()`, `REPLACE()`, `TRIM()`, `UPPER()`, `LOWER()`

### Date and Time Functions
These functions deal with date and time types, allowing for various manipulations and queries.
- **Examples**: `NOW()`, `CURDATE()`, `DATE_ADD()`, `DATEIF()`, `EXTRACT()`, `FORMAT()`, `TIME_TO_SEC()`

### Control Flow Functions
These functions control the flow of query execution and handle conditional logic.
- **Examples**: `IF()`, `CASE`, `IFNULL()`, `NULLIF()`, `COALESCE()`

### Conversion Functions
These functions convert data from one type to another, often used to ensure proper data format.
- **Examples**: `CAST()`, `CONVERT()`, `BINARY()`

### Aggregate Functions
These functions perform calculations on a set of values and return a single result, often used in conjunction with `GROUP BY`.
- **Examples**: `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`, `GROUP_CONCAT()`

### Information Functions
These functions provide information about the database, tables, and the MySQL environment.
- **Examples**: `DATABASE()`, `VERSION()`, `USER()`, `CURRENT_USER()`, `SYSTEM_USER()`

### Full-Text Search Functions
Designed to handle and enhance text searching within databases.

## References
- [TechOnTheNet - MySQL Functions](https://www.techonthenet.com/mysql/functions/index.php)
- [MySQL Documentation - Built-In Function Reference](https://dev.mysql.com/doc/refman/8.4/en/built-in-function-reference.html)

## Topics

- Numeric Functions and Operators
- Aggregate Functions
- String Functions
- Date Functions in MySQL
- Calculating Dates and Times
- The `IFNULL` and `COALESCE` Functions
- The `IF` Function
- The `CASE` Operator

## Numeric Functions and Operators


| Name        | Description                                                       | How to Call         |
|-------------|-------------------------------------------------------------------|----------------------|
| `%`         | Modulo operator: Returns the remainder of a division operation.   | `a % b`              |
| `*`         | Multiplication operator: Multiplies two numbers.                   | `a * b`              |
| `+`         | Addition operator: Adds two numbers.                               | `a + b`              |
| `- (minus)` | Subtracts one number from another.                                 | `a - b`              |
| `- (sign)`  | Changes the sign of a number.                                      | `-a`                 |
| `/`         | Division operator: Divides one number by another.                  | `a / b`              |
| `ABS()`     | Returns the absolute value of a number.                            | `ABS(a)`            |
| `ACOS()`    | Returns the arc cosine (inverse cosine) of a number.               | `ACOS(a)`           |
| `ASIN()`    | Returns the arc sine (inverse sine) of a number.                    | `ASIN(a)`           |
| `ATAN()`    | Returns the arc tangent (inverse tangent) of a number.              | `ATAN(a)`           |
| `ATAN2()`   | Returns the arc tangent of the two arguments (y, x).                | `ATAN2(y, x)`       |
| `CEIL()`    | Returns the smallest integer greater than or equal to a number.    | `CEIL(a)`           |
| `CEILING()` | Returns the smallest integer greater than or equal to a number.    | `CEILING(a)`        |
| `CONV()`    | Converts numbers between different number bases.                   | `CONV(a, from_base, to_base)` |
| `COS()`     | Returns the cosine of an angle.                                    | `COS(a)`            |
| `COT()`     | Returns the cotangent of an angle.                                 | `COT(a)`            |
| `CRC32()`   | Computes a cyclic redundancy check value.                          | `CRC32(a)`          |
| `DEGREES()` | Converts radians to degrees.                                       | `DEGREES(a)`        |
| `DIV`       | Integer division: Returns only the integer part of the quotient.   | `a DIV b`           |
| `EXP()`     | Returns e raised to the power of a number.                         | `EXP(a)`            |
| `FLOOR()`   | Returns the largest integer less than or equal to a number.         | `FLOOR(a)`          |
| `LN()`      | Returns the natural logarithm (base e) of a number.                | `LN(a)`             |
| `LOG()`     | Returns the natural logarithm (base e) of a number.                | `LOG(a)`            |
| `LOG10()`   | Returns the base-10 logarithm of a number.                         | `LOG10(a)`          |
| `LOG2()`    | Returns the base-2 logarithm of a number.                          | `LOG2(a)`           |
| `MOD()`     | Returns the remainder of a division operation (similar to `%`).    | `MOD(a, b)`         |
| `PI()`      | Returns the value of π (pi).                                       | `PI()`              |
| `POW()`     | Returns a number raised to the power of another number.            | `POW(a, b)`         |
| `POWER()`   | Returns a number raised to the power of another number.            | `POWER(a, b)`       |
| `RADIANS()` | Converts degrees to radians.                                       | `RADIANS(a)`        |
| `RAND()`    | Returns a random floating-point number between 0 and 1.            | `RAND()`            |
| `ROUND()`   | Rounds a number to the nearest integer or to a specified number of decimal places. | `ROUND(a, n)`       |
| `SIGN()`    | Returns the sign of a number (-1 for negative, 1 for positive, 0 for zero). | `SIGN(a)`           |
| `SIN()`     | Returns the sine of an angle.                                      | `SIN(a)`            |
| `SQRT()`    | Returns the square root of a number.                               | `SQRT(a)`           |
| `TAN()`     | Returns the tangent of an angle.                                   | `TAN(a)`            |
| `TRUNCATE()`| Truncates a number to a specified number of decimal places without rounding. | `TRUNCATE(a, n)`    |


## String Functions

| Name               | Description                                                                                               | How to Call                                |
|--------------------|-----------------------------------------------------------------------------------------------------------|--------------------------------------------|
| `ASCII()`          | Return numeric value of left-most character                                                               | `ASCII(string)`                           |
| `BIN()`            | Return a string containing binary representation of a number                                              | `BIN(number)`                             |
| `BIT_LENGTH()`     | Return length of argument in bits                                                                         | `BIT_LENGTH(string)`                       |
| `CHAR()`           | Return the character for each integer passed                                                             | `CHAR(integer1, integer2, ...)`            |
| `CHAR_LENGTH()`    | Return number of characters in argument                                                                   | `CHAR_LENGTH(string)`                      |
| `CHARACTER_LENGTH()` | Synonym for `CHAR_LENGTH()`                                                                             | `CHARACTER_LENGTH(string)`                 |
| `CONCAT()`         | Return concatenated string                                                                              | `CONCAT(string1, string2, ...)`            |
| `CONCAT_WS()`      | Return concatenated string with separator                                                                 | `CONCAT_WS(separator, string1, string2, ...)` |
| `ELT()`            | Return string at index number                                                                            | `ELT(index, string1, string2, ...)`        |
| `EXPORT_SET()`     | Return a string such that for every bit set in the value bits, you get an "on" string and for every unset bit, you get an "off" string | `EXPORT_SET(value, on, off, separator)`   |
| `FIELD()`          | Index (position) of first argument in subsequent arguments                                                 | `FIELD(string, string1, string2, ...)`    |
| `FIND_IN_SET()`    | Index (position) of first argument within second argument                                                | `FIND_IN_SET(string, set)`                 |
| `FORMAT()`         | Return a number formatted to specified number of decimal places                                           | `FORMAT(number, decimal_places)`           |
| `HEX()`            | Hexadecimal representation of decimal or string value                                                     | `HEX(value)`                              |
| `INSERT()`         | Insert substring at specified position up to specified number of characters                               | `INSERT(string, position, length, substring)` |
| `INSTR()`          | Return the index of the first occurrence of substring                                                     | `INSTR(string, substring)`                |
| `LCASE()`          | Synonym for `LOWER()`                                                                                     | `LCASE(string)`                           |
| `LEFT()`           | Return the leftmost number of characters as specified                                                     | `LEFT(string, number_of_characters)`       |
| `LENGTH()`         | Return the length of a string in bytes                                                                     | `LENGTH(string)`                           |
| `LIKE`             | Simple pattern matching                                                                                   | `string LIKE pattern`                     |
| `LOAD_FILE()`      | Load the named file                                                                                       | `LOAD_FILE(file_path)`                     |
| `LOCATE()`         | Return the position of the first occurrence of substring                                                   | `LOCATE(substring, string, start_position)` |
| `LOWER()`          | Return the argument in lowercase                                                                          | `LOWER(string)`                            |
| `LPAD()`           | Return the string argument, left-padded with the specified string                                         | `LPAD(string, length, pad_string)`         |
| `LTRIM()`          | Remove leading spaces                                                                                    | `LTRIM(string)`                            |
| `MAKE_SET()`       | Return a set of comma-separated strings that have the corresponding bit in bits set                        | `MAKE_SET(bits, string1, string2, ...)`    |
| `MATCH()`          | Perform full-text search                                                                                  | `MATCH(column) AGAINST(expression)`       |
| `MID()`            | Return a substring starting from the specified position                                                  | `MID(string, start, length)`              |
| `NOT LIKE`         | Negation of simple pattern matching                                                                       | `string NOT LIKE pattern`                 |
| `NOT REGEXP`       | Negation of `REGEXP`                                                                                       | `string NOT REGEXP pattern`               |
| `OCT()`            | Return a string containing octal representation of a number                                                | `OCT(number)`                             |
| `OCTET_LENGTH()`   | Synonym for `LENGTH()`                                                                                     | `OCTET_LENGTH(string)`                     |
| `ORD()`            | Return character code for leftmost character of the argument                                              | `ORD(string)`                             |
| `POSITION()`       | Synonym for `LOCATE()`                                                                                     | `POSITION(substring IN string)`            |
| `QUOTE()`          | Escape the argument for use in an SQL statement                                                            | `QUOTE(string)`                           |
| `REGEXP`           | Whether string matches regular expression                                                                  | `string REGEXP pattern`                   |
| `REGEXP_INSTR()`   | Starting index of substring matching regular expression                                                   | `REGEXP_INSTR(string, pattern)`           |
| `REGEXP_LIKE()`    | Whether string matches regular expression                                                                  | `REGEXP_LIKE(string, pattern)`            |
| `REGEXP_REPLACE()` | Replace substrings matching regular expression                                                             | `REGEXP_REPLACE(string, pattern, replace)` |
| `REGEXP_SUBSTR()`  | Return substring matching regular expression                                                               | `REGEXP_SUBSTR(string, pattern)`          |
| `REPEAT()`         | Repeat a string the specified number of times                                                              | `REPEAT(string, number)`                  |
| `REPLACE()`        | Replace occurrences of a specified string                                                                  | `REPLACE(string, old_string, new_string)`  |
| `REVERSE()`        | Reverse the characters in a string                                                                        | `REVERSE(string)`                         |
| `RIGHT()`          | Return the specified rightmost number of characters                                                         | `RIGHT(string, number_of_characters)`      |
| `RLIKE`            | Whether string matches regular expression                                                                  | `string RLIKE pattern`                    |
| `RPAD()`           | Append string the specified number of times                                                                 | `RPAD(string, length, pad_string)`        |
| `RTRIM()`          | Remove trailing spaces                                                                                     | `RTRIM(string)`                            |
| `SOUNDEX()`        | Return a soundex string                                                                                   | `SOUNDEX(string)`                          |
| `SOUNDS LIKE`      | Compare sounds                                                                                           | `string SOUNDS LIKE pattern`              |
| `SPACE()`          | Return a string of the specified number of spaces                                                           | `SPACE(number)`                            |
| `STRCMP()`         | Compare two strings                                                                                       | `STRCMP(string1, string2)`                |
| `SUBSTR()`         | Return the substring as specified                                                                          | `SUBSTR(string, start, length)`          |
| `SUBSTRING()`      | Return the substring as specified                                                                          | `SUBSTRING(string, start, length)`       |
| `SUBSTRING_INDEX()`| Return a substring from a string before the specified number of occurrences of the delimiter                | `SUBSTRING_INDEX(string, delimiter, count)` |
| `TRIM()`           | Remove leading and trailing spaces                                                                         | `TRIM(string)`                             |
| `UCASE()`          | Synonym for `UPPER()`                                                                                      | `UCASE(string)`                            |
| `UNHEX()`          | Return a string containing hex representation of a number                                                    | `UNHEX(hex_string)`                       |
| `UPPER()`          | Convert to uppercase                                                                                      | `UPPER(string)`                            |
| `WEIGHT_STRING()`  | Return the weight string for a string                                                                      | `WEIGHT_STRING(string)`                   |


## Date and Time Functions

| Name                    | Description                                                       | How to Call                             |
|-------------------------|-------------------------------------------------------------------|-----------------------------------------|
| `ADDDATE()`             | Add time values (intervals) to a date value                      | `ADDDATE(date, interval)`               |
| `ADDTIME()`             | Add time to a datetime value                                      | `ADDTIME(datetime, time)`               |
| `CONVERT_TZ()`          | Convert from one time zone to another                             | `CONVERT_TZ(datetime, from_tz, to_tz)`  |
| `CURDATE()`             | Return the current date                                           | `CURDATE()`                             |
| `CURRENT_DATE()`        | Synonym for `CURDATE()`                                           | `CURRENT_DATE()`                        |
| `CURRENT_TIME()`        | Synonym for `CURTIME()`                                           | `CURRENT_TIME()`                        |
| `CURRENT_TIMESTAMP()`   | Synonym for `NOW()`                                               | `CURRENT_TIMESTAMP()`                   |
| `CURTIME()`             | Return the current time                                           | `CURTIME()`                             |
| `DATE()`                | Extract the date part of a date or datetime expression             | `DATE(datetime)`                        |
| `DATE_ADD()`            | Add time values (intervals) to a date value                       | `DATE_ADD(date, interval)`              |
| `DATE_FORMAT()`         | Format date as specified                                          | `DATE_FORMAT(date, format)`             |
| `DATE_SUB()`            | Subtract a time value (interval) from a date                      | `DATE_SUB(date, interval)`              |
| `DATEDIFF()`            | Subtract two dates                                                | `DATEDIFF(date1, date2)`                |
| `DAY()`                 | Synonym for `DAYOFMONTH()`                                        | `DAY(date)`                             |
| `DAYNAME()`             | Return the name of the weekday                                    | `DAYNAME(date)`                         |
| `DAYOFMONTH()`          | Return the day of the month (0-31)                                | `DAYOFMONTH(date)`                      |
| `DAYOFWEEK()`           | Return the weekday index of the argument                          | `DAYOFWEEK(date)`                       |
| `DAYOFYEAR()`           | Return the day of the year (1-366)                                | `DAYOFYEAR(date)`                       |
| `EXTRACT()`             | Extract part of a date                                            | `EXTRACT(unit FROM date)`               |
| `FROM_DAYS()`           | Convert a day number to a date                                    | `FROM_DAYS(day_number)`                |
| `FROM_UNIXTIME()`       | Format Unix timestamp as a date                                   | `FROM_UNIXTIME(timestamp)`             |
| `GET_FORMAT()`          | Return a date format string                                       | `GET_FORMAT(type, format)`             |
| `HOUR()`                | Extract the hour                                                   | `HOUR(time)`                            |
| `LAST_DAY`              | Return the last day of the month for the argument                 | `LAST_DAY(date)`                        |
| `LOCALTIME()`           | Synonym for `NOW()`                                               | `LOCALTIME()`                           |
| `LOCALTIMESTAMP()`      | Synonym for `NOW()`                                               | `LOCALTIMESTAMP()`                      |
| `MAKEDATE()`            | Create a date from the year and day of year                       | `MAKEDATE(year, day_of_year)`           |
| `MAKETIME()`            | Create time from hour, minute, second                             | `MAKETIME(hour, minute, second)`        |
| `MICROSECOND()`         | Return the microseconds from argument                             | `MICROSECOND(datetime)`                 |
| `MINUTE()`              | Return the minute from the argument                               | `MINUTE(time)`                          |
| `MONTH()`               | Return the month from the date passed                             | `MONTH(date)`                           |
| `MONTHNAME()`           | Return the name of the month                                      | `MONTHNAME(date)`                       |
| `NOW()`                 | Return the current date and time                                  | `NOW()`                                 |
| `PERIOD_ADD()`          | Add a period to a year-month                                      | `PERIOD_ADD(period, number)`            |
| `PERIOD_DIFF()`         | Return the number of months between periods                      | `PERIOD_DIFF(period1, period2)`         |
| `QUARTER()`             | Return the quarter from a date argument                           | `QUARTER(date)`                         |
| `SEC_TO_TIME()`         | Converts seconds to 'hh:mm:ss' format                             | `SEC_TO_TIME(seconds)`                  |
| `SECOND()`              | Return the second (0-59)                                          | `SECOND(time)`                          |
| `STR_TO_DATE()`         | Convert a string to a date                                        | `STR_TO_DATE(string, format)`           |
| `SUBDATE()`             | Synonym for `DATE_SUB()` when invoked with three arguments        | `SUBDATE(date, interval)`               |
| `SUBTIME()`             | Subtract times                                                    | `SUBTIME(time, interval)`               |
| `SYSDATE()`             | Return the time at which the function executes                    | `SYSDATE()`                             |
| `TIME()`                | Extract the time portion of the expression passed                 | `TIME(datetime)`                        |
| `TIME_FORMAT()`         | Format as time                                                     | `TIME_FORMAT(time, format)`             |
| `TIME_TO_SEC()`         | Return the argument converted to seconds                          | `TIME_TO_SEC(time)`                     |
| `TIMEDIFF()`            | Subtract time                                                      | `TIMEDIFF(time1, time2)`                |
| `TIMESTAMP()`           | With a single argument, this function returns the date or datetime expression; with two arguments, the sum of the arguments | `TIMESTAMP(datetime)` or `TIMESTAMP(date, time)` |
| `TIMESTAMPADD()`        | Add an interval to a datetime expression                          | `TIMESTAMPADD(unit, interval, datetime)` |
| `TIMESTAMPDIFF()`       | Return the difference of two datetime expressions, using the units specified | `TIMESTAMPDIFF(unit, datetime1, datetime2)` |
| `TO_DAYS()`             | Return the date argument converted to days                        | `TO_DAYS(date)`                         |
| `TO_SECONDS()`          | Return the date or datetime argument converted to seconds since Year 0 | `TO_SECONDS(date)`                      |
| `UNIX_TIMESTAMP()`      | Return a Unix timestamp                                           | `UNIX_TIMESTAMP(datetime)`              |
| `UTC_DATE()`            | Return the current UTC date                                       | `UTC_DATE()`                            |
| `UTC_TIME()`            | Return the current UTC time                                       | `UTC_TIME()`                            |
| `UTC_TIMESTAMP()`       | Return the current UTC date and time                              | `UTC_TIMESTAMP()`                       |
| `WEEK()`                | Return the week number                                            | `WEEK(date, [mode])`                    |
| `WEEKDAY()`             | Return the weekday index                                          | `WEEKDAY(date)`                         |
| `WEEKOFYEAR()`          | Return the calendar week of the date (1-53)                       | `WEEKOFYEAR(date)`                      |
| `YEAR()`                | Return the year                                                   | `YEAR(date)`                            |
| `YEARWEEK()`            | Return the year and week                                          | `YEARWEEK(date, [mode])`                |


