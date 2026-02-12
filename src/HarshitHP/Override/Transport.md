    public class Transport {
    void travelMode(){
    System.out.println("Traveling...");
     }
    }
    class Bus extends Transport{
    void travelMode(){
    System.out.println("Travel by Bus");
     }
    }
    class Train extends Transport{
    void travelMode (){
    System.out.println("Travel by Train");
     }
    }
    class Flight extends  Transport{
    void travelMode(){
    System.out.println("Travel by Flight");
     }

    static void main(String[] args) {
        Transport t;
        t = new Bus();
        t.travelMode();

        t = new Train();
        t.travelMode();

        t = new Flight();
        t.travelMode();
     }
    }

