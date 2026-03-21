class DownloadManager {

    public void startDownloads() {

        // 3 files ka list
        FileDownloader file1 = new FileDownloader("File1.mp4", 500);
        FileDownloader file2 = new FileDownloader("File2.pdf", 200);
        FileDownloader file3 = new FileDownloader("File3.zip", 800);

        // Threads create
        Thread t1 = new Thread(file1, "Thread-1");
        Thread t2 = new Thread(file2, "Thread-2");
        Thread t3 = new Thread(file3, "Thread-3");

        try {
            // One by one download (sequence)
            t1.start();
            t1.join();

            t2.start();
            t2.join();

            t3.start();
            t3.join();

        } catch (InterruptedException e) {
            System.out.println("Manager interrupted!");
        }
    }
}