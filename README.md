import java.util.*;

public class Demo {
    public static void main(String[] args) {


        String str =" prep p p j insta is best ";
        String[] s1 = str.split(" ");
        for (String x:s1){
            System.out.println(x);
        }

        String s2="";


        for(String x : s1){
            for (int i = 0; i < x.length(); i++) {
                if(i==0 || i==x.length()-1){

                    s2+=Character.toUpperCase(x.charAt(i));
                }
                else {
                    s2+=x.charAt(i);
                }
            }
            s2+=" ";
        }
        System.out.println(s2);
    }
}

