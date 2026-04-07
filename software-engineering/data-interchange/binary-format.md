# Binary Format

- Binary Source File: .binary
- .binary Files Must be Statically Typed
- .binary Files Cannot be Dynamically Typed
- .binary Files are Required
- // This is a Comment

## Numeral Systems

- Unary: Base 1
- Binary: Base 2
- Trinary: Base 3
- Quaternary: Base 4
- Quinary: Base 5
- Heximal: Base 6
- Septenary: Base 7
- Octal: Base 8
- Nonal: Base 9
- Decimal: Base 10
- Hexadecimal: Base 16
- Duotrigesimal: Base 32
- Quadrahexagesimal: Base 64

## Numeral Format Prefixes

- Binary Prefixes: #, %
- Trinary Prefixes: 0t, \t, #t, %t
- Quaternary Prefixes: 0qt, \qt, #qt, %qt
- Quinary Prefixes: 0q, \q, #q, %q
- Heximal Prefixes: 0s, \s, #s, %s
- Septenary Prefixes: 0st, \st, #st, %st
- Octal Prefixes: 0o, \o, #o, %o
- Nonal Prefixes: 0nn, \nn, #nn, %nn
- Decimal Prefixes: 0d, \d, #d, %d
- Hexadecimal Prefixes: 0x, \x, #x, %x
- Duotrigesimal Prefixes: 0dt, \dt, #dt, %dt
- Quadrahexagesimal Prefixes: 0qx, \qx, #qx, %qx

## ASCII Characters

### Control Codes: 1967

| Binary   | Octal | Decimal | Hexadecimal | Abbreviation | Unicode | Caret | C Escape | Name                           | Size   |
| -------- | ------| ------- | ----------- | ------------ | ------- | ----- | -------- | ------------------------------ | ------ |
| 000 0000 | 	000  |	0      | 00          |	NUL         | 	␀     |	^@    |	\0       |  Null                          | 1 Byte |
| 000 0001 | 	001  |	1      | 01          |	SOH         | 	␁     |	^A    |		       |  Start of Heading              | 1 Byte |
| 000 0010 | 	002  |	2      | 02          |	STX         | 	␂     |	^B    |		       |  Start of Text                 | 1 Byte |
| 000 0011 | 	003  |	3      | 03          |	ETX         | 	␃     |	^C    |		       |  End of Text                   | 1 Byte |
| 000 0100 | 	004  |	4      | 04          |	EOT         | 	␄     |	^D    |		       |  End of Transmission           | 1 Byte |
| 000 0101 | 	005  |	5      | 05          |	ENQ         | 	␅     |	^E    |		       |  Enquiry                       | 1 Byte |
| 000 0110 | 	006  |	6      | 06          |	ACK         | 	␆     |	^F    |		       |  Acknowledgement               | 1 Byte |
| 000 0111 | 	007  |	7      | 07          |	BEL         | 	␇     |	^G    |	\a 	     |  Bell (Alert)                  | 1 Byte |
| 000 1000 | 	010  |	8      | 08          |	BS          | 	␈     |	^H    |	\b 	     |  Backspace                     | 1 Byte |
| 000 1001 | 	011  |	9      | 09          |	HT          | 	␉     |	^I    |	\t 	     |  Horizontal Tab                | 1 Byte |
| 000 1010 | 	012  |	10     | 0A          | 	LF          | 	␊     |	^J    |	\n 	     |  Line Feed                     | 1 Byte |
| 000 1011 | 	013  |	11     | 0B          | 	VT          | 	␋     |	^K    |	\v 	     |  Vertical Tab                  | 1 Byte |
| 000 1100 | 	014  |	12     | 0C          | 	FF          | 	␌     |	^L    |	\f 	     |  Form Feed                     | 1 Byte |
| 000 1101 | 	015  |	13     | 0D          | 	CR          | 	␍     |	^M    |	\r 	     |  Carriage Return               | 1 Byte |
| 000 1110 | 	016  |	14     | 0E          | 	SO          | 	␎     |	^N    |		       |  Shift Out                     | 1 Byte |
| 000 1111 | 	017  |	15     | 0F          | 	SI          | 	␏     |	^O    |		       |  Shift In                      | 1 Byte |
| 001 0000 | 	020  |	16     | 10          | 	DLE         | 	␐     |	^P    |		       |  Data Link Escape              | 1 Byte |
| 001 0001 | 	021  |	17     | 11          | 	DC1         | 	␑     |	^Q    |		       |  Device Control 1 (often XON)  | 1 Byte |
| 001 0010 | 	022  |	18     | 12          | 	DC2         | 	␒     |	^R    |		       |  Device Control 2              | 1 Byte |
| 001 0011 | 	023  |	19     | 13          | 	DC3         | 	␓     |	^S    |		       |  Device Control 3 (often XOFF) | 1 Byte |
| 001 0100 | 	024  |	20     | 14          | 	DC4         | 	␔     |	^T    |		       |  Device Control 4              | 1 Byte |
| 001 0101 | 	025  |	21     | 15          | 	NAK         | 	␕     |	^U    |		       |  Negative Acknowledgement      | 1 Byte |
| 001 0110 | 	026  |	22     | 16          | 	SYN         | 	␖     |	^V    |		       |  Synchronous Idle              | 1 Byte |
| 001 0111 | 	027  |	23     | 17          | 	ETB         | 	␗     |	^W    |		       |  End of Transmission Block     | 1 Byte |
| 001 1000 | 	030  |	24     | 18          | 	CAN         | 	␘     |	^X    |		       |  Cancel                        | 1 Byte |
| 001 1001 | 	031  |	25     | 19          | 	EM          |	  ␙     |	^Y    |		       |  End of Medium                 | 1 Byte |
| 001 1010 | 	032  |	26     | 1A          | 	SUB         | 	␚     | ^Z    |		       |  Substitute                    | 1 Byte |
| 001 1011 | 	033  |	27     | 1B          | 	ESC         |	  ␛ 	  | ^[    |	\e       |  Escape                        | 1 Byte |
| 001 1100 | 	034  |	28     | 1C          | 	FS          |	  ␜ 	  | ^\    |		       |  File Separator                | 1 Byte |
| 001 1101 | 	035  |	29     | 1D          | 	GS          |	  ␝ 	  | ^]    |		       |  Group Separator               | 1 Byte |
| 001 1110 | 	036  |	30     | 1E          | 	RS          |	  ␞ 	  | ^^    |          |  Record Separator              | 1 Byte |
| 001 1111 | 	037  |	31     | 1F          | 	US          |	  ␟ 	  | ^_    |		       |  Unit Separator                | 1 Byte |
| 111 1111 | 	177  |	127    | 7F          | 	DEL         | 	␡     | ^?    |		       |  Delete                        | 1 Byte |

### Printable Characters: 1967

| Binary   | Octal | Decimal | Hexadecimal | Glyph | Size   | 
| -------- | ------| ------- | ----------- | ----- | ------ |
| 010 0000 | 	040 | 32       |	20         |       | 1 Byte |
| 010 0001 | 	041 | 33       |	21         |	!    | 1 Byte |
| 010 0010 | 	042 | 34       |	22         |	"    | 1 Byte |
| 010 0011 | 	043 | 35       |	23         |	#    | 1 Byte |
| 010 0100 | 	044 | 36       |	24         |	$    | 1 Byte |
| 010 0101 | 	045 | 37       |	25         |	%    | 1 Byte |
| 010 0110 | 	046 | 38       |	26         |	&    | 1 Byte |
| 010 0111 | 	047 | 39       |	27         |	'    | 1 Byte |
| 010 1000 | 	050 | 40       |	28         |	(    | 1 Byte |
| 010 1001 | 	051 | 41       |	29         |	)    | 1 Byte |
| 010 1010 | 	052 | 42       |	2A         |	*    | 1 Byte |
| 010 1011 | 	053 | 43       |	2B         |	+    | 1 Byte |
| 010 1100 | 	054 | 44       |	2C         |	,    | 1 Byte |
| 010 1101 | 	055 | 45       |	2D         |	-    | 1 Byte |
| 010 1110 | 	056 | 46       |	2E         |	.    | 1 Byte |
| 010 1111 | 	057 | 47       |	2F         |	/    | 1 Byte |
| 011 0000 | 	060 | 48       |	30         |	0    | 1 Byte |
| 011 0001 | 	061 | 49       |	31         |	1    | 1 Byte |
| 011 0010 | 	062 | 50       |	32         |	2    | 1 Byte |
| 011 0011 | 	063 | 51       |	33         |	3    | 1 Byte |
| 011 0100 | 	064 | 52       |	34         |	4    | 1 Byte |
| 011 0101 | 	065 | 53       |	35         |	5    | 1 Byte |
| 011 0110 | 	066 | 54       |	36         |	6    | 1 Byte |
| 011 0111 | 	067 | 55       |	37         |	7    | 1 Byte |
| 011 1000 | 	070 | 56       |	38         |	8    | 1 Byte |
| 011 1001 | 	071 | 57       |	39         |	9    | 1 Byte |
| 011 1010 | 	072 | 58       |	3A         |	:    | 1 Byte |
| 011 1011 | 	073 | 59       |	3B         |	;    | 1 Byte |
| 011 1100 | 	074 | 60       |	3C         |	<    | 1 Byte |
| 011 1101 | 	075 | 61       |	3D         |	=    | 1 Byte |
| 011 1110 | 	076 | 62       |	3E         |	>    | 1 Byte |
| 011 1111 | 	077 | 63       |	3F         |	?    | 1 Byte |
| 100 0000 | 	100 | 64       |	40         |	@    | 1 Byte |
| 100 0001 | 	101 | 65       |	41         |	A    | 1 Byte |
| 100 0010 | 	102 | 66       |	42         |	B    | 1 Byte |
| 100 0011 | 	103 | 67       |	43         |	C    | 1 Byte |
| 100 0100 | 	104 | 68       |	44         |	D    | 1 Byte |
| 100 0101 | 	105 | 69       |	45         |	E    | 1 Byte |
| 100 0110 | 	106 | 70       |	46         |	F    | 1 Byte |
| 100 0111 | 	107 | 71       |	47         |	G    | 1 Byte |
| 100 1000 | 	110 | 72       |	48         |	H    | 1 Byte |
| 100 1001 | 	111 | 73       |	49         |	I    | 1 Byte |
| 100 1010 | 	112 | 74       |	4A         |	J    | 1 Byte |
| 100 1011 | 	113 | 75       |	4B         |	K    | 1 Byte |
| 100 1100 | 	114 | 76       |	4C         |	L    | 1 Byte |
| 100 1101 | 	115 | 77       |	4D         |	M    | 1 Byte |
| 100 1110 | 	116 | 78       |	4E         |	N    | 1 Byte |
| 100 1111 | 	117 | 79       |	4F         |	O    | 1 Byte |
| 101 0000 | 	120 | 80       |	50         |	P    | 1 Byte |
| 101 0001 | 	121 | 81       |	51         |	Q    | 1 Byte |
| 101 0010 | 	122 | 82       |	52         |	R    | 1 Byte |
| 101 0011 | 	123 | 83       |	53         |	S    | 1 Byte |
| 101 0100 | 	124 | 84       |	54         |	T    | 1 Byte |
| 101 0101 | 	125 | 85       |	55         |	U    | 1 Byte |
| 101 0110 | 	126 | 86       |	56         |	V    | 1 Byte |
| 101 0111 | 	127 | 87       |	57         |	W    | 1 Byte |
| 101 1000 | 	130 | 88       |	58         |	X    | 1 Byte |
| 101 1001 | 	131 | 89       |	59         |	Y    | 1 Byte |
| 101 1010 | 	132 | 90       |	5A         |	Z    | 1 Byte |
| 101 1011 | 	133 | 91       |	5B         |	[    | 1 Byte |
| 101 1100 | 	134 | 92       |	5C         |	\    | 1 Byte |
| 101 1101 | 	135 | 93       |	5D         |	]    | 1 Byte |
| 101 1110 | 	136 | 94       |	5E         |	^    | 1 Byte |
| 101 1111 | 	137 | 95       |	5F         |	_    | 1 Byte |
| 110 0000 | 	140 | 96       |	60         |	`    | 1 Byte |
| 110 0001 | 	141 | 97       |	61         |	a    | 1 Byte |
| 110 0010 | 	142 | 98       |	62         |	b    | 1 Byte |
| 110 0011 | 	143 | 99       |	63         |	c    | 1 Byte |
| 110 0100 | 	144 | 100      | 	64         | 	d    | 1 Byte |
| 110 0101 | 	145 | 101      | 	65         | 	e    | 1 Byte |
| 110 0110 | 	146 | 102      | 	66         | 	f    | 1 Byte |
| 110 0111 | 	147 | 103      | 	67         | 	g    | 1 Byte |
| 110 1000 | 	150 | 104      | 	68         | 	h    | 1 Byte |
| 110 1001 | 	151 | 105      | 	69         | 	i    | 1 Byte |
| 110 1010 | 	152 | 106      | 	6A         | 	j    | 1 Byte |
| 110 1011 | 	153 | 107      | 	6B         | 	k    | 1 Byte |
| 110 1100 | 	154 | 108      | 	6C         | 	l    | 1 Byte |
| 110 1101 | 	155 | 109      | 	6D         | 	m    | 1 Byte |
| 110 1110 | 	156 | 110      | 	6E         | 	n    | 1 Byte |
| 110 1111 | 	157 | 111      | 	6F         | 	o    | 1 Byte |
| 111 0000 | 	160 | 112      | 	70         | 	p    | 1 Byte |
| 111 0001 | 	161 | 113      | 	71         | 	q    | 1 Byte |
| 111 0010 | 	162 | 114      | 	72         | 	r    | 1 Byte |
| 111 0011 | 	163 | 115      | 	73         | 	s    | 1 Byte |
| 111 0100 | 	164 | 116      | 	74         | 	t    | 1 Byte |
| 111 0101 | 	165 | 117      | 	75         | 	u    | 1 Byte |
| 111 0110 | 	166 | 118      | 	76         | 	v    | 1 Byte |
| 111 0111 | 	167 | 119      | 	77         | 	w    | 1 Byte |
| 111 1000 | 	170 | 120      | 	78         | 	x    | 1 Byte |
| 111 1001 | 	171 | 121      | 	79         | 	y    | 1 Byte |
| 111 1010 | 	172 | 122      | 	7A         | 	z    | 1 Byte |
| 111 1011 | 	173 | 123      | 	7B         | 	{    | 1 Byte |
| 111 1100 | 	174 | 124      | 	7C         | 	|    | 1 Byte |
| 111 1101 | 	175 | 125      | 	7D         | 	}    | 1 Byte |
| 111 1110 | 	176 | 126      | 	7E         | 	~    | 1 Byte |

## Keywords and Primitive Types

### Primitive Types

| symbol   | size    | Binary | Octal | Decimal | Hexadecimal |
| -------- | ------- | ------ | ----- | ------- | ----------- |
| bool     | 4 Bytes |
| byte     | 4 Bytes |
| char     | 4 Bytes |
| float32  | 7 Bytes |
| float64  | 7 Bytes |
| float128 | 8 Bytes |
| isize    | 5 Bytes |
| int8     | 4 Bytes |
| int16    | 5 Bytes |
| int32    | 5 Bytes |
| int64    | 5 Bytes |
| int128   | 6 Bytes |
| map      | 3 Bytes |
| str      | 3 Bytes |
| usize    | 5 Bytes |
| uint8    | 5 Bytes |
| uint16   | 6 Bytes |
| uint32   | 6 Bytes |
| uint64   | 6 Bytes |
| uint128  | 7 Bytes |

### Keywords

| symbol   | size    | Binary | Octal | Decimal | Hexadecimal |
| -------- | ------- | ------ | ----- | ------- | ----------- |
| break    | 5 Bytes |
| case     | 4 Bytes |
| const    | 5 Bytes |
| continue | 8 Bytes |
| default  | 7 Bytes |
| else     | 4 Bytes |
| exlcude  | 7 Bytes |
| export   | 6 Bytes |
| false    | 5 Bytes |
| func     | 4 Bytes |
| if       | 2 Bytes |
| import   | 6 Bytes |
| include  | 7 Bytes |
| return   | 6 Bytes |
| static   | 6 Bytes |
| struct   | 6 Bytes |
| switch   | 6 Bytes |
| true     | 4 Bytes |
| var      | 3 Bytes |
| while    | 5 Bytes |
| type     | 4 Bytes |

## Binary Format Syntax

```shell

```

