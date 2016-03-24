# symbols
extract symbols from file 

usage:
	
	symbols [--all] [--stdin] [--threads] 
		[--as-hex] [--nocase] [--help] 
			file1 file2 ... fileN

	flags:

	--all
	    count occurrences of ALL characters,
	    not just symbols

	--stdin
	    read file list from stdin

	--threads
	    run program in multithreaded manner 

	--nocase
	    treat content of files as case insensitive
	    (eg file.content.downcase!)

	--as-hex
	    output content of file as hexadecimal digits
	    rather than ascii characters

	--help
		get this help screen
	
sample output (ran on LICENSE file)
	
	oz@ozmo:~/git/symbols$ symbols --all --nocase LICENSE
	
	symbol count
	+--------+-------+------------+
	| symbol | count | percentage |
	+--------+-------+------------+
	| 0x20   | 120   | 24.6914%   |
	| o      | 31    | 6.3786%    |
	| e      | 31    | 6.3786%    |
	| t      | 30    | 6.1728%    |
	| i      | 29    | 5.9671%    |
	| n      | 24    | 4.9383%    |
	| a      | 22    | 4.5267%    |
	| c      | 21    | 4.321%     |
	| d      | 18    | 3.7037%    |
	| s      | 18    | 3.7037%    |
	| 0xa    | 13    | 2.6749%    |
	| u      | 13    | 2.6749%    |
	| r      | 13    | 2.6749%    |
	| h      | 13    | 2.6749%    |
	| m      | 10    | 2.0576%    |
	| l      | 8     | 1.6461%    |
	| y      | 8     | 1.6461%    |
	| w      | 7     | 1.4403%    |
	| f      | 7     | 1.4403%    |
	| p      | 7     | 1.4403%    |
	| b      | 6     | 1.2346%    |
	| g      | 6     | 1.2346%    |
	| v      | 5     | 1.0288%    |
	| 0      | 5     | 1.0288%    |
	| .      | 4     | 0.823%     |
	| k      | 3     | 0.6173%    |
	| 2      | 3     | 0.6173%    |
	| ,      | 3     | 0.6173%    |
	| 4      | 2     | 0.4115%    |
	| )      | 1     | 0.2058%    |
	| @      | 1     | 0.2058%    |
	| <      | 1     | 0.2058%    |
	| >      | 1     | 0.2058%    |
	| (      | 1     | 0.2058%    |
	| j      | 1     | 0.2058%    |
	+--------+-------+------------+
	--------------------------------------------------
	total characters: 486
	total symbols: 10
	--------------------------------------------------
	48.6 characters/symbol
	0.02 symbols/character
	symbol percentage: 2.5%

	-------------------------------------------------------------

	oz@ozmo:~/git/symbols$ symbols --all --nocase --as-hex LICENSE
	
	symbol count
	+--------+-------+------------+
	| symbol | count | percentage |
	+--------+-------+------------+
	| 0x20   | 120   | 24.6914%   |
	| 0x6F   | 31    | 6.3786%    |
	| 0x65   | 31    | 6.3786%    |
	| 0x74   | 30    | 6.1728%    |
	| 0x69   | 29    | 5.9671%    |
	| 0x6E   | 24    | 4.9383%    |
	| 0x61   | 22    | 4.5267%    |
	| 0x63   | 21    | 4.321%     |
	| 0x64   | 18    | 3.7037%    |
	| 0x73   | 18    | 3.7037%    |
	| 0x A   | 13    | 2.6749%    |
	| 0x75   | 13    | 2.6749%    |
	| 0x72   | 13    | 2.6749%    |
	| 0x68   | 13    | 2.6749%    |
	| 0x6D   | 10    | 2.0576%    |
	| 0x6C   | 8     | 1.6461%    |
	| 0x79   | 8     | 1.6461%    |
	| 0x77   | 7     | 1.4403%    |
	| 0x66   | 7     | 1.4403%    |
	| 0x70   | 7     | 1.4403%    |
	| 0x62   | 6     | 1.2346%    |
	| 0x67   | 6     | 1.2346%    |
	| 0x76   | 5     | 1.0288%    |
	| 0x30   | 5     | 1.0288%    |
	| 0x2E   | 4     | 0.823%     |
	| 0x6B   | 3     | 0.6173%    |
	| 0x32   | 3     | 0.6173%    |
	| 0x2C   | 3     | 0.6173%    |
	| 0x34   | 2     | 0.4115%    |
	| 0x29   | 1     | 0.2058%    |
	| 0x40   | 1     | 0.2058%    |
	| 0x3C   | 1     | 0.2058%    |
	| 0x3E   | 1     | 0.2058%    |
	| 0x28   | 1     | 0.2058%    |
	| 0x6A   | 1     | 0.2058%    |
	+--------+-------+------------+
	--------------------------------------------------
	total characters: 486
	total symbols: 10
	--------------------------------------------------
	48.6 characters/symbol
	0.02 symbols/character
	symbol percentage: 2.5%
