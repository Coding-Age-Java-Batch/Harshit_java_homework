public class Rectangle {
int lenth;
int breath;

    Rectangle(int l, int b){
        lenth = l;
        breath = b;
    }
    void compareArea(Rectangle r){
        int area1 = lenth * breath;
        int area2 = r.lenth * r.breath;

        System.out.println("Rectangle 1 and Rectangle 2 have equal area :" +(area1 == area2));
    }

    public static void main(String[] args) {
        Rectangle r1 = new Rectangle(10,5);
        Rectangle r2 = new Rectangle(5,10);

        r1.compareArea(r2);
    }
}