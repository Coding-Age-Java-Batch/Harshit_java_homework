    class Account {
    double balance;

     Account(double bl){
         balance = bl;
     }
     void showBalance(){
         System.out.println("Balance: " +balance);
     }
    }

    class SavingAccount extends Account{
     double interestRate;

     SavingAccount(double balance, double iRate){
         super(balance);
         interestRate = iRate;
     }
     void showBalance(){
         double updatebalance = balance + (balance * interestRate/100);
         System.out.println("Balance with interest: " +updatebalance);
     }
     public static void main(String[] args){
         SavingAccount sa = new SavingAccount(1000,5);
         sa.showBalance();
     }
    }
