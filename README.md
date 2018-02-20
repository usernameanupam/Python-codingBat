# Python-codingBat
# warmup 1

# sleepin
The parameter weekday is True if it is a weekday, and the parameter vacation is True if we are on vacation. We sleep in if it is not a weekday or we're on vacation. Return True if we sleep in.


sleep_in(False, False) → True
sleep_in(True, False) → False
sleep_in(False, True) → True

def sleep_in(weekday, vacation):
  return (not weekday or vacation);
# ..................................................................................................................................

# monkey_trouble


We have two monkeys, a and b, and the parameters a_smile and b_smile indicate if each is smiling. We are in trouble if they are both smiling or if neither of them is smiling. Return True if we are in trouble.


monkey_trouble(True, True) → True
monkey_trouble(False, False) → True
monkey_trouble(True, False) → False

def monkey_trouble(a_smile, b_smile):
  return (b_smile == a_smile);
  
# ..................................................................................................................................

# sum_double

Given two int values, return their sum. Unless the two values are the same, then return double their sum.


sum_double(1, 2) → 3
sum_double(3, 2) → 5
sum_double(2, 2) → 8

def sum_double(a, b):
  
  sum = a + b
  
  if a == b:
    sum = sum * 2
    
  return sum
  
 # ..................................................................................................................................

# diff21

Given an int n, return the absolute difference between n and 21, except return double the absolute difference if n is over 21.


diff21(19) → 2
diff21(10) → 11
diff21(21) → 0

def diff21(n):
  if n <= 21:
    return 21 - n
  
  else:
    return (n - 21) * 2
 # ..................................................................................................................................
 
 # makes10
 
 Given 2 ints, a and b, return True if one if them is 10 or if their sum is 10.


makes10(9, 10) → True
makes10(9, 9) → False
makes10(1, 9) → True

  return (a == 10 or b == 10 or a + b == 10)

 # ..................................................................................................................................

# parrot trouble


We have a loud talking parrot. The "hour" parameter is the current hour time in the range 0..23. We are in trouble if the parrot is talking and the hour is before 7 or after 20. Return True if we are in trouble.


parrot_trouble(True, 6) → True
parrot_trouble(True, 7) → False
parrot_trouble(False, 6) → False

    return (talking and (hour < 7 or hour > 20));
 # ..................................................................................................................................

# near_hundred


Given an int n, return True if it is within 10 of 100 or 200. Note: abs(num) computes the absolute value of a number.


near_hundred(93) → True
near_hundred(90) → True
near_hundred(89) → False

 return( (abs(100 - n) <= 10) or (abs(200 - n) <= 10))
 # ..................................................................................................................................
 
 # pos_neg
 Given 2 int values, return True if one is negative and one is positive. Except if the parameter "negative" is True, then return True only if both are negative.
 
 pos_neg(1, -1, False) → True
pos_neg(-1, 1, False) → True
pos_neg(-4, -5, True) → True

def pos_neg(a, b, negative):
  if(negative):
    return (a < 0 and b < 0);
  
  return ( (a < 0 and b > 0) or (a > 0 and b < 0) );
  # ..................................................................................................................................

# not_string


Given a string, return a new string where "not " has been added to the front. However, if the string already begins with "not", return the string unchanged.


not_string('candy') → 'not candy'
not_string('x') → 'not x'
not_string('not bad') → 'not bad'

def not_string(str):
  if len(str) >= 3 and str[:3] == "not":
    return str
  return "not " + str
  # str[:3] goes from the start of the string up to but not
  # including index 3

   # ..................................................................................................................................

 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
