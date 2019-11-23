```java
abstract class Cshape{
  protected String color;
  public void setColor(String str){
    color=str;
  }
  public abstract void show();
}

class CTriangle extends Cshape{
  protected double sa,sb,sc;
  public CTriangle(double a,double b,double c){
    sa=a;
    sb=b;
    sc=c;
  }
  public void show(){
    System.out.print("color="+color+", ");
    System.out.println("area="+(0.5*sa*sb));
  }
}
class Main {
  public static void main(String[] args) {
   CTriangle rect=new CTriangle(3, 4, 5);
   rect.setColor("red");
   rect.show();
  }
}
```
