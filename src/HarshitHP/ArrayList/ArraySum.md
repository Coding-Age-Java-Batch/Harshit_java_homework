public class ArraySum {
static void main(String[] args) {
int[] num = {4,5,6,4,1};

        int sum = 0;
        for(int i=0; i<num.length; i++){
            sum = sum + num[i];
        }
        System.out.println("Sum of all elements: " +sum);
    }
}
