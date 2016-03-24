# symbols
extract symbols from file 

usage:

	symbols [--all] [--stdin] [--threads] [--nocase]

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
