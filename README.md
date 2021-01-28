# Reverse-Engineering-02

public class Fruit{
  
    private boolean formalin = false;
    public String name = "";
    
    public Fruit(){
        this.formalin = false;
        this.name = name;    
    }
    
    public String getName(){
        return name;
    }
    
    public boolean hasFormalin(){
        return formalin;
    }
    
}



// public Fruit(boolean formalin, String name){
  //      this.formalin = formalin;
    //    this.name = name;    
    //}


\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
public class Mango extends Fruit {
 
  private boolean formalin = false;
  
    public String name = " ";
    
    public Fruit(){
    this.formalin=true;
    this.name="Mango";
     
    
    }
    
   
    
    public String getName(){
        return name;
    }
    
     public boolean hasFormalin(){
        return formalin;
    }

}

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

import java.util.*;

public class Test{
  
    public static void testFruit(Fruit f){
        System.out.println("----Printing Detail-----");
        if(f.hasFormalin()){      
            System.out.println("Do not eat the "+f.getName()+".");
            System.out.println(f);
        }else{
            System.out.println("Eat the "+f.getName()+".");
            System.out.println(f);
        }
    }  
    
    public static void main(String [] args){
        Mango m = new Mango();
        testFruit(m);
        Jackfruit j = new Jackfruit();
        testFruit(j);
    }
       
}





