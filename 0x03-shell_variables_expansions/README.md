

0x03. Shell, init files, variables and expansions Project at alx.

Learning objectives is to understand the concept of variables, expansions and init files.

The task performed includes;

0.	alias ls='rm *'	---Create a script that creates an alias.

1.	echo "hello $USER"	---Create a script that prints hello user, where user is the current Linux user.

2.	PATH=$PATH:/action	---Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.

3.	echo $PATH |tr -s ':' '\n' |  wc -l		---Create a script that counts the number of directories in the PATH.

4.	printenv	---Create a script that lists environment variables.

5.	set	---Create a script that lists all local variables and environment variables, and functions

6.	BETTY="Holberton"	---Create a script that creates a new local variable.  Name: BETTY Value: Holberton

7.	export HOLBERTON="Betty"	---Create a script that creates a new global variable.  Name: HOLBERTON   Value: Betty

8.	echo $((128+TRUEKNOWLEDGE))	---prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line.

9.	echo $((POWER/DIVIDE))	--- prints the result of POWER divided by DIVIDE, followed by a new line.  POWER and DIVIDE are environment variables.

10.	echo $(( BREATH ** LOVE ))	---  displays the result of BREATH to the power LOVE. BREATH and LOVE are environment variables. The script displays the result, followed by a new line.

11.	echo $((2#$BINARY))	--- converts a number from base 2 to base 10.  The number in base 2 is stored in the environment variable BINARY.

12.	 echo {a..z}{a..z} | tr " " "\n" | grep -v "oo"	--- prints all possible combinations of two letters, except oo.  Letters are lower cases, from a to z.  One combination per line.

13.	printf "%.2f" $NUM | sort	---prints a number with two decimal places, followed by a new line.  The number will be stored in the environment variable NUM.

14.	 printf '%x\n' $DECIMAL		--- converts a number from base 10 to base 16.  The number in base 10 is stored in the environment variable DECIMAL.

15.	tr 'A-Za-z' 'N-ZA-Mn-za-m'	---encodes and decodes text using the rot13 encryption. ASCII.

16.	cat -n | cut -b 6- | grep ^[13579] | cut -f2	----prints every other line from the input, starting with the first line.

17.	echo $(printf %o $(($((5#$(echo $WATER | tr 'water' '01234'))) + $((5#$(echo $STIR | tr 'stir.' '01234'))))) | tr '01234567' 'behlnort')		---script that adds the two numbers stored in the environment variables WATER and STIR and prints the result. WATER is in base water. STIR is in base stir. The result is in base behlnort

Done…
 
