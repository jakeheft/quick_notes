# Ruby Methods

## String
### String methods, unless otherwise stated, do not alter the original string if it is a variable
- **str#capitalize**: capitalizes 1st character of string, downcases the rest
   ```ruby
   "heLLo".capitalize => "Hello"
   ```
- **str#upcase**: changes all letters to uppercase
   ```ruby
   "heLLo".upcase => "HELLO"
   ```
- **str#downcase**: changes all letters to lowercase
```ruby
"heLLo".downcase => "hello"
```
- **str#reverse**: reverses all characters in string
```ruby
"heLLo".reverse => "oLLeh"
```
- **str#sub**: substitutes given part of the string for another, returns altered string, but does not update if variable. Only applies to first occurrence.
```ruby
string = "here is my string"
string.sub("e", "eee") => "heeere is my string"
string => "here is my string"
```
- **str#gsub**: same as #sub, however will replace _all_ occurrences. You can also use this to change or remove multiple characters (in no particular order, see ex2 below)
```ruby
string = "here is my string"
string.gsub("e", "eee") => "heeereee is my string"
string => "here is my string"
#ex2
string.gsub(/[aeiou]/, "x") => "hxrx xs my strxng"
string.gsub(/[aeiou]/, "") => "hr s my strng"
```
- **str#chop**: removes last character of string and return the string w/o letter
```ruby
"heLLo".chop => "heLL"
```
- **str#chomp**: removes trailing newlines from strings. Can also remove given separator if provided, if and only if that separator exists at the end of the string.
```ruby
string = "Here is my string\n"
string.chomp => "Here is my string"
string = "Another string"
string.chomp("ring") => "Another st"
```
- **str#length**: returns length of string
```ruby
"hello".length => 5
```
- **str#count**: counts the number of characters passed through as parameters; the parameters do not have to be in any order
```ruby
string = "let's count the number of 'n' in this string"
string.count("n") => 5
string = "now let's count all of the vowels, including 'y'"
string.count("aeiouy") => 13
```
- **str#include?**: checks to see if a string includes whatever is put through in the parameters, returns true or false
```ruby
string = "check out this string"
string.include?("check") => true
string.include?("dog") => false
```
- **str#concat**: adds parameters onto end of string
```ruby
"hello".concat(" world") => "hello world"
```
- **str#<<**: (shovel operator), same as #concat
```ruby
greeting = "Hello "
name = "Jake"
greeting << name => "Hello Jake"
```
- **str#strip**: removes leading and trailing whitespace (spaces & \n characters)
```ruby
string = "    this doesn't look quite right...          "
string.strip => "this doesn't look quite right..."
```

## Integer  
- **int#even?** & **int#odd?**: checks to see if number is even or odd and returns true/false  
```ruby
5.even? => false
5.odd? => true
num = 8984
num.even? => true
```

## Float
- **float#round**: rounds to nearest whole number. Can also put int in parameters to round to certain decimal
```ruby
3.14159.round => 3
3.14159.round(3) => 3.142
```
- **float#ceil**: rounds up to next highest whole number
```ruby
3.14.ceil => 4
52.000001.ceil => 53
```

## Array
```ruby
name_array = ["Jake", "Erica", "Brian", "Megan"]
str_array = ["This is a sentence.", "Here is another.", "What are these for?"]
num_array = [1, 2, 3, 4, 5]
```
- **array#shift**: removes 1st element of array returns it  
   ```ruby
   name_array.shift => "Jake"  
   name_array => ["Erica", "Brian", "Megan"]
   ```
- **array#**


## Hash
