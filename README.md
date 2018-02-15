# Python-codingBat
# warmup 1


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

