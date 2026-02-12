    public class BankAccount {
    int balance = 7000;

    void display(){
        System.out.println("Initial Balance: " +balance);
     }
    }
    class SaveAccount extends BankAccount{

    void deposit(int amount){
        System.out.println("Deposited: " +amount);

        balance = balance + amount;

        System.out.println("New balance: " +balance);
    }

    static void main(String[] args) {
        SaveAccount sa = new SaveAccount();
        sa.display();
        sa.deposit(3000);
     }
    }
