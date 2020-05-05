package textbasedbank;

import java.util.Scanner;
/**
 * @author jleonn_
 */
public class textBasedBank {

    public static void main(String[] args) {
        
        Scanner input = new Scanner(System.in);
        int userInput;
        int def = 0;
        double[] accountBalance = new double[100];
        String[] accountName = new String[100];
        
        for(;true;){
        
      
        System.out.println("Bank Administration Control");
        System.out.println("+-------------------------+");
        System.out.println("");
        System.out.println("1. Add Customer to the Bank");
        System.out.println("2. Change Customer's Name");
        System.out.println("3. Check Account Balance");
        System.out.println("4. Modify Account Balance");
        System.out.println("5. Summary");
        System.out.println("");
        System.out.println("6. End Control Session");
        
        userInput = input.nextInt();
    
        if (userInput == 1){
            
            System.out.println("New Customer Information");
            System.out.println("+-----------------------+");
            System.out.println("Please specify account balance:");
            double balance = input.nextDouble();
            accountBalance[def] = balance;
            System.out.println("Please enter account name:");
            input.nextLine();
            String name = input.nextLine();
            accountName[def] = name;
            System.out.println("Customer ID: B00" + def);
            def = def + 1;
        
        }
        else if(userInput == 2){
            
            System.out.println("Account Name Update");
            System.out.println("+------------------+");
            System.out.println("Customer ID:");
            int index = input.nextInt();
            System.out.println("What is the new account name?");
            input.nextLine();
            accountName[index] = input.nextLine();
                
        }
        else if(userInput == 3){
            
            System.out.println("Account Balance Information");
            System.out.println("+------------------+");
            System.out.println("Customer ID:");  
            int index = input.nextInt();
            double balance = accountBalance[index];
            System.out.println("Account Balance:" + balance);
         
        }
        
        else if(userInput == 4){
            
            System.out.println("Account Balance Update");
            System.out.println("+------------------+");
            System.out.println("Customer ID:");  
            int index = input.nextInt();
            System.out.println("What is your updated balance?");
            input.nextDouble();
            accountBalance[index] = input.nextDouble();
             
        }
        else if(userInput == 5){
            
            System.out.println("Bank Account Summary");
            System.out.println("+-------------------+");
            System.out.println("");
            double total = 0;
            for (int i = 0 ; i < def ; i++){
                total = total + accountBalance[i];
                System.out.println(accountName[i] + " has RM " + accountBalance[i]);
            }
            System.out.println("There are RM " + total);
        }
        else if(userInput == 6){
            System.out.println("6");
            System.exit(6);
        }
        else{
            System.out.println("ERROR MESSAGE : Invalid Input!");
        }
        }
        
    }
    
}
