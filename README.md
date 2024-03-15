# To-print-program-in-x-pattern-

Program

public class Main{
    public static void main(String[] args) {
        printXPattern("Program");
    }

    public static void printXPattern(String word) {
        int length = word.length();

        for (int i = 0; i < length; i++) {
            for (int j = 0; j < length; j++) {
                if (i == j || j == length - i - 1) {
                    System.out.print(word.charAt(j));
                } else {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }
    }
}
