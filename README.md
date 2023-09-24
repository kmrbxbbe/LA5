MAD5234 Learning Activity 5 Student                                                           Name:- Bobby kumar                      Student Id:- C0880053
Java Code
public class StringManipulator {
public StringManipulator() {
    // Constructor (not needed for this assignment)
}
​
// Method to reverse the input string
public String reverse(String input) {
    // Ensure input is not null
    if (input == null) {
        return null;
    }
​
    StringBuilder reversed = new StringBuilder();
    for (int i = input.length() - 1; i >= 0; i--) {
        reversed.append(input.charAt(i));
    }
    return reversed.toString();
}
​
// Method to convert the input string to uppercase
public String toUpperCase(String input) {
    // Ensure input is not null
    if (input == null) {
        return null;
    }
​
    return input.toUpperCase();
}
​
// Method to concatenate two strings
public String concatenate(String str1, String str2) {
    // Ensure neither str1 nor str2 is null
    if (str1 == null || str2 == null) {
        return null;
    }
​
    return str1 + str2;
}
​
public static void main(String[] args) {
    StringManipulator sm = new StringManipulator();
​
    // Demonstrate reverse
    String word = "Hello";
    System.out.println("Original: " + word);
    System.out.println("Reversed: " + sm.reverse(word));
​
    // Demonstrate toUpperCase
    String lowerCaseWord = "hello world";
    System.out.println("\nOriginal: " + lowerCaseWord);
    System.out.println("Uppercase: " + sm.toUpperCase(lowerCaseWord));
​
    // Demonstrate concatenate
    String first = "Hello";
    String second = " World";
    System.out.println("\nFirst Word: " + first);
    System.out.println("Second Word: " + second);
    System.out.println("Concatenated: " + sm.concatenate(first, second));
}
}
​
Step-by-step breakdown for proving correctness of each method:
For reverse(String input) method:
Preconditions:
The input string input should not be null.
Algorithm:
Reverses the input string by iterating over characters and appending them in reverse order.
Postconditions:
The returned string is the reverse of the input string.
For toUpperCase(String input) method:
Preconditions:
The input string input should not be null.
Algorithm:
Converts the input string to uppercase.
Postconditions:
The returned string is the uppercase version of the input string.
For concatenate(String str1, String str2) method:
Preconditions:
Neither str1 nor str2 should be null.
Algorithm:
Concatenates str1 and str2.
Postconditions:
The returned string is the concatenation of str1 and str2.
