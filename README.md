THis is just an arthematic series repos I created to teach myself version and commit
Started - Nov 1,2024

Below section until specified is used as notes of the course - Learn Python Basics from Openclasroom
Learning About Variables:
   Components of Variables - Name, Value and Types
       Name - is case sensitive and can start with letter or underscore. NOT IN NUMBERS.
            - only alphanumeric char and underscores (no other special chars).
            - suggestions : to spell it out and no shortcuts to maintain sanity :)

       Types - Numeric , Boolean, Strings
              Numeric can be both integers and float
              Boolean - T/F
              String - should be specified within quotes.
   LISTS -  uses square brackets  []  to denote a list.   
         - access elements of list , we can index,
         - each element has an index related to it depending on its position in the list.
         - get the value of the index using list[index]
         - IMP :INDICES STARTS with 0 (NOT 1)
         -To get the last element of a list, use the -1 index.

   LIST INDEX - strings can indexed, too! In fact, Python strings are really just lists of characters. Each character is given an index from zero to the length of the string.

For example, the string  language = "PYTHON" ,   language[2]  would give you T , because at index position 2 in the word "PYTHON" you find the character "T." Or, using inverse the index position, youwould use  language[-4]  to access  T .
A list of the following elements: P, Y, T, H, O, N. 
          the indices are indices: 0,1,2,3,4,5
        the inverse indices are  : -6,-5,-4,-3,-2,-1

LIST METHODS: append(),remove() ,sort(), len()
sort - alphabetically for lists of strings, and numerically for lists of numbers.

Tuples  are another Python structure that can be used to store data, although instead of brackets [], they are defined using parentheses ().

Ex - social_platforms_tuple = ("Facebook", "Instagram", "TikTok", "Twitter")
Many tuple properties are similar to those of a regular list. For example, both lists and tuples can be indexed. The main difference is that tuples are immutable (can't be modified), while lists are mutable (can be modified).

DICTIONARY:
Dictionaries are denoted by curly braces  {}  at the beginning and end. Each key-value pair has a colon  :  in between the key and value and a comma  ,  at the end. Each dictionary has to have unique keys within it.
can also create a new dictionary with just empty curly brackets  {}  or the  dict() function and add key-value pairs in after:
         conversion_rates = {}
          conversion_rates['facebook'] = 3.4
          conversion_rates['instagram'] = 1.2
          conversion_rates = dict()
         conversion_rates['facebook'] = 3.4
         conversion_rates['instagram'] = 1.2
--Access a Value in a Dictionary : To access the different values, you can use the key for any one of the key-value pairs.

   >> conversion_rates['facebook']
     3.4
---Use Common Operations With Dictionaries : Add a Key-Value Pair
Just like lists, there are many methods (or operations) built into Python that makes it easy to interact with data in dictionaries.
---Add a Key-Value Pair
To add a key-value pair to a dictionary, just add a new key to the existing dictionary. If the key already exists, setting a value will overwrite the existing key. The following code creates a dictionary called  golden_doodle_facts  and saves information about the mass and origin of the Goldendoodle dog breed. 
   golden_doodle_facts = {
    "mass": "30-35 lbs.",
    "origin": "United States"}
To add a new key-value about the scientific name of Goldendoodles, add:
    golden_doodle_facts['scientific_name'] = "Canis lupus familiaris"
 Now  golden_doodle_facts is:
golden_doodle_facts = {
    "mass": "30-35 lbs.",
    "origin": "United States",
    "scientific_name": "Canis lupus familiaris"}
--- overwrite :
            If you were to write  golden_doodle_facts[“mass”] = “100 lbs.” , that would overwrite the existing value, so that:
          >> golden_doodle_facts["mass"]
             "100 lbs"
----Delete a Key-Value Pair
To delete a key-value pair, use the  del  keyword and the key you want to delete.
  To delete the  “origin”  key-value pair from  golden_doodle_facts , type:
      >> del golden_doodle_facts[“origin”]
      >> print(golden_doodle_facts)
        { "mass": "30-35 lbs.",
         "scientific_name": "Canis lupus familiaris"}


KEYWORDS:
     Certain words are part of the Python language and can’t be used when naming variables. 
     Examples are del,if, and else. Such words are known as reserved words or keywords. 

Check for the Existence of a Specific Key
You can use the  in  keyword to check whether a specific key exists in a dictionary. To do this, specify the key you want to search for, the keyword  in  , and the name of the dictionary variable to search. The result will be a boolean indicating whether or not the key is in that dictionary. For example, if you want to search if the key “mass” exists in your  golden_doodle_facts  dictionary, type the following: 



PROGRAM FLOW:
1. 
>> "mass" in golden_doodle_facts
True
>> "breed" in golden_doodle_facts
False
