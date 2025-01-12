import java.util.Scanner;

class Chilis {

    int servingStaff;
    int waitInMins;
    String address;

    public Chilis(int vacantTables, int waitInMins, String address) {
        this.servingStaff = 10;
        this.waitInMins = 0;
        this.address = "4650 13th St, St Cloud, FL 34769";

    }
    public void askForPartySize() {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the party size: ");
        while (!scanner.hasNextInt()) { // Validate that the input is an integer
            System.out.println("Invalid input. Please enter a valid integer.");
            scanner.next(); // Clear the invalid input
            System.out.print("Enter the party size: ");
        }
        this.waitInMins = scanner.nextInt(); // Read the integer input
        scanner.close(); // Close the scanner
    }
    public void displayWaitTime() {
        System.out.println("The wait time is: " + waitInMins + " minutes.");
    }
    public void displayAddress() {
        System.out.println("Location: " + address);
    }
    public void displayStaffOnHand() {
        System.out.println("Current Staff: " + servingStaff);
    }
}

public class Main {
    public static void main(String[] args) {
        // Create an instance of Chilis
        Chilis chilis = new Chilis(10, 15, "123 Main St");

        // Ask for party size
        chilis.askForPartySize();

        // Display the wait time
        chilis.displayWaitTime();

        // Display the wait time
        chilis.displayStaffOnHand();

        // Display the wait time
        chilis.displayAddress();
    }
}
