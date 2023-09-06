# CS.12.01-Tutorial.1.2.9

You will implement the constructor and another method for the following WordPairList class.

public class WordPairList 
{

	private ArrayList<WordPair> allPairs;
 

	public WordPairList(String[] words) 
	{	

		// To be implemented.

	}

	public int numMatches()
	{

		// To be implemented.

	}


}

a) Write the constructor for the WordPairList class. The constructor takes an array of strings words as a parameter and initialises the instance variable allPairs to an ArrayList of WordPair objects.

A WordPair object consists of a word from the array paired with a word that appears later in the array. The allPairs list contains WordPair objects (words[i], words[j]) for every i and j, where 0 <= i < j < words.length. Each WordPair object is added exactly once to the list. 

The following examples illustrate two different WordPairList objects.

Example 1

String[] wordNums = {“one”, “two”, “three”};

WordPairList exampleOne = new WordPairList(wordNums);

After the code segment has executed, the allPairs instance variable of exampleOne will contain the following WordPair objects in some order.

(“one”, “two”), (“one”, “three”), (“two”, “three”)

Example 2

String[] phrase = {“the”, “more”, “the”, “merrier”};

WordPairList exampleTwo = new WordPairList(phrase);

After the code segment has executed, the allPairs instance variable of exampleTwo will contain the following WordPair objects in some order.

(“the”, “more”), (“the”, “the”), (“the”, “merrier”), (“more”, “the”), (“more”, “merrier”), (“the”, “merrier”)

Complete the WordPairList constructor.



This question involves reasoning about pairs of words that are represented by the following WordPair class.

public class WordPair 
{

	public WordPair(String first, String second) 
	{
		
		// To be implemented.

	}

	public String getFirst() 
	{
	
		// To be implemented.
	
	}

	public String getSecond() 
	{
	
		// To be implemented.
	
	}

}

b) Write the WordPairList method numMatches. This method returns the number of WordPair objects in allPairs for which the two strings match.

For example, the following code segment creates a WordPairList object.

String[] moreWords = {“the”, “red”, “fox”, “the”, “red”};

WordPairList exampleThree = new WordPairList(moreWords);

After the code segment has executed, the allPairs instance variable of exampleThree will contain the following WordPair objects in some order. 

(“the”, “red”), (“the”, “fox”), (“the”, “the”), (“the”, “red”), (“red”, “fox”), (“red”, “the”), (“red”, “red”), (“fox”, “the”), (“fox”, “red”), (“the”, “red”)

The call exampleThree.numMatches() should return 2.


