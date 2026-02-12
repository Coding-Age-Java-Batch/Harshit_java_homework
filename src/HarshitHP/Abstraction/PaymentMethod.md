    PaymentMethod {
    void pay(double amount);
    }

    class CredirCard implements PaymentMethod{
    public void pay(double amount){
    System.out.println("Paid " + amount + " using Credit Card");
    }
    }

    class UPI implements PaymentMethod{
    public void pay(double amount){
    System.out.println("Paid " + amount + " using UPI");
    }
    }
    class Cash implements PaymentMethod{
    public void pay(double amount){
    System.out.println("Paid " + amount + " using Cash");
    }

    static void main(String[] args) {
        PaymentMethod cd = new CredirCard();
        PaymentMethod upi = new UPI();
        PaymentMethod cash = new Cash();

        cd.pay(1000);
        upi.pay(500);
        cash.pay(300);
    }
    }

