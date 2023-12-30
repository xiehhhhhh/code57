# code57
package x;
import java.util.Random;
import java.util.Scanner;
  

public class x {
    //增加名字
    public static void addname(String[] name){
        Scanner sc=new Scanner(System.in);

        for(int i=0;i<name.length;i++){
            name[i]=sc.next();

        }

    }
    //打印名字
    public static void printname(String[] name){
        for(int i=0;i<name.length;i++){
      System.out.println(name[i]);
        }
    }
//随机名字
    public static String random(String[] name) {
       // Random sc=new Random();
      //  int t=sc.nextInt(name.length);
        int t=new Random().nextInt(name.length);
        String ming=name[t];
        return ming;
    }

    public static void main (String[] args)
    {
      String[] name=new String[3];
      addname(name);
      printname(name);
      random(name);
      String randomname=random(name);
      System.out.println("名字为"+randomname);
    }
}
