# Simple-Calculator-project-in-Java
The Simple Calculator project is a command-line application that allows users to perform basic arithmetic operations, such as addition, subtraction, multiplication, and division.
import java.util.Scanner;

public class SimpleCalculator {
    public static double add(double a, double b) {
        return a + b;
    }

    public static double subtract(double a, double b) {
        return a - b;
    }

    public static double multiply(double a, double b) {
        return a * b;
    }

    public static double divide(double a, double b) {
        return a / b;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter first number: ");
        double a = scanner.nextDouble();
        System.out.print("Enter second number: ");
        double b = scanner.nextDouble();

        System.out.println("Select operation:");
        System.out.println("1. Add");
        System.out.println("2. Subtract");
        System.out.println("3. Multiply");
        System.out.println("4. Divide");

        int choice = scanner.nextInt();

        switch (choice) {
            case 1:
                System.out.println(add(a, b));
                break;
            case 2:
                System.out.println(subtract(a, b));
                break;
            case 3:
                System.out.println(multiply(a, b));
                break;
            case 4:
                System.out.println(divide(a, b));
                break;
            default:
                System.out.println("Invalid choice");
                break;
        }
    }
}
