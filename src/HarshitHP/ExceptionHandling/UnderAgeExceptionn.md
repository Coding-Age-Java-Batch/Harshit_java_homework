class UnderAgeExceptionn extends RuntimeException{
UnderAgeExceptionn(String msg){
super(msg);
}
}
public class VotingCheck{
static void main(String[] args) {
int age = 16;

        try{
            if(age < 18){
                throw new UnderAgeExceptionn("You are underage for voting");
            }
            else{
                System.out.println("You are eligible to vote");
            }
        }
        catch(UnderAgeExceptionn e){
            System.out.println(e.getMessage());
        }
    }
}
