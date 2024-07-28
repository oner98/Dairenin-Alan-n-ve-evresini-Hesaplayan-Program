# Dairenin-Alan-n-ve-evresini-Hesaplayan-Program
import java.util.Scanner;

public class DaireHesaplayici {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        final double PI = 3.14;

        // Kullanıcıdan yarıçapı al
        System.out.print("Dairenin yarıçapını giriniz: ");
        double yaricap = scanner.nextDouble();

        // Kullanıcıdan merkez açının ölçüsünü al
        System.out.print("Merkez açının ölçüsünü giriniz: ");
        double aci = scanner.nextDouble();

        // Dairenin alanını hesapla
        double alan = PI * yaricap * yaricap;
        
        // Dairenin çevresini hesapla
        double cevre = 2 * PI * yaricap;
        
        // Daire diliminin alanını hesapla
        double dilimAlani = (PI * yaricap * yaricap * aci) / 360;

        // Sonuçları ekrana yazdır
        System.out.println("Dairenin Alanı: " + alan);
        System.out.println("Dairenin Çevresi: " + cevre);
        System.out.println("Daire Diliminin Alanı: " + dilimAlani);
    }
}
