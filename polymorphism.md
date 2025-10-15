# Polymorphism

## heritage

```
public class Animal{
...
}

public class Chat extend Animal{

}
```

Noted : C extends B, B extends A  
Constructor C starts to construct A first then B and finish by C

## Interface

```
public interface Vehicule{
    public void passerVitesse();
    public void accelerer();
    public void freiner();
}

public class Moto implements Vehicule{
    public void passerVitesse(){
    ...
    }
    
    public void accelerer(){
    ...
    }
    
    public void freiner(){
    ...
    }
}

```
Noted : Interface contains only signatures  
Not allowed to implement a method into interface  
A class can implemented one or many interfaces  
interface permits multiple heritage  
Methods from interfaces cannot be synchronized

## Abstract

```
abstract ClassName{

    abstract method();
    
    public void methodName(){
    ...
    }

}

class SubClass extends ClassName{
    abstract method(){
    ...
    }
    
    public void methodName(){
    ...
    }
}

```

Abstract class is abstract only if one method is abstract  
a class extends abstract class (not implement)
Methods from interfaces cannot be synchronized