# 100 Days Of Code - Log

### Day 0: August 17, 2019

**Today's Progress**: Committed to the 100 Days of Code and decided to use the challenge to work through Zed Shaw's Learn Python The Hard Way.

**Thoughts:** First day and already procrastinating! Was supposed to start on exercises but put it off.

### Day 1: August 18, 2019

**Today's Progress**: Completed exercise 15 of Learn Python the Hard Way, with today's topic being on reading files. Had to read through and look up a number of functions and study drills required me to do proper commenting of the code, and play around with the code.

**Thoughts**: I did not expect to take so much time on today's exercise, since it was a new topic with a fair bit of study drills to work through, that much was expected.

**Link(s) to work**: [Tweet](https://twitter.com/HeyMadifz/status/1162918920459702272?s=20)

-----------------------------

### Day 1: Feb 3, 2020 (attempt 2 at 100 Days of code)

Actually restarted much earlier than today but decided to commit to this log to push myself to code everyday. Currently taking the Complete Machine Learning and Data Science: Zero to Mastery Udemy course by Andrei Neagoie and Daniel Bourke. Have completed sections 1 - 4 and currently on the learn python path (which I have completed lessons 211 - 247. Today I completed lessons 248 - 253 and learnt about list unpacking, none and dictionaries.

#type conversion exercise

```
import datetime

today = str(datetime.date.today())
current_year = int(today[:4])
birth_year = input('what year were you born?')
age = current_year - int(birth_year)
print(f'Are you going to be {age} this year?')

#password checker exercise


username = input('Username:')
password = input('Password:')

password_length = len(password)
hidden_password = '*' * password_length

print(f'{username}, your password, {hidden_password}, is {password_length} letters long')
```

Also completed exercise 24 of Learn Python the Hard Way - more practice on printing strings and functions.

```
print("Let's practice everything.")
print('You\'d need to know \'bout escapes with \\ that do:')
print('\n newlines and \t tabs.')

poem = """
\tThe lovely world
with logic so firmly planted
cannot discern \n the needs of love
nor comprehend passion from intuition
and requires an explanation
\n\t\twhere there is none.
"""

print("--------------")
print(poem)
print("--------------")
```
```
five = 10 - 2 + 3 - 6
print(f"This should be five: {five}")
```
```
def secret_formula(started):
    jelly_beans = started * 500
    jars = jelly_beans / 1000
    crates = jars / 100
    return jelly_beans, jars, crates


start_point = 10000
beans, jars, crates = secret_formula(start_point)

print("With a starting point of: {}".format(start_point))

print(f"We'd have {beans} beans, {jars} jars, and {crates} crates.")

start_point = start_point / 10

print("We can also do that this way:")
formula = secret_formula(start_point)

print("We'd have {} beans, {} jars, and {}crates".format(*formula))
```

----------------

### Day 2: Feb 4, 2020

Forgot to update progress for yesterday, day 2 was mainly practice. I reviewed the article "Python Dictionaries 101: A Detailed Visual Introduction" (https://www.freecodecamp.org/news/python-dictionaries-detailed-visual-introduction/) to go deeper on python dictionaries and wrote a frequencies dictionary as part of the article's exercise:

```
def freq_dict(data):
    freq = {}
    for elem in data:
        if elem in freq:
            freq[elem] += 1
        else:
            freq[elem] = 1
    return freq

print(freq_dict("Hello, how are you?"))

print(freq_dict([5, 2, 6, 2, 6, 5, 2, 2, 2]))
```

I also completed exercise 25 of Learn Python the Hard Way which was a practice in creating functions to break up words, sort them and print specific words.

```
def break_words(stuff):
    """This function will break up words for us."""
    words = stuff.split(' ')
    return words

def sort_words(words):
    """Sorts the words."""
    return sorted(words)

def print_first_word(words):
    """Prints the first word after popping it off."""
    word = words.pop(0)
    print(word)

def print_last_word(words):
    """Prints the last word after popping it off."""
    word = words.pop(-1)
    print(word)

def sort_sentence(sentence):
    """Takes in a full sentence and returns the sorted words."""
    words = break_words(sentence)
    return sort_words(words)

def print_first_and_last(sentence):
    """Prints the first and last words of the sentence."""
    words = break_words(sentence)
    print_first_word(words)
    print_last_word(words)

def print_first_and_last_sorted(sentence):
    """Sorts the words then prints the first and last one."""
    words = sort_sentence(sentence)
    print_first_word(words)
    print_last_word(words)
```

-----------------------------

### Day 3: Feb 4, 2020

Completed lessons 254- 259 of Complete Machine Learning and Data Science: Zero to Mastery.

-----------------------------

### Day 4 & 5: Feb 5-6, 2020 

Didn’t do much coding exercises. Completed lessons 260- 303 of Complete Machine Learning and Data Science: Zero to Mastery. 40 more lessons before I complete python core and can move on to ML part of the course.

-----------------------------

### Day 6: Feb 7, 2020
Completed lessons 304 - 311 of Complete Machine Learning and Data Science: Zero to Mastery. 32 more lessons before I complete python core and can move on to ML part of the course.

-----------------------------

### Day 7: Feb 9, 2020

Missed 1 day of #100DaysofCode because I knocked out after work. Today managed to complete an exercise creating a counter that loops over a list and adds up all the items of the list. It was a more elegant version than the solution provided in the ZTM course.

```
# Counter
my_list = [1,2,3,4,5,6,7,8,9,10]
list_total = 0
for i in my_list:
  list_total += i

print(list_total) 
```
Also completed lessons 312 - 319 of Complete Machine Learning and Data Science: Zero to Mastery. Exercise code for lesson 318 below(printing an image from a given matrice of list of lists). 24 more lessons before I complete python core and can move on to ML part of the course. 

```
#Exercise!
#Display the image below to the right hand side where the 0 is going to be ' ', and the 1 is going to be '*'. This will reveal an image!
picture = [
  [0,0,0,1,0,0,0],
  [0,0,1,1,1,0,0],
  [0,1,1,1,1,1,0],
  [1,1,1,1,1,1,1],
  [0,0,0,1,0,0,0],
  [0,0,0,1,0,0,0]
]
#iterate over picture
for image in picture:
  for pixel in image:
    if (pixel == 1):
      print('*', end = '')
    else:
      print(' ', end = '')
  print()
```

-----------------------------

### Day 8: Feb 10, 2020

Completed lessons 320 - 336 of Complete Machine Learning and Data Science: Zero to Mastery. Exercise code for lesson 320 (Find Duplicates) 325 (Tesla) below. 7 more lessons before I complete python core and can move on to ML part of the course. 

```
# Exercise: check for duplicates in list

some_list = ['a', 'b', 'c', 'b', 'd', 'm', 'n', 'n']

duplicate = []

for letter in some_list:
  if some_list.count(letter) > 1:
    if letter not in duplicate:
      duplicate.append(letter)

print(duplicate)
```

```
def checkDriverAge(age = 0):
  if int(age) < 18:
    print("Sorry, you are too young to drive this car. Powering off")
  elif int(age) > 18:
    print("Powering On. Enjoy the ride!");
  elif int(age) == 18:
    print("Congratulations on your first year of driving. Enjoy the ride!")
    
checkDriverAge(92)
```

-----------------------------


### Day 9: Feb 11, 2020

Completed lessons 336 - 343 of Complete Machine Learning and Data Science: Zero to Mastery. Exercise code for lesson 343 (List Comprehensions) below. Lesson 344 is a set to 2 quizzes on Python.

```
some_list = ['a', 'b', 'c', 'b', 'd', 'm', 'n', 'n']

duplicates = list(set([value for value in some_list if some_list.count(value) > 1]))

print(duplicates)
```
