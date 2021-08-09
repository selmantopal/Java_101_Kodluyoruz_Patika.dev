# Java_101_Kodluyoruz_Patika.dev
Kodluyoruz ile öğrenmeye başladığım Java için açmış olduğum repo.


Ödev #1 Kod:

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

            String kaldiMİ = (ortalama<60) ? "Sınıfta Kaldı!" : "Sınıfı Geçti.";
            System.out.println(kaldiMİ);
        }
     }
     
Ödev #2 Kod:
      
      import java.util.Scanner;

      public class KdvHesaplama {
      
         public static void main(String[] args) {
        

            double fiyat, kdv, kdvli, kdv1 = 0.18, kdv2= 0.08;

            Scanner input = new Scanner(System.in);
            System.out.print("Fiyat giriniz :");
            fiyat = input.nextDouble();


            boolean kosul1 = fiyat >= 0;
            boolean kosul2 = fiyat <= 1000;
            boolean sonuc = kosul1 && kosul2;

            System.out.println("KDV'siz Fiyat :" + fiyat);

            kdv= sonuc ? kdv1 : kdv2;
            kdvli = fiyat + (fiyat * kdv);

            System.out.println("KDV'li Fiyat :" + kdvli);
            System.out.println("KDV Tutarı :" + kdv);
         
        }
    }
    
Ödev #3 Kod:


    import java.util.Scanner;

    class Main {
        public static void main(String[] args) {
        
            double kenar1, kenar2, hipotenus;

            Scanner inp = new Scanner(System.in);
            System.out.print("Üçgenin birinci kenar uzunluğunu giriniz :");
            kenar1= inp.nextDouble();
            System.out.print("Üçgenin birinci kenar uzunluğunu giriniz :");
            kenar2= inp.nextDouble();
      
            hipotenus = Math.sqrt ((kenar1*kenar1)+(kenar2*kenar2));

            System.out.println("Üçgenin hipotenüs uzunluğu : "+" "+ hipotenus);


            double a, b, c;

            System.out.println("Alan hesaplama ----------");

            System.out.print("Üçgenin 1. kenarını giriniz :");
            a = inp.nextInt();

            System.out.print("Üçgenin 2. kenarını giriniz :");
            b = inp.nextInt();

            System.out.print("Üçgenin 3. kenarını giriniz :");
            c = inp.nextInt();

            double alan, u;

            u=(a+b+c)/2;
            alan = Math.sqrt (u*(u-a)*(u-b)*(u-c));

            System.out.print("Üçgenin alanı :" + alan);

        }  
    }

Ödev #4 Kod:


       import java.util.Scanner;


       class Main {
              public static void main(String[] args) {

                     double km, katSayi=2.2, minUcret=20, acilisUcret=10, toplamUcret, odenecekUcret;  

                     Scanner inp = new Scanner(System.in);
                     System.out.println("Gidilmiş olan km mesafesini giriniz :");
                     km = inp.nextDouble(); 

                     toplamUcret = acilisUcret + (km*katSayi); 
                     boolean kosul = toplamUcret <20;
                     odenecekUcret = kosul ? minUcret : toplamUcret;

                     System.out.println("Taksimetre Tutarı :"+ " " + odenecekUcret + "  "+"TL'dir.");
              }
       }
       
       
Ödev #5 Kod:
 
       import java.util.Scanner;

       class Main {
       
              public static void main(String[] args) {
              
                     int r;
                     double pi = 3.14, alan, cevre;

                     Scanner inp = new Scanner(System.in);
                     System.out.println("Yarıçapı giriniz :");
                     r = inp.nextInt();

                     alan= pi*r*r;
                     System.out.println("Dairenin Alanı : " + alan + "cm\u00B2");

                     cevre= 2*pi*r;
                     System.out.println("Dairenin Çevresi : " + cevre + "cm");

                     double merkezAci, daireDilimAlan;
                     System.out.print("Dairenin merkez açısını giriniz : ");
                     merkezAci = inp.nextDouble();

      
                     daireDilimAlan=(pi*(r*r)*merkezAci)/360;
                     System.out.println("Daire diliminin alanı : " + daireDilimAlan + "cm\u00B2");
              }
       } 
       
       
Ödev #6 Kod:

       import java.util.Scanner;

       class Main {
              public static void main(String[] args) {

                     double boy, kilo, indeks;

                     Scanner i = new Scanner(System.in);
                     System.out.println("Lütfen boyunuzu(metre cinsinde) giriniz : ");
                     boy=i.nextDouble();

                     System.out.println("Lütfen kilonuzu giriniz : ");
                     kilo=i.nextDouble();

                     indeks = kilo/(boy*boy);
                     System.out.println("Vücut Kitle İndeksiniz : " + indeks);
              }
       }
       
       
Ödev #7 Kod:

       import java.util.Scanner;

       public class ManavKasa {
       
              public static void main(String[] args) {
              
                     double armutKg=2.14, elmaKg=3.67, domatesKg=1.11, muzKg=0.95, patlicanKg=5, armut, elma, domates, muz, patlican, toplamTutar;
                     Scanner input = new Scanner(System.in);

                     System.out.print("Armut Kaç Kilo ? :");
                     armut = input.nextFloat();

                     System.out.print("Elma Kaç Kilo ? :");
                     elma = input.nextFloat();

                     System.out.print("Domates Kaç Kilo ? :");
                     domates = input.nextFloat();

                     System.out.print("Muz Kaç Kilo ? :");
                     muz = input.nextFloat();

                     System.out.print("Patlıcan Kaç Kilo ? :");
                     patlican = input.nextFloat();

                     toplamTutar=(armut*armutKg)+(elma*elmaKg)+(domates*domatesKg)+(muz*muzKg)+(patlican*patlicanKg);
                     System.out.print("Toplam Tutar :" + toplamTutar + " TL");
              }
       }

