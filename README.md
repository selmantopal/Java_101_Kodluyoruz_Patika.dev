# Java_101_Kodluyoruz_Patika.dev
Kodluyoruz ile öğrenmeye başladığım Java için açmış olduğum repo.


Ödev.1 Kod:

import java.util.Scanner;

public class NotOrtalamasi {
  public static void main(String[] args) {
  
        int mat, fiz, kim, tur, tar, muz;
    
        Scanner input = new Scanner(System.in);

        System.out.println("Matematik notunu giriniz : ");
        mat = input.nextInt();
        System.out.println("Fizik notunu giriniz : ");
        fiz = input.nextInt();
        System.out.println("Kimya notunu giriniz : ");
        kim = input.nextInt();
        System.out.println("Turkçe notunu giriniz : ");
        tur = input.nextInt();
        System.out.println("Tarih notunu giriniz : ");
        tar = input.nextInt();
        System.out.println("Muzik notunu giriniz : ");
        muz = input.nextInt();

        double ortalama= (mat + fiz + kim + tur + tar + muz)/6; 
        System.out.println("Derslerin Ortalaması" + ortalama);

        String kaldiMİ = (ortalama<60) ? "Sınıfta Kaldı..." : "Sınıfı Geçti...";
        System.out.println(kaldiMİ);
  }
}
