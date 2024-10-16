package src;

import java.util.Scanner;

public class PocketMoneyCalculator {
    
    public static void main(String[] args) {
        // Create a scanner object to read input
        Scanner scanner = new Scanner(System.in);
        
        // Get weekly budget from the user
        System.out.print("Enter your weekly pocket money budget: $");
        double weeklyBudget = scanner.nextDouble();
        
        // Get the number of weeks from the user
        System.out.print("Enter the number of weeks: ");
        int weeks = scanner.nextInt();
        
        // Calculate total pocket money
        double totalPocketMoney = weeklyBudget * weeks;
        
        // Display the result
        System.out.println("Total pocket money for " + weeks + " weeks is: $" + totalPocketMoney);
        
        // Close the scanner to avoid resource leak
        scanner.close();
    }
}
