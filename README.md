# Laminasyon Makinesi – Güncelleme Paketleri

Bu depo yalnızca **Laminasyon Makinesi kontrol paneli** programının güncelleme paketlerini dağıtmak içindir.
Kaynak kod burada değildir.

Makinedeki program açılışta ve 6 saatte bir bu deponun **Releases** bölümündeki son sürümü kontrol eder.
Yeni sürüm varsa üst bardaki sürüm rozeti turuncu olur. Kurulumu yalnızca **Servis** veya **Yönetici**
girişiyle ve **makine dururken** başlatılabilir; program kendiliğinden güncellemez.

## Her sürümde iki dosya bulunur

| Dosya | Açıklama |
|---|---|
| `LaminasyonMakinesi-x.y.z.zip` | Program dosyaları (`Config.xml` içermez; makinenin ayarları korunur) |
| `LaminasyonMakinesi-x.y.z.zip.sha256` | Paketin SHA256 doğrulama değeri; program bu değeri tutmayan paketi kurmaz |

## İnternetsiz makineye kurulum (USB)

1. İki dosyayı da aynı klasöre, USB belleğe kopyalayın.
2. Programda Servis/Yönetici girişi yapın, üst bardaki sürüm rozetine dokunun.
3. **Dosyadan / USB'den Kur** ile `.zip` dosyasını seçin.

## Geri dönüş

Her güncellemede önceki sürüm program klasöründeki `_guncelleme_yedekleri` altına yedeklenir (son 3 yedek saklanır).
Yeni sürüm açılamazsa güncelleyici eski sürüme kendiliğinden döner. Elle dönmek için güncelleme penceresinde
**Bu Sürüme Geri Dön** kullanılır.
