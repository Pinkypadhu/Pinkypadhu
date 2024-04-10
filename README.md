An anagram of a string is another string
with the same characters in the same
frequency, in any order. For example
'abc', 'bca', 'acb', 'bac', 'cba', 'cab'are all
anagrams of the string 'abc'. Given two
arrays of strings, for every string in one
list, determine how many anagrams of it
are in the other list. Write a function that
receives dictionary and query, two string
arrays. It should return an array of
integers where each element i contains
the number of anagrams of query[i] that
Exist in dictionary.
Example
dictionary = ['hack', 'a', 'rank', 'khac', 'ackh', 'kran', 'rankhacker', 'a', 'ab', 'ba', 'stairs', 'raits']
query = ["a", "nark", "bs", "hack", "stair"]query[0] = 'a' has 2 anagrams in dictionary. 'a' and 'a'.
query[1] = 'nark' has 2 anagrams in dictionary. 'rank' and 'kran'.
query[2] = 'bs'has O anagrams in dictionary.
query[3] = 'hack' has 3 anagrams in dictionary. 'hack', 'khac' and 'ackh'.
query[4] = 'stair' has 1 anagram in dictionary: 'raits'. While the characters are the same in 'stairs', the frequency of 's'differs, so it is not an anagram. The final answer is [2, 2, 0, 3, 1].
Function Description
Complete the function stringAnagram in the editor below.
stringAnagram has the following parameters:
string dictionary[n]: an array of strings to search in
string query[q]: an array of strings to search forReturns
int[q]: an array of integers where the ith value is the answer to query[i]
Constraints
1 ≤ length(dictionary), length(query) ≤
105
1 ≤ length(dictionary[i]) ≤ 15
1 ≤ length(query[i]) ≤ 15
• Every string consists of lowercase English letters.
Input Format For Custom Testing
▼ Sample Case 0
Sample Input
STDIN
Function
dictionary [] size n
5
= 5
heater → dictionary =
['heater', 'cold', 'clod', 'reheat', 'docl']
cold
clodreheat
docl
3
← query[] size q query = = 3 ['codl', codl → 'heater', 'abcd']
heater
abcd
Sample Output
3
2
0
Explanationquery[0] = 'codl' has 3 anagrams in dictionary. 'cold', 'clod' and 'docl'.
query[1] = 'heater' has 2 anagrams in dictionary. Heater' and 'reheat.
query[2] = 'abcd' has O anagrams in dictionary.
The final answer is [3, 2, 0].
Sample Case 1
