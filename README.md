Wild cards are special characters used in where clauses	(They are used with a 'LIKE' keyword)

These characters are used for substitution of string characters

% - symbol, matches 0 or more characters

Syntax:
select * from User
where User_Language like "en%";

_ - symbol, matches any single character

Syntax:
select * from User
where User_City like "L_n_o_";

[] - symbol, matches any single character within the brackets. Its like an OR statement 
where letters has to match with either of the given letters. The string can have 0 or more characters

Syntax:
select * from User
where User_Country like '[UT]%';

- = symbol, matches any single character within a given range

Syntax:
select * from User
where User_city like '[A-L]%';

^ - symbol, matches any one(1) character not specified within the brackets

Syntax:
select * from User
where User_Country like '[^U]%'; 

In this the code is matching 
any character that is NOT specified in the bracket
