    abstract class BankAccount {

    protected double balance;

    void deposit(double amount) {
        if (amount > 0) {
            balance = balance + amount;
            System.out.println("Deposited: " + amount);
            System.out.println("Balance: " + balance);
        }
    }

    abstract void withdraw(double amount);
    }
    class SavingAccount extends BankAccount{
    void withdraw(double amount){
    if(amount <= balance){
    balance = balance - amount;
    System.out.println("Saving withdraw: " +amount);
}
else{
System.out.println("Saving Account: Insufficient balance!");
}
System.out.println("Balance: " +balance);
}
} 
class CurrentAccount extends BankAccount{
private final double overdraftLimit = 10000;

    void withdraw(double amount){
        if(amount <= balance + overdraftLimit){
            balance = balance - amount;
            System.out.println("Current withdraw: " +amount);
        }
        else{
            System.out.println("Current Account: Overdraft limit exceeded!");
        }
        System.out.println("Balance: "+ balance);
    }

    static void main(String[] args) {
        BankAccount saving = new SavingAccount();
        BankAccount current = new CurrentAccount();

        System.out.println("----Saving Account----");

        saving.deposit(5000);
        saving.withdraw(3000);

        System.out.println("----Current Account----");

        current.deposit(5000);
        current.withdraw(4000);
    }
}
