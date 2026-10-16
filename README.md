Berkay Bağ 
Kod-Asistan v0.1
BAŞLA
  saat = 1
  DÖNGÜ (Her saat başı sensör kontrolü)
    Yazdır: "Lütfen ", saat, ". saat için su seviyesini giriniz:"
    Oku su_seviyesi
    
    EĞER su_seviyesi > 50 İSE
      Yazdır: "Kritik eşik aşılmıştır!"
      DÖNGÜDEN ÇIK (Kır)
    DEĞİLSE
      Yazdır: "Su seviyesi güvenli sınırda. Kapaklar kapalı."
      saat = saat + 1
    EĞER BİTTİ
  DÖNGÜ BİTTİ

  Yazdır: "Tahliye Saati: ", saat
  Yazdır: "Kritik Su Seviyesi: ", su_seviyesi, " metre"
BİTİR
