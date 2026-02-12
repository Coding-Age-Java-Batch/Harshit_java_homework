    public class Book {
    String title;
    String Author;
    Book(String tl, String ar){
    title = tl;
    Author = ar;
    }

    void showDetails(){
        System.out.println("Title: " +title);
        System.out.println("Author: " +Author);;
     }
    }
    class LibraryBook extends Book{
    int shelfNo;
    LibraryBook(String title, String Author, int sn){
    super(title,Author);
    shelfNo = sn;
    }

    void showDetails(){
        System.out.println("Title: " +title);
        System.out.println("Author: " +Author);
        System.out.println("ShelfNumber: " +shelfNo);
    }

    static void main(String[] args) {
        LibraryBook lb = new LibraryBook("Java Programming","John smith",5);
        lb.showDetails();
    }
    }
