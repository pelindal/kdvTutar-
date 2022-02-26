# kdvTutar-

import java.util.Scanner;
public class kdvHesaplama {
    public static void main(String[] args) {
        Scanner inp=new Scanner(System.in);
        double fiyat;
        System.out.print("Lütfen fiyat giriniz: ");
        fiyat=inp.nextDouble();
        double kdvOrani=(fiyat<=1000)?0.18:0.08;
        double kdv= (fiyat*kdvOrani);
        double yeniFiyat= fiyat+kdv;

        System.out.println("Kdv tutarı: "+ kdv);
        System.out.println("Yeni tutar: "+ yeniFiyat);


    }
}
