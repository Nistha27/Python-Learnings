#### PART-1
### 0.1 Python Numbers

#### **Types of numbers**
1. Integers - -1,-2,0,1,2
2. Float    - 0.1,0.8,0.5

#### **Types of Operational Operators**
1. + (addition)
2. - (subtration)
3. *(multiplication)
4. / (Division)
5. //(Floor Division)
6. % (Modulus)
7. ** (Power)
8. () (Parenthesis)

## 0.2 **Variable Assigment**
### **Rules to be noted**
1. Names cannot start with numbers
2. No special characters (only _ underscore)
3. No keywords allowed that has special meaning in python

#### **Assigngning Values**
*Syntax: *
name = object ( = as assignment operator)

#### **To determine variable type**
 *use* type()
##### **Types of variables**
1. int
2. float
3. str
4. list
5. tuple
6. dict
7. set
8. bool

## 03. Strings 
*immutable datatype*

### **Creating String**
 to create string use single quotes ('') or double quotes (" ")
 
### **Printing String**

print('Hello World' )
  Hello World
 
**Note**- 
1. \n - for new lines
2. \t - for space
		  
### **String Basics**
check length of the string

len('Hello World')

11

### **String Indexing**

Use [ ] (square brackets)
Use : (to perform Slicing)

### **String Properties**
 1. + - *concatenate strings i.e adding two strings*
 2. * -  *to create repeatition in string*
 3. .upper() - uppercase all
 4. .lower() - lowercase all
 5. .split() - split string by blank spaces (by default)
 
### **Print Formatting**

*.format() method*

Example:

1. print('This is a string {}'. format('inserted'))

     This is  a string inserted

2. print('The {} {} {} '.format('fox','brown','quick'))

     The fox brown quick 

3. print('The {2} {0} {1}'.format('fox','brown','quick'))
    
	The quick fox brown (*by using index no.*)
	
#### by float formatting method 

Example:

1. result=100/777
   
   result = 104.1235
   
   print('The result was {r}'.format(r=result))
   
   The result was 104.1235
   

## 0.4 **Lists**

#### **Creating List**

mylist = [1,22,3]

>>len(mylist)
3

#### **Indexing and Slicing**

mylist= ['one,'two','three',4,5]

>>mylist[:3]
['one','two','three']

**Note** :

+ to concatenate the list

#### Basic List Methods

1. Making a new list by addding new item 
>> mylist.append('')

2. Deleting items from list
>>mylist.pop()

**Note :** by default pop deletes off the last index object

3. Reversing the list
>>mylist.reverse()

4. Sorting
>>mylist.sort()

**Note**:
>> For alphabets it takes alphabetical order
>> For numbers it takes asending order

#### **Nesting Lists**

>>lst_1=[1,2,3]
>>lst_2=[4,5,6]

>>matrix = [lst_1,lst_2]

>>matrix
[[1,2,3],[4,5,6]]
 
## Dictionaries

>#### Creating Dictionaries

>> mydict={'key1':'value1','key2':'value2'}

##### Calling values by their key

>> mydict['key2']
   value2
   
##### Setting the object equal to itself minus 123

>> mydict['key1'] = 123
>> mydict['key1']
   123
  
##### Or by assinging direct value
>> d = {}
   d['animal'] = 42
   d['answer'] = 'Dog'

>> d
{'animal':42,'answer':'Dog']

##### Nesting with Dictionaries

>> d = {'key1':{''nesting':'dictionary'},'key2':'value'}
>> d['key1;]
   {'nesting':'dictionary'}
   
##### Dictionary Methods

**d.keys():** Grabs all keys
>> dict_keys(['key1','key2'])
**d.values():** Grabs all the values
>> dict_values([{'nesting':'dictionary'},'value'])
**d.items():** Grabs all the items 
>> dict_items([('key1',{'nesting':'dictionary'}),('key2',value)]

## Tuples
**(immutable datatype)**

#### Constructing Tuples
>>`t=(1,2,3)`
>>`len(t)`
  3 

#### Basic Tuples Methods 

##### In built functions 
1. `**t.index()**`: To enter a value and returns the index 
2. `**t.count()**`: To count the no of times a value appears

## Sets   
Set of unorderd collection of unique elements

#### Constructing Set
>> `x =set()`
>> `x.add(1)`
>> x
  {1}

>> `x.add(2)`
>>` x`
   {1,2}

##### Creating a list with repeats

>> `list1=[1,1,2,2,4,5,6,1,1`]
>> `set(list)`
  {1,2,4,5,6}

## Booleans
True or Flase
**None:** As a placeholder for an object that we dont want to reassign yet.

## Files

##### To open file 
>> `my_file = open("Test.txt")`

##### To Read
1. `my_file.read()` : reads all the lines
>> *Hello , this is a quick test file.*

2. `my_file.seek(0)` : seek to start of file (index 0)

3. `my_file.readlines()` : Returns a listof the lines in the file 
>> [Hello , this is a quick test file.*]

##### Writing to a File 
( by default open() func only allows you to read the file )

>> `my_file = open("Test.text','w+')`

*open file w or w+* --> meaning original file is detected and is written.

##### Appending to  a File 

**a:** opens a file and put the pointer at the end so it is appeneded

**w+ and a+:** lets us read and write the file if the file does not exists, one be created  