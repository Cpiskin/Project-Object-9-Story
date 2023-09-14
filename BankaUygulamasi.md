public class BankaUygulamasi {
    public static void main(String[] args) {
        // Yeni bir banka hesabı oluşturma
        BankaHesabi musteriHesabi = new BankaHesabi("Ahmet Yılmaz", "1234567890");

        // Para yatırma ve çekme işlemleri
        musteriHesabi.paraYatir(1000.0);
        musteriHesabi.paraCek(500.0);

        // Bakiye sorgulama
        double bakiye = musteriHesabi.bakiyeSorgula();
        System.out.println("Hesap Sahibi: " + musteriHesabi.hesapSahibi);
        System.out.println("Hesap Numarası: " + musteriHesabi.hesapNumarasi);
        System.out.println("Hesap Bakiyesi: " + bakiye + " TL");
    }
}
