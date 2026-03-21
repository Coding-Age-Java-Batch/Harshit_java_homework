class FileDownloader implements Runnable {

    private String fileName;
    private int fileSize; // in KB

    public FileDownloader(String fileName, int fileSize) {
        this.fileName = fileName;
        this.fileSize = fileSize;
    }

    @Override
    public void run() {
        System.out.println("Starting download: " + fileName);

        for (int i = 0; i <= 100; i += 10) {

            // Progress bar banana
            int bars = i / 10;
            String progressBar = String.format("%-" + 10 + "s", "").replace(" ", "=").substring(0, bars);

            System.out.println(Thread.currentThread().getName() +
                    " | " + fileName +
                    " | [" + progressBar + ">] " + i + "%");

            try {
                Thread.sleep(500); // delay
            } catch (InterruptedException e) {
                System.out.println(fileName + " download interrupted!");
            }
        }

        System.out.println(fileName + " download completed!\n");
    }
}
