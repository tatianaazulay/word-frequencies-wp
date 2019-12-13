# This is a presentation for word-frequencies java program, which 
1. asks the user to input a path to a text file
2. reads from the text file
3. captures the data into a HashMap
4. counts the appearance of each unique word in the text file
5. prints out a word frequency list in descending order sorted by number of occurrences in the following format:<br/>
 number of occurrences: word

<p>     - Punctuation marks are eliminated by applying regular expression "[^a-zA-Z']" to each word.<br>
        - Stopwords (such as the, a) are filtered out from the analysis. HashSet is used to store string values of stopwords
        as HashSet offers constant time performance for the basic operation: contains() which is used to identify stop words in the file while 
        reading it.<br>
        - Words from the text file are stored in a HashMap where the word is stored as a key and a number of occurences is stored as a value.<br>
        - Search on a HashMap is O(1), which allows to check if the next word from the file is already in a HashMap in constant time
        and if yes, increase the number of its occurences.<br>
        - Keys are not case sensitive.<br>
        - Word cloud is used as a visual technique to demostrate how often words are mentioned in the text. <br>
        - Data visualization is done with <a href="https://www.anychart.com/" target="_blank">AnyChart JavaScript charting library.</a>
    </p><br>
 
 **Sample of input file: song lyrics "Lessons" by Sohn**<br/>
![inputFile](https://user-images.githubusercontent.com/41156932/70396525-e5114a00-19d7-11ea-8ea0-879d51559089.jpg)<br/>
 **Sample of output**<br/>
![output](https://user-images.githubusercontent.com/41156932/70396554-24d83180-19d8-11ea-808d-b14a669f1b7f.jpg)

 
