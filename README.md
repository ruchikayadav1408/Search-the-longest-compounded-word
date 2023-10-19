# search-the-longest-compounded-word
#This Java program is designed to find the longest and second-longest compound words within a list of words stored in a file and calculate the total number of compound words. A compound word is defined as a word that can be formed by concatenating copies of shorter words found in the same list.

How to Execute the Code:

Ensure you have a Java development environment installed on your system.

Place the Java source files (LongestCompoundWord.java, Pair.java, and Trie.java) in the same directory.

Create a text file (e.g., words for problem.txt) containing a list of words, where each word is separated by whitespace.

Modify the File file = new File("words for problem.txt"); line in LongestCompoundWord.java to specify the correct path to your word list file.

Compile the Java code using javac LongestCompoundWord.java in your command prompt or terminal.

Run the compiled program using java LongestCompoundWord.

The program will read the word list, identify the longest and second-longest compound words, and display the results on the console.

#Program Overview:

The program uses a Trie data structure to efficiently store and retrieve words from the word list.
It scans the input word list file, adds words with suffixes to a queue, and inserts each word into the Trie.
It processes the words in the queue, checking if they can be concatenated with other words to form compound words.
If a compound word is found, it checks whether it's the longest or second-longest and updates the relevant variables.
The program keeps track of compound words in a HashSet to calculate the total number of compound words.
Finally, it displays the longest compound word, the second-longest compound word, and the total number of compound words on the console.
Design Decisions:

A Trie data structure was chosen to efficiently store and retrieve words and to find all suffixes of a given word.
The program uses a queue to process potential compound word candidates and update relevant variables for the longest and second-longest compound words.
It utilizes a HashSet to ensure that only unique compound words are counted for the total.

#Approach:

The program first reads and processes the word list, identifying words with suffixes that may form compound words.
It inserts each word into the Trie data structure.
It iterates through the queue of potential compound word candidates, checking for compound words by examining suffixes and Trie structure.
If a compound word is found, it is evaluated for being the longest or second-longest, and the HashSet keeps track of compound words.
The final results are displayed on the console.


#OUTPUT

![Output_1](https://github.com/ruchikayadav1408/Search-the-longest-compounded-word/assets/86114973/c625f8a7-1fc6-4f2e-9260-190cb9306469)

![Output_2](https://github.com/ruchikayadav1408/Search-the-longest-compounded-word/assets/86114973/ca1b762b-62c6-4aff-bb9f-2244619b188a)


