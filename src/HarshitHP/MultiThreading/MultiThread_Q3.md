public class SleepExample extends Thread{

    public void run(){
        try{
            for(int i = 0; i<=5; i++){
                System.out.println("Working...");
                Thread.sleep(500);
            }
        }
        catch(InterruptedException e){
            System.out.println("Thread interrupted");
        }
    }

    static void main(String[] args) {
        SleepExample sp = new SleepExample();
        sp.start();
    }
}
