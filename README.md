# Python-Data-Structures-Assignmente-Day-5
# ==========================================
# Python Data Structures Assignment
# ==========================================

# Types of Data Structures:
# List | Tuple | Set | Dictionary

# ==========================================
# LISTS
# ==========================================

# Create empty list
a = []

# print the value of a
print(a)

# print the type of a
print(type(a))

# Create list
languages = ['R', 'Python', 'SAS', 'Scala', 42]

# Print number of elements
print(len(languages))

# Iterate and print elements
for i in languages:
    print(i)

# Select second item
temp = languages[1]

# Print temp and type
print(temp)
print(type(temp))

# Append Java
languages.append('Java')
print(languages)

# Remove 42
languages.remove(42)
print(languages)

# Create colors list
colors = ['Red', 'Blue', 'White']

# Append Black
colors.append('Black')
print(colors)

# Insert Orange at index 1
colors.insert(1, 'Orange')
print(colors)

# Print colors
print(colors)

# Create another list
colors2 = ['Grey', 'Sky Blue']

# Extend colors
colors.extend(colors2)

# Print length and elements
print(len(colors))
print(colors)

# Sort list
colors.sort()
print(colors)

# ==========================================
# STRING OPERATIONS
# ==========================================

# Create string
sent = 'Coronavirus Caused Lockdowns Around The World'

# Split string
words = sent.split()
print(words)

# Convert to lowercase
words_lower = [word.lower() for word in words]
print(words_lower)

# Check country in list
print('country' in words_lower)

# Remove 'the'
words_lower.remove('the')
print(words_lower)

# First 4 words
x4 = words_lower[:4]

# Print x4
print(x4)

# Join list into string
joined = " ".join(words_lower)
print(joined)

# ==========================================
# SETS
# ==========================================

# Create list
stud_grades = ['A', 'A', 'B', 'C', 'C', 'F']

# Length
print(len(stud_grades))

# Convert to set
stud_grades_set = set(stud_grades)

# Print set
print(stud_grades_set)

# Types and elements
print(type(stud_grades))
print(type(stud_grades_set))

print(stud_grades)
print(stud_grades_set)

# Add G
stud_grades_set.add('G')
print(stud_grades_set)

# Add F again
stud_grades_set.add('F')
print(stud_grades_set)

# Remove F
stud_grades_set.remove('F')

# Print elements and length
print(stud_grades_set)
print(len(stud_grades_set))

# Colors and fruits
colors = ['red', 'blue', 'orange']
fruits = ['orange', 'grapes', 'apples']

# Print lists
print(colors)
print(fruits)

# Convert to sets
colors_set = set(colors)
fruits_set = set(fruits)

# Print sets
print(colors_set)
print(fruits_set)

# Union
print(colors_set.union(fruits_set))

# Intersection
print(colors_set.intersection(fruits_set))

# Difference
print(fruits_set.difference(colors_set))

# ==========================================
# TUPLES
# ==========================================

# Create temp list
temp = [17, 'Virat', 50.0]

# Iterate and print
for i in temp:
    print(i)

# Replace first element
temp[0] = 11
print(temp)

# Convert to tuple
temp1 = tuple(temp)

# Iterate tuple
for i in temp1:
    print(i)

# Tuple cannot be modified
# temp1[0] = 17   # Error

# Create city tuple
city = ("Bangalore", 28.9949521, 72)

# Print first element
print(city[0])

# Create city2
city2 = ('Chennai', 30.01, 74)

# Nested tuple
cities = (city, city2)

# Print cities
print(cities)

# Type of first element
print(type(cities[0]))

# Type of cities
print(type(cities))

# ==========================================
# DICTIONARY
# ==========================================

# Create dictionary
d = {
    "actor": "amir",
    "animal": "cat",
    "earth": 2,
    "list": [23, 32, 12]
}

# d[0] gives KeyError
# print(d[0])

# Store actor
actor = d['actor']

# Print type
print(type(actor))

# Store list
List = d['list']

# Print type
print(type(List))

# Create d1
d1 = {
    'singer': 'Kr$na',
    'album': 'Still here',
    'genre': 'hip-hop'
}

# Merge dictionaries
d.update(d1)

# Print dictionary
print(d)

# Print keys
print(d.keys())

# Print values
print(d.values())

# Iterate dictionary
for key, value in d.items():
    print(key, "---->", value)

# Character count using dictionary
char_count = {}

for char in sent:
    if char in char_count:
        char_count[char] += 1
    else:
        char_count[char] = 1

print(char_count)
