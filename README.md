# wea\
import java.util.*;
class Main {
    public static void main(String[] args) {
        Random random = new Random();
        Scanner scan = new Scanner(System.in);
        
        int arithmetic = 4;//random.nextInt(4)+1;
        int a = random.nextInt(10)+1;
        int b = random.nextInt(10)+1;
        
        String[] op = {"+","-","*","/"};
        int operator = arithmetic - 1;
        System.out.println("What is " + a + op[operator] + b + "?");
        System.out.print("Answer :");
        int answer = scan.nextInt();
        
        if(arithmetic == 1){
            int add = a + b;
            if(answer == add){
                System.out.println("Correct! The answer is " + add);
            }else{
                 System.out.println("Wrong! The answer is " + add);
            }
        }
        else if(arithmetic == 2){
            int minus = a - b;
            if(answer == minus){
                System.out.println("Correct! The answer is " + minus);
            }else{
                 System.out.println("Wrong! The answer is " + minus);
            }
        }
        else if(arithmetic == 3){
            int times = a * b;
            if(answer == times){
                System.out.println("Correct! The answer is " + times);
            }else{
                 System.out.println("Wrong! The answer is " + times);
            }
        }
        else if(arithmetic == 4){
            double div = a / b;
            if(answer == div){
                System.out.println("Correct! The answer is " + div);
            }else{
                 System.out.println("Wrong! The answer is " + div);
            }
        }
    }
}
