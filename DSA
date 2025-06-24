#Write a Java program to reverse an integer array using the stack data structure.


import java.util.Stack;

public class ReverseArrayUsingStack {
    public static void reverseArray(int[] arr) {
        Stack<Integer> stack = new Stack<>();

        // Push all elements into the stack
        for (int num : arr) {
            stack.push(num);
        }

        // Pop all elements back into the array
        for (int i = 0; i < arr.length; i++) {
            arr[i] = stack.pop();
        }
    }

    public static void main(String[] args) {
        int[] arr = {10, 20, 30, 40, 50};

        System.out.print("Original Array: ");
        for (int num : arr) {
            System.out.print(num + " ");
        }

        reverseArray(arr);

        System.out.print("\nReversed Array: ");
        for (int num : arr) {
            System.out.print(num + " ");
        }
    }
}


Output:
Original Array: 10 20 30 40 50 
Reversed Array: 50 40 30 20 10



#Write a Java program to check if the parentheses in a string are balanced using a stack.


import java.util.Stack;

public class ParenthesesMatcher {
    public static boolean areParenthesesBalanced(String expr) {
        Stack<Character> stack = new Stack<>();

        for (char ch : expr.toCharArray()) {
            if (ch == '(' || ch == '{' || ch == '[') {
                stack.push(ch);
            } else if (ch == ')' || ch == '}' || ch == ']') {
                if (stack.isEmpty()) return false;
                char open = stack.pop();
                if (!isMatchingPair(open, ch)) return false;
            }
        }

        return stack.isEmpty();
    }

    private static boolean isMatchingPair(char open, char close) {
        return (open == '(' && close == ')') ||
               (open == '{' && close == '}') ||
               (open == '[' && close == ']');
    }

    public static void main(String[] args) {
        String expr1 = "{[()]}";
        String expr2 = "{[(])}";

        System.out.println("Expression 1: " + expr1);
        System.out.println("Is Balanced? " + areParenthesesBalanced(expr1));

        System.out.println("Expression 2: " + expr2);
        System.out.println("Is Balanced? " + areParenthesesBalanced(expr2));
    }
}


Output:
Expession:{[()]} => true
Expession:{[()]} => False





#Write a Java program to calculate the sum of all elements in an integer array using a recursive method.


public class RecursiveSum {
    public static int recursiveSum(int[] arr, int index) {
        if (index == arr.length) {
            return 0;
        }
        return arr[index] + recursiveSum(arr, index + 1);
    }

    public static void main(String[] args) {
        int[] arr = {5, 10, 15, 20};

        System.out.print("Array: ");
        for (int num : arr) {
            System.out.print(num + " ");
        }

        int total = recursiveSum(arr, 0);
        System.out.println("\nSum of elements: " + total);
    }
}


Output:
Array Sum:150
