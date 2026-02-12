    public class LibraryBook {
    String title;
    String author;
    boolean isAvailable;

    void setDetails(String tl, String ar){
        title = tl;
        author = ar;
        isAvailable = true;
    }

    void borrowBook(){
        if(isAvailable){
            isAvailable = false;
            System.out.println("Book has been borrowed");
        }
        else{
            System.out.println("Book is already borroweed");
        }
    }

    void returnBook(){
        isAvailable = true;
        System.out.println("Book has been return");
    }
    void displayStatus(){
        System.out.println("Title : "+title);
        System.out.println("Author : "+author);
        if(isAvailable){
            System.out.println("Status: Available");
        }
        else{
            System.out.println("Status: Not Available");
        }
        System.out.println("        ");
    }
    public static void main(String[] args){
        LibraryBook book = new LibraryBook();

        book.setDetails("Java Programming","James Gosling");
        book.displayStatus();

        book.borrowBook();
        book.displayStatus();

        book.returnBook();
        book.displayStatus();
    }
}
