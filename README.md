# SUM-OF-ABS-DIFF-BTW-ASCII-VALUES-OF-A-STRING
import java.util.*;
class HelloWorld {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        String s1=sc.nextLine();
        int n=s1.length();
        int sum=0;
        char a[]=s1.toCharArray();
        for(int i=0;i<n-1;i++){
            int ch=(int)a[i];
            int m=(int)a[i+1];
            if(ch-m>=0)
            sum=sum+(ch-m);
            else
            sum=sum-(ch-m);
           
        }
        System.out.println("sum : "+sum);
    }
}
