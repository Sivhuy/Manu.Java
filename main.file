import java.util.Scanner;

public class Menu {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Welcome to Javalicious");
        System.out.println("PLease enter your name: ");
        String name = scanner.nextLine();
        System.out.println("You have a beautiful name ❤️❤️");
        System.out.println("Do you want to pick up for ourselves or order from our app?");
        String pickUpOrOrder = scanner.nextLine();
        if (pickUpOrOrder.equals("order")) {
            System.out.println("Please provide your gmail address: ");
            String gmailaddress = scanner.nextLine();
        } else if (pickUpOrOrder.equals("pick up")) {
            System.out.println("Got it, thank you!!");
        } else {
            System.out.println("Invalid information");
        }
        System.out.println("PLease select your menu");

        // Coffee menu
        String[] coffeeNames = {"Americano", "Espresso", "Latte", "Cappuccino", "Mocha", "Flat White", "None"};
        double[] coffeePrices = {2.50, 2.75, 3.0, 3.50, 4.00, 3.25, 0.00};
        
        // Food menu
        String[] foodNames = {"Fried rice", "Noodle", "Beef stewed with bread", "Brownie", "None"};
        double[] foodPrices = {3.25, 3.0, 2.50, 1.0, 0.00};

        // Print menu
        System.out.println("\n===== Coffee Menu =====");
        for (int i = 0; i < coffeeNames.length; i++) {
            System.out.println((i + 1) + ". " + coffeeNames[i] + " - $" + coffeePrices[i]);
        }
        System.out.println("\n===== Food Menu =====");
        for (int j = 0; j < foodNames.length; j++) {
            System.out.println((j + 1) + ". " + foodNames[j] + " - $" + foodPrices[j]);
        }

        // Take order input
        System.out.print("\nEnter the number of the coffee you want to order: ");
        int coffeeNumber = scanner.nextInt();

        // Validate input
        if (coffeeNumber < 1  coffeeNumber > coffeeNames.length) {
            System.out.println("Invalid selection. Please restart and choose a valid option.");
            return;
        }

        // Get coffee details
        String selected_Coffee = coffeeNames[coffeeNumber - 1];
        double coffeePrice = coffeePrices[coffeeNumber - 1];

        // Get quantity

        System.out.print("Enter the quantity: ");
        int quantity = scanner.nextInt();

        System.out.print("\nEnter the number of the food you want to order: ");
        int foodNumbers = scanner.nextInt();
        if (foodNumbers < 1  foodNumbers > foodNames.length) {
            System.out.println("Invalid selection. Please restart and choose a valid option.");
            return;
        }
        String selected_food = foodNames[foodNumbers - 1];
        double foodPrice = foodPrices[foodNumbers - 1];

        // Get quantity
        System.out.print("Enter the quantity: ");
        int quantity_food = scanner.nextInt();

        if (quantity <= 0) {
            System.out.println("Invalid quantity. Please restart and enter a valid number.");
            return;
        }

        // Calculate total price
        double totalcoffee = coffeePrice * quantity;
        double totalfood = foodPrice * quantity_food;
        double totalprice = totalcoffee + totalfood;

        // Print receipt
        System.out.println("---------------------------");
        System.out.println("==== Purchase Overview ====");
        System.out.println("---------------------------");
        System.out.println(selected_Coffee + " x " + quantity + " - $" + totalcoffee);
        System.out.println(selected_food + " x " + quantity_food + " - $" + totalfood);
        System.out.println("Total price: " + totalprice);
        System.out.println("\nThank you" + " " + name + " " + "for your order! 🙏🏻");

        scanner.close();
    }
}
