public class BankaHesabi {
    // Banka hesabı özellikleri
    private String hesapSahibi;
    private String hesapNumarasi;
    private double bakiye;

    // Constructor (hesap oluşturma)
    public BankaHesabi(String sahipAdi, String hesapNo) {
        hesapSahibi = sahipAdi;
        hesapNumarasi = hesapNo;
        bakiye = 0.0; // Yeni hesapların başlangıç bakiyesi sıfırdır.
    }

    // Para yatırma işlemi
    public void paraYatir(double miktar) {
        if (miktar > 0) {
            bakiye += miktar;
            System.out.println(miktar + " TL yatırıldı. Yeni bakiye: " + bakiye + " TL");
        } else {
            System.out.println("Geçersiz miktar. Pozitif bir miktar giriniz.");
        }
    }

    // Para çekme işlemi
    public void paraCek(double miktar) {
        if (miktar > 0 && miktar <= bakiye) {
            bakiye -= miktar;
            System.out.println(miktar + " TL çekildi. Yeni bakiye: " + bakiye + " TL");
        } else {
            System.out.println("Geçersiz işlem. Bakiye yetersiz veya geçersiz miktar.");
        }
    }

    // Bakiye sorgulama
    public double bakiyeSorgula() {
        return bakiye;
    }
}
