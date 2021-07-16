# BPS Data Storing Format

BPS is a key-value data storing structure. It allows to store data in several types, even array.

## Specification

- **Comments**: BPS allows one-line comments. Comments start with hash symbol (`#`). E.g. `# This is a comment`.
- **Keys**: keys can be started with underscore (`_`) or letter, followed of numbers, lower or upper case letters and/or underscores.
- **Values**:
  * **Strings**: strings should be in double-quotes. E.g. `"this is a string"`.
  * **Chars**: chars should be in quotes. E.g. `'c'`.
  * **Integers**: e.g. `256`.
  * **Float**: floats can be write `256.`, `256.0` or `256f`.
  * **Double**: e.g. doubles can be write `256.0d` or `256d`.
  * **Boolean**: booleans can be `true` or `false`.
  * **Array**: arrays should be between braces (`[ ]`) separated by comma `,`. E.g. `[0, 1, 2]`, `['a', 'b', 'c']`, `[[0, 1], [0, 1]]` and so on.

## File in BPS Notation

```

# All data types of a BPS file.

# Literals
string:"string \"between\" double quotes";
char:'c';
quote_in_char:'\'';

# Numerics
int:10;
float:0.5;

# Booleans
boolTrue:true;
boolFalse:false;

# Vector
stringArr:["yes", "no", "maybe"];
chargArr:['a', 'b', 'c'];
intArr:[0, 1, 2, 10, -5];
floatArr:[0.9, 1.7, -0.2, 1.06, -5.618];
boolArr:[true, false, true];

# Multdimensional array
multArr2:[
  [0, 1, 2],
  [0, 1, 2],
  [0, 1, 2]
];

# And so on
multArr3:[
  [
    [0, 1, 2],
    [0, 1, 2],
    [0, 1, 2]
  ],
  [
    [0, 1, 2],
    [0, 1, 2],
    [0, 1, 2]
  ],
  [
    [0, 1, 2],
    [0, 1, 2],
    [0, 1, 2]
  ]
];

```
