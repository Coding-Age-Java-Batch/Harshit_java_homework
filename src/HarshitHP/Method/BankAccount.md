    public class BankAccount {

    String HolderName;
    int AccNo;
    double balance;

    void setDetails(String hn, int an, double bc){
        HolderName = hn;
        AccNo = an;
        balance = bc;
    }
    void deposite(double amount){
        if(amount > 0){
            balance = balance + amount;
            System.out.println("Amount Deposited " +amount);
        }
        else{
            System.out.println("Invalid deposite Amount ");
        }
    }
    void withdraw(double amount){
        if(amount > 0 && amount <= balance){
            balance = balance - amount;
            System.out.println("Amount withdraw " +amount);
        }
        else{
            System.out.println("Insufficient balance");
        }
    }
    void desplayInfo(){
        System.out.println("Bank Holder name : " +HolderName);
        System.out.println("Account number : " +AccNo);
        System.out.println("Balance : " +balance);
    }

    public static void main(String[] args){

        BankAccount ba = new BankAccount();

        ba.setDetails(" ️Harshit",1000,5000);
        ba.desplayInfo();
        ba.deposite(4000);
        ba.withdraw(3500);


    }

}
