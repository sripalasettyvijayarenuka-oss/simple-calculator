import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);

        while (true) {
            try {
                System.out.print("Enter first number (or type '00' to exit): ");
                double num1 = reader.nextDouble();

                System.out.print("Enter an operator (+, -, *, /): ");
                char op = reader.next().charAt(0);

                System.out.print("Enter second number: ");
                double num2 = reader.nextDouble();

                double result;

                switch (op) {
                    case '+': result = num1 + num2; break;
                    case '-': result = num1 - num2; break;
                    case '*': result = num1 * num2; break;
                    case '/': 
                        if (num2 == 0) throw new ArithmeticException("Cannot divide by zero.");
                        result = num1 / num2; 
                        break;
                    default:
                        System.out.println("Invalid operator!");
                        continue;
                }
                System.out.println("Result: " + result);
                System.out.println("------------------");

            } catch (ArithmeticException e) {
               
                System.out.println("Error: " + e.getMessage());
            } catch (Exception e) {
               
                System.out.println("Invalid input! Please enter numbers only.");
                reader.nextLine(); // Clears the error from the scanner memory
            }
        }
    }
}
