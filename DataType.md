=================
Mysql DataType
==================
Tine         Integr  =>Maximum Characters[4]     
Small        Integr  =>Maximum Characters[6]
Medium       Integr  =>Maximum Characters[9]
Big          Integr  =>Maximum Characters[20]
Integer      Integr  =>Maximum Characters[11] | 2147483647(maximum value )


=========================================

Date   			=>YYY-MM--DD 1000-01-01  9999-12-31
Datetime        =>YYYY-MM-DD HH:MI:SS
timestamp		=>YYYY-MM-DD HH:MI:SS
time      		=>HH:Mi:SS
Year			=>YYYY|YY

===========================================
Char 		=>Character

-store fixed value
-max charcter 255
-faster[use static memory]

VarChar 	=>variable Character

-store variable value 
-max character 65.535
slower[use Dynamic memory]


=========================================
=>Text 		=>STORE STRING

-DATE & COMPARED DEPEND ON CHARSET
-STORE LONG STRING

=>BLOB    =>binary large object

-deal & compared depend on  numeric value of the bytes
-used to store images & other files 
========================================
=>MYSQL STRING FUNCTION SYNTAX:
[01]LEFT(STRING,LENGTH)
[02]MID(STRING,POSITION,LENGTH)
[03]right(string,length)

[04] length(string)
[05]char_length(string)
[06]LCASE(STRING) => lower case(string)
[07]UCASE(STRING) => UPPER case (string)
[08]Repeat(string, number of repeats)
[09]Replace(string, from , to)
[10]reverse(string)
[11] concat(string, string, string)
[12]concat_ws(separator, string,string)
[13]insert(string , position, length, new string)
[14]trim(methods[leadind | triling | both],[remove string] from[string])
-methods optional if not written both will be used
-remove string if not written space will be removed
+lTrim
+Rtrim
[15]lpad &rpad:(string,)
==============================================
=>MYSQL NUMERIC & MATH FUNCTION
[01]ceil(number)
[02]floor(number)
[03]round(number, Decimal)
[04]Truncate(number,Decimal)
[05]pow(number,power)
[06]mod(number,modules)
===========================================
DAte & time function syntax
[1]TIME:
curtime()
current_time()
current_time

RESULT
[HH:MM:SS]
-------------
[2]DATE
CURDATE()
CURRENT_DATE()
CURRENT_DATE

RESULT:
[YYYY-MM-DD]
--------------


[3]NOW:
NOW()
CURRENT_TIMESTAMP()
CURRENT_TIMESTAMP

RESULT:
YYYY-MM--DD HH:MM:SS

--
[4]DAY:

DAYNAME(DATE)
DAY OF MONTH(DATE) ->DAY
DAY OF WEEK(DATE)
DAY OF YEAR(DATE)
==============================
comparison function syntax 
==========================
[1]IN(values) & NotIN(values)
[2]betwwen(Expr) & not between(Expr)
[3]like & not like {using for search }
 =>% (empty or collection of characters)
 => _ (only one charcter)

-------------------------------------------
=============================
comparison operator 
=================
= [equal]
 > [greater than]
 >[less than]
 >= [equal or greater than]
 <= [equal or less than]
 != or <> [not equal]

-------------------------------------
logical operator
[1] And && {condition + condition}
[2]Not ! {negative}
[3]or || {condition or condtion}
[4] Xor {one of two condition must be true}

------------------------------------------
======================
control flow function
====================
[1]if (condition, true , flase ){
	
}
[2]case & switch
 	when expression = value then 'result'
 	when expression = value then 'result'
 	when expression = value then 'result'
else:result
end;

























