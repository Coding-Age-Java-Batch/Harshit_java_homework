interface Order {
void processOrder();
}
class OnlineOrder implements Order{
private int orderId;
OnlineOrder(int orderId){
this.orderId = orderId;
}
public void processOrder(){
System.out.println("Online order Id: "+ orderId + " Processed successfully");
}
}
class OfflineOrder implements Order{
private int orderId;

    OfflineOrder(int orderId){
        this.orderId = orderId;
    }
    public void processOrder(){
        System.out.println("Offline Order id: " + orderId + " Processes at store");
    }

    static void main(String[] args) {
        Order o1 = new OnlineOrder(101);
        Order o2 = new OfflineOrder(102);

        o1.processOrder();
        o2.processOrder();
    }
}
