    public class Product {
    private int id;
    private String name;
    private double price;

    public Product(){

    }
    public int getid(){
        return id;
    }
    public void setid(int i) {
        id = i;
    }
    public String getName(){
        return name;
    }
    public void setName(String n){
        name = n;
    }
    public double getPrice(){
        return price;
    }
    public void setPrice(double pr){
        price = pr;
    }

    public static void main(String[] args) {

        Product p = new Product();
        p.setid(101);
        p.setName("Laptop");
        p.setPrice(50000);

        System.out.println("Product ID : " +p.getid());
        System.out.println("Product Name : "+p.getName());
        System.out.println("Product Price : " +p.getPrice());
    }
}
