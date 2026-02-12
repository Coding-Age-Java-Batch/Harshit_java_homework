    public class Device {
    String DeviceName = "Samsung Galaxy";

    void showInfo(){
        System.out.println("Device Name: " +DeviceName);
    }
    }
    class Mobile extends Device{
    String os = "Andriod";

    void showInfo(){
        System.out.println("Device Name: " +DeviceName);
        System.out.println("Operating System: " +os);
    }

    static void main(String[] args) {
        Mobile m = new Mobile();
        m.showInfo();
    }
    }
