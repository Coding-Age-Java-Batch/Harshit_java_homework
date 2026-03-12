public class Task implements Runnable{
public void run(){
try{
for(int i =0; i<=5; i++){
System.out.print(i + " ");
Thread.sleep(200);
}
} catch (InterruptedException e) {
System.out.println("Thread Interrupted");
}
}

    static void main(String[] args) {
        Task t = new Task();

        Thread td = new Thread(t);

        td.start();
    }
}
