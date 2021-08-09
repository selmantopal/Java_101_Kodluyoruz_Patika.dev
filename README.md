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

