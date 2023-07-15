# practiceprograms

A HashMap is a data structure in Java that stores key-value pairs. It is part of the Java Collections Framework and is based on the concept of a hash table. It provides fast and efficient lookup, insertion, and deletion operations.

In a HashMap, each key is unique, and it is associated with a corresponding value. The key and value can be of any object type. The HashMap uses an internal hashing mechanism to store and retrieve elements based on their hash codes //hashmap functioin to print occurance of characters

import java.util.Scanner;
import java.util.HashMap;
public class Main{
    public static void main(String[] args) throws NullPointerException,ArrayIndexOutOfBoundsException
    {
        Scanner sc=new Scanner (System.in);
        System.out.println("enter the string");
        String name=sc.nextLine();
        String[] str=name.split("");
        HashMap <String,Integer> hash=new HashMap <String,Integer>() ;
        for(int i=0;i<str.length;i++)
        {
            if(hash.containsKey(str[i]))
            {
            int count=hash.get(str[i]);
            hash.put(str[i],count+1);}
            else
            {
               hash.put(str[i],1) ;
            }
        }
        System.out.println(hash);
        
        
    }
}

