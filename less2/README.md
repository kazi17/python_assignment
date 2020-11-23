# python_assignment02

#T6Q1
#A list behaves like a container, and it is able to contain more than one value. Create a list with the
#values as shown in the example below.

aList = ['Hello',0,20.0,'World']

#T6Q2
#A list can be modified, and more elements can be added to an existing list. Use the append(x) function
#to add some more items to the list to produce the same content shown in the sample below.

aList = ['Hello', 0] 

aList.append(20.0)
aList.append('World')

#T6Q3
#A list can be modified, and elements can be removed from an existing list. Use the remove(x) function
#to remove some items from the list shown in the sample given below so that the list is left with the
#following content: ['hello', 'python','programming'].


aList = ['hello', 'i', 'love', 'python', 'programming'] 

aList.remove('i')
aList.remove('love')

#T6Q4
#Write a function addNumbersInList(numbers) to add all the numbers in a list. To access each element in
#a list, you can use the statement 'for num in numbers:'.

def addNumbersInList(numbers):
    return sum(i for i in numbers)

#T6Q5
#Write a function addOddNumbers(numbers) to add all the odd numbers in a list. To access each element in
#a list, you can use the statement 'for num in numbers:'. 

return sum(i for i in numbers if i%2 ==1)

#T6Q6
#Write a function countOddNumbers(numbers) to count the number of odd numbers in a list.

s=0
	for num in numbers:
		if num%2==1:
			s+=1
	return s

#T6Q7
#Write a function getEvenNumbers(numbers) to return all the even numbers in a list. 

def getEvenNumbers(numbers):
	s=[]
	for num in numbers:
		if num%2==0:
			s.append(num)
	return s
		

#T6Q8
#Write a function removeFirstAndLast(list) that takes in a list as an argument and remove the first and last
#elements from the list. The function will return a list with the remaining items. 



#T6Q9
#Write a function getMaxNumber(numbers) that returns the maximum number in a list. 
def getMaxNumber(numbers):
	if(numbers == []):
        	return "N.A"
        a = list(numbers)
        return max(a)

#T6Q10
#Write a function getMinNumber(numbers) that returns the minimum number in a list. 

def getMinNumber(numbers):
	if(numbers == []):
        	return "N.A"
        s=list(numbers)
        return min(s)

#T6Q11
#Write a function that does matrix multiplication.
#The product of a mxn matrix with a nxp matrix results in a mxp matrix.
#A mxn matrix, with m rows and n columns, can be represented using nested lists.
#Am,n = [ [x11, x12, ..., x1n], ..., [xm1, ..., xmn] ] 



#T6Q13
#A mxn matrix, m rows and n columns, can be represented using
#nested lists. Write a function that returns the diminensions of a matrix. 


#T6Q16
#Write a function combine(la, lb) that takes in two lists and return
#a list with the contents of both list sorted in ascending order.

def combine(la, lb): 
	c=(la+lb)
	return sorted(c)
  
#T6Q17
#The transpose of a matrix M, denoted MT, is formed by interchanging
#the rows and columns of M. That is, a mxn matrix is transformed into
#a nxm matrix.[MT]ij = [M]ji. Write a function that returns the
#transpose of a matrix. 

def transpose(matrix): 
	 return map(list, zip(*matrix))
    
#T6Q19
#Write a function calCumulativeSum(numbers) that takes in a list of
#numbers as argument and returns the cumulative sum of the list. That
#is, the new list where the i element is the sum of the first i + 1
#elements from the original list. For example, the cumulative sum of
#[1, 2, 3] is [1, 3, 6]. 



#T6Q20
#Write a function combineList(list1, list2) that takes in two lists
#as arguments and return a list that combines all the elements in
#the two list. 

def combineList(list1, list2):
	return (list1+list2)
  
#T6Q21
#Write a function (list1, list2) that takes in two lists as arguments
#and return a list that is the result of removing elements from list1
#that can be found in list2. 

def subtractList(list1, list2):
	new_list = [num for num in list1 if num not in list2]
	return new_list
  
#T6Q22
#Write a function countLetters(word) that takes in a word as argument
#and returns a list that counts the number of times each letter appears.
#The letters must be sorted in alphabetical order. 

##def countLetters(word):
##    from collections import Counter
##    return Counter(word)



#T6Q23
#Write a function getNumbers(number) that takes in a number as argument
#and return a list of numbers as shown in the samples given below
#>>> getNumbers(10)
#    [100, 64, 36, 16, 4, 0, 4, 16, 36, 64, 100]


#T6Q24
#Write a function getSumOfFirstDigit(numList) that takes in a list of
#positive numbers and returns the sum of all the first digit in the list. 



#T6Q26
#List comprehension offers a concise way to derive a new list from an




Topic 7: Question 1
Write the function countA(word) that takes in a word as argument and returns the number of 'a' in that word.

def countA(word):
	return word.count('a')
  
 Topic 7: Question 2
Write the function countLetter(word, letter) that takes in a word and a letter as arguments and returns the number of occurrence of that letter in the word.

def countLetter(word, letter):
	return word.count(letter)
  
 Topic 7: Question 3
Write a function removeLetter(word, letter) that takes in a word and a letter as arguments and remove all the occurrence of that particular letter from the word. The function will returns the remaining leters in the word.

def removeLetter(word, letter):
	return word.replace(letter,'')
  
 Topic 7: Question 4
Write the function changeCase(word) that changes the case of all the letters in a word and returns the new word.

def changeCase(word):
    result = ""
    for letter in word:
        if letter == letter.upper():
            result += letter.lower()
        else:
            result += letter.upper()
    return result
	
 Topic 7: Question 5
Write the function search(word, substring) that takes in a word and a substring as arguments and returns the position (0 indexed) of the substring if it is found in the word. The function returns -1 if the substring is not found.

def search(word, substring):
	if substring in word:
		return len(substring)
	return -1
  
 Topic 7: Question 6
A string contains a sequence of characters. Elements within a string can be accessed using index that starts from 0. Write the function getChar(word, pos) that takes in a word and a number as argument and returns the character at that position.

Topic 7: Question 7
Write a function countVowels(word) that takes in a word as an argument and returns the number of vowels ('a', 'e', 'i', 'o', 'u') in the word.

def countVowels(word):
	counter=0
	for i in word:
		if i in ('a', 'e', 'i', 'o', 'u'):
			counter+=1
	return(counter)
	
  
  Topic 7: Question 8
Write the function getVowels(word) that takes in a word as an argument and returns the vowels ('a', 'e', 'i', 'o', 'u') in that word.

def getVowels(word):
	array=[]
	for i in word:
		if i in ('a','e','i','o','u','A','E','I','O','U'):
			array.append(i)
	return(array)
  
 Topic 7: Question 9
Write the function capitalizeVowels(word) that returns the word with all the vowels capitalized.

Topic 7: Question 10
Write the function startEndVowels(word) that returns True if the word starts and ends with vowels.
def startEndVowels(word):
	vowels = tuple("aeiouAEIOU")
	return word.startswith(vowels) and word.endswith(vowels) 
  
  Topic 7: Question 11
Write the function removeVowels(word) that removes all the vowels ('a', 'e', 'i', 'o', 'u') in a word and returns the remaining letters in the word.

def removeVowels(word):  
	for i in "aeiouAEIOU":
		word = word.replace(i,"")
	return word
  
  Topic 7: Question 12
Write the function reverseWord(word) that returns the word in the reverse order.

Topic 7: Question 13
Write the function isReverse(word1, word2) that takes two words as arguments and returns True is the second word is the reverse of the first word.



Topic 7: Question 14
Write the function startWithVowel(word) that takes in a word as argument and returns a substring that starts with the first vowel found in the word. The function returns 'No vowel' if the word does not contain vowel.

def startWithVowel(word):
	if word[0] in 'aeiou':
		return word

	else:
		for i in range(1,len(word)):
			if word[i] in 'aeiou':
				return word[i:]
	return "No vowel"


Topic 7: Question 15
Write the function getCommonLetters(word1, word2) that takes in two words as arguments and returns a new string that contains letters found in both string. Ignore repeated letters and sort the result in alphabetical order.

Topic 7: Question 16
Write a function mirrorText(word1, word2) that takes in 2 words as arguments and returns a new word in the following order: word1word2word2word1.

def mirrorText(word1,word2):
	return (word1+word2+word2+word1)
  
  Topic 7: Question 17
Write a function echoWord(word) that takes in a word as arguments and returns a word that repeats itself based on the number of letter in the word.

def echoWord(word):
	for i in word:
		return (len(word)*word)
  
  
  Topic 7: Question 18
Write a function rightJustify(word) that takes in a word as argument and return a word with leading spaces so that the last letter of the word is in column 50 of the display.

Topic 7: Question 19
A palindrome is a word, phrase, number or other sequence of units that can be read the same way in either direction. Write a function that determines whether the given word or number is a palindrome.

Topic 7: Question 20
Write a function isInAlphabeticalOrder(word) that takes in a word as argument and returns True if the word contains letters that are arranged in alphabetical order. For example, the letter 'c' should not appear before the letter 'a'.

def isInAlphabeticalOrder(word):
    for i in range(len(word)-1):
        if word[i] > word[i + 1]:
            return False
    return True
    
    
Topic 7: Question 21
Write a function isAllLettersUsed(word, required) that takes in a word as the first argument and returns True if the word contains all the letters found in the second argument.

def isAllLettersUsed(word, required):
	for i in word:
		if i in required:
			return True
		else:
			return False
      
 Topic 7: Question 22
Write a function isTripleDouble(word) that takes in a word as argument and returns True if the word contains three consecutive double letters.

23	Split Word	Write a function splitWord(word, numOfChar) that takes in a word and a number as arguments. The function will split the word into smaller segments with each segment containing the number of letter specified in the numOfChar argument. These segments are stored and returned in a list.


24	Anagram	An anagram is a word formed by reordering the letters of another word. Write a function isAnagram(w1, w2) that takes in two words as arguments and return True if one word is an anagram of the other word.






#T8Q1
# Initialize dictionary "contactinfo" with the values 
# as shown in above examples. Hint: The key is a string 
# literal while the value is a dictionary type.
contactinfo ={}

contactinfo["Tom"]={'Email':'tom@gmail.com', 'Phone':61234567}
contactinfo["Sally"]={'Email':'sally@hotmail.com', 'Phone':67654321}

#T8Q5
#In gene expression, mRNA is transcribed from a DNA template. The 4
#nucleotide bases of A, T, C, G corresponds to the U, A, G, C bases
#of the mRNA. Write a function that returns the mRNA transcript given
#the sequence of a DNA strand.
#Use a dictionary to provide the mapping of DNA to RNA bases.
def mRNAtranscription(dna_template):

 dna2rna = {'A':'U','T':'A','C':'G','G':'C' }
    mRNA = ''
    for base in dna_template:  
    	mRNA+=dna2rna.get(base)  


    return mRNA

#T8Q6
#A DNA strand consisting of the 4 nucleotide bases is usually represented
#with a string of letters: A,T, C, G. Write a function that computes the base
#composition of a given DNA sequence. 

counts={'A':0,'C':0,'T':0,'G':0}
	for letter in dna_seq:
		if  letter in counts:
			counts[letter]+=1
	return counts

#T8Q7
#Write a function countLetters(word) that takes in a word as argument and
#returns a dictionary that counts the number of times each letter appears. 

def countLetters(word): 
    result = { }
    letters = ""
    for i in word:
        if i not in letters:
            letters += i
            result[i] = 0
    for i in word:
        if i in letters:
            result[i] += 1
    return result


#T8Q8
#Write a function reverseLookup(dictionary, value) that takes in a dictionary
#and a value as arguments and returns a sorted list of all keys that contains
#the value. The function will return an empty list if no match is found.

def reverseLookup(dictionary, value):
	result=[]
	for i in dictionary:
		if dictionary[i]==value:
			result.append(i)
	return sorted(result)

#T8Q9
#Write a function invertDictionary(d) that takes in a dictionary as argument
#and return a dictionary that inverts the keys and the values of the original
#dictionary. 



#T8Q10
#A sparse vector is a vector whose entries are almost all zero, like
#[1, 0, 0, 0, 0, 0, 0, 2, 0]. Storing all those zeros wastes memory and
#dictionaries are commonly used to keep track of just the nonzero entries.
#For example, the vector shown earlier can be represented as {0:1, 7:2}, since
#the vector it is meant to represent has the value 1 at index 0 and the value
#2 at index 7. Write a function that converts a sparse vector into a dictionary
#as described above. 

#T8Q11
#A sparse vector is a vector whose entries are almost all zero, like
#[1, 0, 0, 0, 0, 0, 0, 2, 0]. Storing all those zeros wastes memory and dictionaries
#are commonly used to keep track of just the nonzero entries. For example, the vector
#shown earlier can be represented as {0:1, 7:2}, since the vector it is meant to represent
#has the value 1 at index 0 and the value 2 at index 7. Write a function that converts a
#dictionary back to its sparese vector representation. 


  
#T9Q3
#The determinant of a 2x2 matrix is the product of the elements on the main
#diagonal minus the product of the elements off the main diagonal. 

def det(M):
	a=M[0][0]
	b=M[0][1]
	c=M[1][0]
	d=M[1][1]
	return((a*d)-(b*c))
    
#T9Q4
#Write a function hasSameContent(t1, t2) that takes in two tuples as arguments
#and return True if both tuples contain the same items. 

def hasSameContent(t1, t2):
    if(len(t1) != len(t2)):
        return False
    if sorted(t1)==sorted(t2):
    	return True
    else:
    	return False

#T9Q5
#Write a function sumNumbers(*args) that takes in a variable-length argument
#list of numbers and returns the sum of the numbers. 

def sumNumbers(*args):
    a = args
    return sum(a)

#T9Q6
#Write a function commonElements(t1, t2) that takes in 2 tuples as arguments
#and returns a sorted tuple containing elements that are found in both tuples. 

def commonElements(first, second):
    return tuple((sorted(set(first) & set(second))))

#T9Q7
#Write a function removeCommonElements(t1, t2) that takes in 2 tuples as
#arguments and returns a sorted tuple containing elements that are not found
#in both tuples. 

def removeCommonElements(first,second):
    return tuple((sorted(set(first) ^ set(second))))

#T9Q8
#Write a function shiftByTwo(*args) that takes in variable-length argument
#and returns a tuple with its elements shifted to the right by two indices.

#T9Q9
#Write a function sortByIndex(aList) that takes in a list of tuple in the
#following format: (index, value) and returns a new tuple with its elements
#sorted based on the index. 


#T9Q10
#Write a function sortByLength(t, order) that takes in a tuple of string and
#returns a new tuple with its elements sorted by the length of the string. The
#order of sorting is based on the value of the second argument: 'asc' or 'des'. 




#existing list or sequence. Given a list of numbers, write a function
#that returns the numbers that are greater than the average. 






