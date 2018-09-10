# Lists
Usage of lists and dictionaries to store and access data.
import java.util.*;
import java.io.*;

class Solution{
    public static void main(String []args){
       
            Scanner s = new Scanner(System.in);
            int n= s.nextInt();
            HashMap<String,Integer>phone= new HashMap<String,Integer>();
            
            for( int i=0; i<n; i++)
            {
                String name=s.next();
                int number=s.nextInt();
                phone.put(name,number);
            }
        
            for(int j=0; j<n;j++)
            {
                String newname=s.next();
                System.out.println(phone.get(newname)!=null? newname+"="+phone.get(newname):"Not found");
            }
        }
        
    }
