# hesap-makinesi
patika.dev hesap makinesi

import java.util.Scanner;
public class main {
    public static void main (String[]args){
int n1,n2,sltn;
double sonuc;
System.out.println("Yapmak istediğiniz işlemi seçiniz:");
System.out.println("1- Toplama \n 2- Çıkartma \n 3- Çarpma \n 4- Bölme");
Scanner inp = new Scanner(System.in);
sltn = inp.nextInt();
System.out.print("1. sayıyı giriniz:");
Scanner aaa = new Scanner(System.in);
n1 = aaa.nextInt();
System.out.print("2. sayıyı giriniz:");
Scanner bbb = new Scanner(System.in);
n2 = bbb.nextInt(); 

switch (sltn) {
case 1 : System.out.print("Toplam= "+ (n1 + n2));
    break; 
case 2 : System.out.print("Kalan= "+ (n1 - n2));
    break;
case 3 : System.out.print("Çarpım= "+ (n1*n2));
    break;
case 4:
     if (n2 == 0) {
        System.out.println("Bir sayı sıfıra bölünemez");
break;
    }else{
    sonuc = n1 / n2;
    System.out.println("İşlemin sonucu : " + sonuc);}
break;
    
default :
 System.out.println("Hatalı giriş yaptınız");

        }
    }
}
