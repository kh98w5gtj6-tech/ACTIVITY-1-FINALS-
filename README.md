# ACTIVITY-1-FINALS-
public class StringExplorer {
    public static void main(String[] args) {

        String sentence = "Java Programming is interesting.";

        System.out.println("Original sentence: " + sentence);
        System.out.println("Length: " + sentence.length());
        System.out.println("Uppercase: " + sentence.toUpperCase());
        System.out.println("Lowercase: " + sentence.toLowerCase());
        System.out.println("First character: " + sentence.charAt(0));
        System.out.println("Last character: " + sentence.charAt(sentence.length() - 1));

        char letter = 'a';
        int count = 0;
        int position = sentence.indexOf(letter);

        while (position != -1) {
            count++;
            position = sentence.indexOf(letter, position + 1);
        }

        System.out.println("Occurrences of a: " + count);
        System.out.println("Contains Java: " + sentence.contains("Java"));
    }
}