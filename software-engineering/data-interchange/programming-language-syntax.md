# Programming Language

- Code Source File: .source
- Binary Format Source File: .binary
- .source Files Must be Statically Typed
- .source Files Cannot be Dynamically Typed
- .binary Files Must be Statically Typed
- .binary Files Cannot be Dynamically Typed
- .source || .binary Files are Required
- // This is a Comment

## Language Syntax

```shell
// Constant Keyword - const
// Data Structure Keyword - struct
// For Loop Keyword - for
// Function Keyword - func
// Else Condition Keyword - else
// Generic Type Keyword - type
// If Condition Keyword - if
// Reference Pointer Operator - &
// Target Pointer Operator - *
// Variable Keyword - var
// While Loop Keyword - while

// Data Structure Initialization
// Syntax - struct name {fields};
struct DataStructure {
	byte_type byte = null; // Encoding Dependent: ASCII, Binary, UTF-8, UTF-16, UTF-32
	unsigned_integer_size usize = 0; // Platform Dependent: x86, x86_64, AARCH32, AARCH64, RISC32, RISC64
	unsigned_integer_8bit uint8 = 1;
	unsigned_integer_16bit uint16 = 2;
	unsigned_integer_32bit uint32 = 3;
	unsigned_integer_64bit uint64 = 4;
	unsigned_integer_128bit uint128 = 5;
	signed_integer_size isize = null; // Platform Dependent: x86, x86_64, AARCH32, AARCH64, RISC32, RISC64
	signed_integer_8bit int8 = -1;
	signed_integer_16bit int16 = -2;
	signed_integer_32bit int32 = -3;
	signed_integer_64bit int64 = -4;
	signed_integer_128bit int128 = -5;
	float_32bit float32 = null;
	float_64bit float64 = 2.0;
	float_128bit float128 = 3.0;
	boolean_type bool = true;
	character_type char = 'a'; // Encoding Dependent: ASCII, UTF-8, UTF-16, UTF-32
	string_type str = "string"; // Encoding Dependent: ASCII, UTF-8, UTF-16, UTF-32
	array_type [5]uint8 = {};
	map_type map<uint8, str> = {};
	structure_type DataStructure = {};
};

// Variable Declaration
// Syntax - var name type;

// Boolean Initialization
// Syntax - var name type = value;
// OR
// Null Syntax - var name type = null;
var boolean_type bool = true;

// Character Initialization
// Syntax - var name type = value;
// OR
// Null Syntax - var name type = null;
// Encoding Dependent: ASCII, UTF-8, UTF-16, UTF-32
var character_type char = 'a';

// Float Initialization
// Syntax - var name type = value;
// OR
// Null Syntax - var name type = null;
var float_32bit float32 = 1.0;

// Integer Initialization
// Syntax - var name type = value;
// OR
// Null Syntax - var name type = null;
var unsigned_integer_8bit uint8 = 1;

// String Initialization
// Syntax - var name type = value;
// OR
// Null Syntax - var name type = null;
// Encoding Dependent: ASCII, UTF-8, UTF-16, UTF-32
var string_type str = "string";

// Array Initialization
// Syntax - var name [length]type = [values];
// OR
// Multi-Dimensional Syntax - var name [rows][columns]type = [values];
// OR
// Unknown Size Syntax - var name []type = [values];
// OR
// Null Syntax - var name [length]type = [null];
// Array Index Syntax - name[index]
var array_type [5]uint8 = [
	1,
	2,
	3,
	4,
	5
];

// Array Initialization
// Syntax - var name [length]type = {values};
// OR
// Multi-Dimensional Syntax - var name [rows][columns]type = {values};
// OR
// Unknown Size Syntax - var name []type = {values};
// OR
// Null Syntax - var name [length]type = {null};
// Array Index Syntax - name[index]
var array_type [5]uint8 = {
	1,
	2,
	3,
	4,
	5
};

// Hash Map Initialization
// Syntax - var name type<type, type> = {(key:value)};
// OR
// Null Syntax - var name type<type, type> = {(null:null)};
// Hash Map Index Syntax - name[key]
var map_type map<uint8, str> = {
	(1:"string"),
	(2:"string"),
	(3:"string"),
	(4:"string"),
	(5:"string")
};

// Function Declaration
// Syntax - func name(parameter type) type {scope};
func conditional_function(first_parameter int8, second_parameter int8) str {
	var result str;
	var number int8 = first_parameter - second_parameter;

	// If Conditional Statement
	// Syntax - statement (condition) {scope} branch {scope};
	if (number < 1) {
		result = "failed";
	} else {
		number = number + 1;
		result = "success";
	}

	return result;
};

// Function Declaration
// Syntax - func name(parameter type) type {scope};
func loop_function(first_parameter int8, second_parameter int8) uint8 {
	var index usize = 0;
	var array_type [3]uint8 = [
		0,
		1,
		2
	];
	var number int8 = first_parameter - second_parameter;
	
	// While Loop Statement
	// Syntax - statement (condition) {scope};
	while (number < 1) {
		number = number + 1;
	}

	// For Loop Statement
	// Syntax - statement (initial_condition; evalutation_condition; iteration_increment) {scope};
	for (index = 0; index < 2; index++) {
		array_type[index] = array_type[index + 1];
	}

	return value;
};
```

