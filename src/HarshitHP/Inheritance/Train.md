     class Train {
    void run(){
    System.out.println("Train id Running");
    }
    }
    class Metro extends Train{
    void run(){
    System.out.println("Metro is running on electric track");
    System.out.println("Train is aslo Running");
    }

    static void main(String[] args) {
        Metro m = new Metro();
        m.run();
    }
    }
