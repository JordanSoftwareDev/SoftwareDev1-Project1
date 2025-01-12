import java.util.Scanner;

class HashHouseAGoGo {


    int servingStaff;
    String mealBeingServed;
    String address;

    public HashHouseAGoGo(int servingStaff, String mealBeingServed, String address) {
        this.servingStaff = 13;
        this.mealBeingServed = "";
        this.address = "5350 INTERNATIONAL DR, ORLANDO, FL 32819, UNITED STATES";

    }

    public void askForResTime() {
        Scanner scanner = new Scanner(System.in);
        int number = 0;
        boolean validInput = false;

        while (!validInput) {
            System.out.print("Enter your reservation time (as an integer in military time): ");
            System.out.println("\n");

            if (scanner.hasNextInt()) {
                number = scanner.nextInt(); // Read the integer input
                if (number >= 6 && number <= 15) {
                    validInput = true; // Exit the loop
                }
                else {
                    System.out.println("\n");
                    System.out.println("Restaurant opens at 6am and closes at 3pm. Please choose another time slot.");
                }
            } else {
                System.out.println("Invalid input. Please enter a valid integer.");
                scanner.next(); // Clear the invalid input
            }
        }

        // Check if the number is between 6 and 11

        if (number >= 6 && number <= 11) {
            mealBeingServed = "Breakfast";
        } else {
            mealBeingServed = "Brunch";
        }

        System.out.println(mealBeingServed);
        scanner.close(); // Close the scanner
    }

    public void displayMeal() {
        System.out.println("The meal is: " + mealBeingServed);
    }

    public void displayAddress() {
        System.out.println("Location: " + address);
    }

    public void displayStaffOnHand() {
        System.out.println("Current Staff: " + servingStaff);
    }
}
public class HashHouse {
    public static void main(String[] args) {
        // Create an instance of hashHouse
        HashHouseAGoGo hashHouseAGoGo = new HashHouseAGoGo(10, "", "5350 INTERNATIONAL DR, ORLANDO, FL 32819, UNITED STATES");

        // Ask for party size
        hashHouseAGoGo.askForResTime();

        // Display the wait time
        hashHouseAGoGo.displayMeal();

        // Display the wait time
        hashHouseAGoGo.displayStaffOnHand();

        // Display the wait time
        hashHouseAGoGo.displayAddress();
        }
    }

