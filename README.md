a)
integers.

import java.util.Scanner;

public class acad {
public static void main(String args[])
{
Scanner s = new Scanner(System.in);
int b = 123;
int c  = 321;
a= b+c;
System.out.println(a);
}

}

b)

import java.util.Scanner;

public class acad {
public static void main(String args[])
{
Scanner s = new Scanner(System.in);
int x = s.nextInt();
int y  = s.nextInt();
a= x+y;
System.out.println(a);
}

}



c) 


import java.util.Scanner;

public class acad {
public static int sum(int x,int y)
{
int d = x+y;
return d;
}
public static void main(String args[])
{
Scanner s =new Scanner(System.in);
int c = s.nextInt();
int d =s.nextInt();
System.out.println( "First number is:"+c);
System.out.println("Second number is:"+d);
System.out.println("Sum is:"+sum(c,d));
}

}


d)


import java.util.Scanner;

public class acad {
public static void main(String args[])
{
StringBuffer sb = new StringBuffer();
StringBuffer sb1 = new StringBuffer();
Scanner s =new Scanner(System.in);
int x = s.nextInt();
int y =s.nextInt();
for (int i = x; i <=y; i++) {
if(i%2==0)
{
sb.append(i);
sb.append(" ");
}
else
{
sb1.append(i);
sb1.append(" ");
}
}
System.out.println("The even number are");
System.out.println(sb.toString());
System.out.println("The odd number are");
System.out.println(sb1.toString());
}

}

e)



import java.util.Scanner;

public class acad {
public static void main(String args[])
{
Scanner s= new Scanner(System.in);
System.out.println("Input");
int a = s.nextInt();
System.out.println("Output");
for (int i = 1; i <=10; i++) {
System.out.println(a+"x"+i+"="+i*a);
}
}

}


f)


import java.util.Scanner;

public class acad {
public static void sum(int x, int y)
    {
         System.out.println(x+y);
         
    }
    public static void  sum(String s ,String s1)  
    {
     String s2 = s+s1;
         System.out.println(s2);
    }
public static void main(String args[])
{
Scanner s= new Scanner(System.in);
int a = s.nextInt();
int b = s.nextInt();
String s = s.next();
String s4 = s.next();
sum(a,b);//sum with integer type as input
sum(s,s4);// sum with String type as input
}
}
  
  g)Can you overload a method with the same return type? Explain your
answer with proper logic.
  
  Yes we can overload method with same return type but the argument list should be different . If it is the case that arguments are same as that of the other then at least the sequence of the arguments should be changed.
  
Method Overloading means to have two or more methods with same name in the same class with different arguments. The benefit of method overloading is that it allows you to implement methods that support the same semantic operation but differ by argument number or type.

Important Points

Overloaded methods MUST change the argument list
Overloaded methods CAN change the return type
Overloaded methods CAN change the access modifier
Overloaded methods CAN declare new or broader checked exceptions
A method can be overloaded in the same class or in a subclass
import java.util.Scanner;

public class acad {
public static int sum(int x , int y)
    {
return x+y; 
    }
    public static int  sum(char c)  
    {
     int n =(int)c;
         return n;
    }
public static void main(String args[])
{
Scanner s= new Scanner(System.in);
int a = s.nextInt();
int b = s.nextInt();
System.out.println("output");
System.out.println(sum(a,b));//sum with integer type as input
System.out.println(sum('a'));// sum with char type as input
}
}
  Here we can see that the method sum has the same return type but argument list is different one gives actual sum and the other gives the ascii value of the character.
  
  
  h)

import java.util.Arrays;
import java.util.Collections;
import java.util.Scanner;

public class acad {
public static void main(String args[])
{
Scanner s= new Scanner(System.in);
Integer[] intArray = new Integer[5];
for (int i = 0; i < 5; i++) {
intArray[i]=s.nextInt();
}
Arrays.sort(intArray, Collections.reverseOrder());
System.out.println("Output");
for (int i = 0; i < intArray.length; i++) 
{
System.out.println(intArray[i]);
}
}
}

