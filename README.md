# lab-exp-1
import java.util.*;
class Complexnumber{
float real,img;
Complexnumber(){
}
Complexnumber(float real,float img){
this.real=real;
this.img=img;
}
void add(Complexnumber c1,Complexnumber c2) {
this.real=c1.real+c2.real;
this.img=c1.img+c2.img;
System.out.println("Addition of no.:"+real+" + i"+img);
}
void sub(Complexnumber c1,Complexnumber c2) {
this.real=c1.real-c2.real;
this.img=c1.img-c2.img;
System.out.println("Subtraction of no.:"+real+" + i"+img);
}
void multi(Complexnumber c1,Complexnumber c2) {
this.real=c1.real*c2.real;
this.img=c1.img*c2.img;
System.out.println("Multiplication of no.:"+real+" + i"+img);
}
void div(Complexnumber c1,Complexnumber c2) {
this.real=c1.real/c2.real;
this.img=c1.img/c2.img;
System.out.println("Division of no.:"+real+" + i"+img);
}
}
public class ComplexResult {
public static void main(String[] args) {
Scanner sc=new Scanner(System.in);
// Program to Calculate Operations on Complex Numbers
float r1,r2,m1,m2;
System.out.println("===================================================
========");
System.out.println("----------------Operations Complex Numbers-----------------");
System.out.print("Enter real part of 1st Complex Number:");
r1=sc.nextInt();
System.out.print("Enter imaginary part of 1st Complex Number:");
m1=sc.nextInt();
System.out.print("Enter real part of 2nd Complex Number:");
r2=sc.nextInt();
System.out.print("Enter imaginary part of 2nd Complex Number:");
m2=sc.nextInt();
Complexnumber C1=new Complexnumber(r1,m1);
Complexnumber C2=new Complexnumber(r2,m2);
Complexnumber C3=new Complexnumber();
System.out.print("\n");
C3.add(C1, C2);
C3.sub(C1, C2);
C3.multi(C1, C2);
C3.div(C1, C2);
}
}
