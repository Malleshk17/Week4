import java.util.Scanner;

public class TextAdventureGame {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Welcome to the Text Adventure Game!");
        System.out.println("You find yourself in a mysterious forest. Choose your path wisely.");

        // Start of the game
        int decision;
        do {
            System.out.println("\n1. Go left");
            System.out.println("2. Go right");
            System.out.println("3. Stay put");

            System.out.print("Enter your choice (1, 2, or 3): ");
            decision = getUserChoice(scanner);

            switch (decision) {
                case 1:
                    System.out.println("You encounter a friendly creature. They guide you safely.");
                    break;
                case 2:
                    System.out.println("You stumble upon a dark cave. Enter at your own risk!");
                    break;
                case 3:
                    System.out.println("You choose to stay put and rest. Nothing eventful happens.");
                    break;
                default:
                    System.out.println("Invalid choice. Please choose again.");
            }

        } while (decision != 1 && decision != 2 && decision != 3);

        System.out.println("Thanks for playing the Text Adventure Game!");
    }

    private static int getUserChoice(Scanner scanner) {
        while (!scann
