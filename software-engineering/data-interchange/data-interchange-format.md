# Data Interchange Format

- Data Source File: .data
- Binary Format Source File: .binary
- Schema Definition Header File: .schema
- .data Files May be Dynamically Typed
- .data Files May be Statically Typed
- .binary Files Must be Statically Typed
- .binary Files Cannot be Dynamically Typed
- .data || .binary Files are Required
- .schema Files Must be Statically Typed
- .schema Files Cannot be Dynamically Typed
- .schema Files are Optional
- // This is a Comment

## Dynamically Typed Syntax

```shell
// Data Structure Initialized Declaration
// Syntax - Name {fields};
DataStructure {
	byte_type = null;
	integer_type = 1;
	float_type = 1.0;
	boolean_type = true;
	character_type = 'a';
	string_type = "string";
	array_type = {};
	map_type = {};
	structure_type = DataStructure {};
};

// Boolean Initialization
// Syntax - name = value;
// OR
// Null Syntax - name = null;
boolean_type = true;

// Byte Initialization
// Syntax - name = value;
// OR
// Null Syntax - name = null;
// Encoding Dependent: ASCII, Binary, UTF-8, UTF-16, UTF-32
byte_type = 'a';

// Character Initialization
// Syntax - name = value;
// OR
// Null Syntax - name = null;
// Encoding Dependent: ASCII, UTF-8, UTF-16, UTF-32
character_type = 'a';

// Float Initialization
// Syntax - name = value;
// OR
// Null Syntax - name = null;
float_type = 1.0;

// Integer Initialization
// Syntax - name = value;
// OR
// Null Syntax - name = null;
integer_type = 1;

// String Initialization
// Syntax - name = value;
// OR
// Null Syntax - name = null;
// Encoding Dependent: ASCII, UTF-8, UTF-16, UTF-32
string_type = "string";

// Array Initialization
// Syntax - name = {values};
// OR
// Null Syntax - name = {null};
array_type = {
	1,
	2,
	3,
	4,
	5
};

// Hash Map Initialization
// Syntax - name = {(key:value)};
// OR
// Null Syntax - name = {(null:null)};
map_type = {
	(1:"string"),
	(2:"string"),
	(3:"string"),
	(4:"string"),
	(5:"string")
};
```

## Statically Typed Syntax

```shell
// Data Structure Keyword - struct
// Generic Type Keyword - type
// Variable Keyword - var

// Data Structure Declaration
// Syntax - struct Name {fields};
struct DataStructure {
	byte_type: byte,
	unsigned_integer_size: usize,
	unsigned_integer_8bit: uint8,
	unsigned_integer_16bit: uint16,
	unsigned_integer_32bit: uint32,
	unsigned_integer_64bit: uint64,
	unsigned_integer_128bit: uint128,
	signed_integer_size: isize,
	signed_integer_8bit: int8,
	signed_integer_16bit: int16,
	signed_integer_32bit: int32,
	signed_integer_64bit: int64,
	signed_integer_128bit: int128,
	float_32bit: float32,
	float_64bit: float64,
	float_128bit: float128,
	boolean_type: bool,
	character_type: char,
	string_type: str,
	array_type: [5]uint8,
	map_type: map<uint8, str>,
	structure_type: DataStructure
};

// Data Structure Initialization
// Syntax - var name: type = {fields};
var structure_type: DataStructure = {
	byte_type: null,
	unsigned_integer_size: 0,
	unsigned_integer_8bit: 1,
	unsigned_integer_16bit: 2,
	unsigned_integer_32bit: 3,
	unsigned_integer_64bit: 4,
	unsigned_integer_128bit: 5,
	signed_integer_size: null,
	signed_integer_8bit: -1,
	signed_integer_16bit: -2,
	signed_integer_32bit: -3,
	signed_integer_64bit: -4,
	signed_integer_128bit: -5,
	float_32bit: null,
	float_64bit: 2.0,
	float_128bit: 3.0,
	boolean_type: true,
	character_type: 'a',
	string_type: "string",
	array_type: {},
	map_type: {},
	structure_type: {}
};

// Data Structure Initialized Declaration
// Syntax - struct Name {fields};
struct DataStructure {
	byte_type: byte = null;
	unsigned_integer_size: usize = 0;
	unsigned_integer_8bit: uint8 = 1;
	unsigned_integer_16bit: uint16 = 2;
	unsigned_integer_32bit: uint32 = 3;
	unsigned_integer_64bit: uint64 = 4;
	unsigned_integer_128bit: uint128 = 5;
	signed_integer_size: isize = null;
	signed_integer_8bit: int8 = -1;
	signed_integer_16bit: int16 = -2;
	signed_integer_32bit: int32 = -3;
	signed_integer_64bit: int64 = -4;
	signed_integer_128bit: int128 = -5;
	float_32bit: float32 = null;
	float_64bit: float64 = 2.0;
	float_128bit: float128 = 3.0;
	boolean_type: bool = true;
	character_type: char = 'a';
	string_type: str = "string";
	array_type: [5]uint8 = {};
	map_type: map<uint8, str> = {};
	structure_type: DataStructure = {};
};

// Variable Declaration
// Syntax - var name: type;

// Boolean Initialization
// Syntax - var name: type = value;
// OR
// Null Syntax - var name: type = null;
var boolean_type: bool = true;

// Byte Initialization
// Syntax - var name: type = value;
// OR
// Null Syntax - var name: type = null;
// Encoding Dependent: ASCII, Binary, UTF-8, UTF-16, UTF-32
var byte_type: byte = 'a';

// Character Initialization
// Syntax - var name: type = value;
// OR
// Null Syntax - var name: type = null;
// Encoding Dependent: ASCII, UTF-8, UTF-16, UTF-32
var character_type: char = 'a';

// Float Initialization
// Syntax - var name: type = value;
// OR
// Null Syntax - var name: type = null;
var float_32bit: float32 = 1.0;

// Integer Initialization
// Syntax - var name: type = value;
// OR
// Null Syntax - var name: type = null;
var unsigned_integer_8bit: uint8 = 1;

// Platform Dependent Integer Size Initialization
// Syntax - var name: type = value;
// OR
// Null Syntax - var name: type = null;
// Platform Dependent: x86, x86_64, AARCH32, AARCH64, RISC32, RISC64
var signed_integer_size: isize = -1;

// String Initialization
// Syntax - var name: type = value;
// OR
// Null Syntax - var name: type = null;
// Encoding Dependent: ASCII, UTF-8, UTF-16, UTF-32
var string_type: str = "string";

// Array Initialization
// Syntax - var name: [length]type = {values};
// OR
// Multi-Dimensional Syntax - var name: [rows][columns]type = {values};
// OR
// Unknown Size Syntax - var name: []type = {values};
// OR
// Null Syntax - var name: [length]type = {null};
var array_type: [5]uint8 = {
	1,
	2,
	3,
	4,
	5
};

// Hash Map Initialization
// Syntax - var name: type<type, type> = {(key:value)};
// OR
// Null Syntax - var name: type<type, type> = {(null:null)};
var map_type: map<uint8, str> = {
	(1:"string"),
	(2:"string"),
	(3:"string"),
	(4:"string"),
	(5:"string")
};
```

