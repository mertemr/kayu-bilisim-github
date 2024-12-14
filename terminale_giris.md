# Bash 101

Bu doküman, Bash terminalinde kullanılabilecek temel komutları ve kısa açıklamalarını içerir. Yeni başlayanlar için anlaşılır bir rehberdir.

---

## Temel Komutlar

- **`ls`** (*List*)  
  Bulunduğunuz dizindeki dosya ve klasörleri listeler.

- **`pwd`** (*Print Working Directory*)  
  Şu anda bulunduğunuz dizinin tam yolunu gösterir.

- **`cd`** (*Change Directory*)  
  Başka bir dizine geçiş yapmanızı sağlar. Örnek:  
  - `cd desktop` → "desktop" adlı dizine geçer.

- **`.. , . , ~ , *`**  
  - `..` → Bir üst dizine geçer.  
  - `.` → Bulunduğunuz mevcut dizini ifade eder.  
  - `~` → Kullanıcının ana dizinini ifade eder.  
  - `*` → Dosya adı eşleştirme için joker karakterdir.

- **`clear`**  
  Terminal ekranını temizler ve komut geçmişini yukarı kaydırır.

---

## Dosya ve Klasör İşlemleri

- **`mkdir`** (*Make Directory*)  
  Yeni bir klasör oluşturur. Örnek:  
  - `mkdir denemeKlasoru` → "denemeKlasoru" adlı bir klasör oluşturur.

- **`touch`**  
  Yeni bir dosya oluşturur. Örnek:  
  - `touch deneme.txt` → "deneme.txt" adlı bir dosya oluşturur.

- **`rm`** (*Remove*)  
  Dosya veya klasörleri siler. Örnek:  
  - `rm deneme.txt` → "deneme.txt" dosyasını siler.  
  - `rm -rf denemeKlasoru` → "denemeKlasoru" adlı klasörü ve içindekileri siler.  
  **Uyarı:** *Yanlış kullanımda dosyalarınızı geri alamazsınız!*

---

## Sistem Güncelleme

- **`sudo apt update && sudo apt upgrade`**  
  Sistemin mevcut yazılım paketlerini günceller.  
  - `sudo apt update` → Paket listesini günceller.  
  - `sudo apt upgrade` → Paketlerin en son sürümlerini yükler.  

---

## Eğlenceli Komutlar

- **`cowsay -f tux "Hello Linux"`**  
  Terminal ekranında bir penguenin "Hello Linux" yazısını konuşuyormuş gibi göstermesini sağlar. Eğlenceli bir görsel komuttur.

---

## Ek Linux Komutları

### 1. **`echo`**  
Ekrana bir mesaj veya metin yazdırır. Örnek:  
- `echo "Merhaba Linux"` → Terminalde "Merhaba Linux" yazar.

### 2. **`cat`**  
Dosya içeriğini terminalde görüntüler. Örnek:  
- `cat dosya.txt` → "dosya.txt" dosyasının içeriğini gösterir.

### 3. **`cp`** (*Copy*)  
Bir dosyayı veya klasörü kopyalar. Örnek:  
- `cp dosya.txt yeni_dosya.txt` → "dosya.txt" adlı dosyayı "yeni_dosya.txt" olarak kopyalar.

### 4. **`mv`** (*Move/Rename*)  
Dosyaları taşır veya yeniden adlandırır. Örnek:  
- `mv dosya.txt yeni_dosya.txt` → "dosya.txt" dosyasını "yeni_dosya.txt" olarak yeniden adlandırır.  
- `mv dosya.txt /home/kullanici` → "dosya.txt" dosyasını belirtilen dizine taşır.

### 5. **`whoami`**  
Hangi kullanıcı olarak oturum açtığınızı gösterir.

### 6. **`date`**  
Sistemin tarih ve saatini görüntüler.

### 7. **`man`** (*Manual*)  
Komutlar için detaylı açıklamaları içeren kılavuzu açar. Örnek:  
- `man ls` → "ls" komutunun ne işe yaradığını, tüm seçeneklerini ve kullanım detaylarını gösterir.

### 8. **`history`**  
Daha önce çalıştırdığınız komutların bir listesini gösterir.

### 9\. **`wget`** (_Web Get_)

Bir web sitesinden dosya indirmenizi sağlayan bir komuttur. Özellikle dosya indirme işlemlerinde kullanılır.  
Örnek:

-   `wget https://example.com/dosya.zip` → "dosya.zip" adlı dosyayı belirtilen URL'den indirir.  
    **Not:** Bazı sitelerde indirme işlemi için internet erişim izni gerekebilir.

### 10\. **`convert`** (_ImageMagick_)

Görselleri farklı formatlara dönüştürmek veya boyutlandırmak için kullanılan bir komuttur.  
Örnekler:

-   `convert dosya.png dosya.jpg` → "dosya.png" görselini "dosya.jpg" olarak dönüştürür.
-   `convert -resize 50% orijinal.jpg yeni.jpg` → Görselin boyutunu %50 küçültüp "yeni.jpg" olarak kaydeder.  
    **Not:** Bu komut, sistemde _ImageMagick_ yüklü olduğunda çalışır.

### 11\. **`htop`**

Sistemin donanım ve işlem kaynaklarını gerçek zamanlı olarak izlemek için kullanılan bir araçtır. _htop_, _top_ komutunun daha kullanıcı dostu ve görselli bir alternatifidir.

-   `htop` → CPU, RAM, işlemler gibi sistem bilgilerini detaylı ve renkli bir arayüzde gösterir.  
    **Not:** Bu komutu çalıştırmadan önce `sudo apt install htop` ile kurulum yapmanız gerekebilir.

### 12\. **`btop`** (_Better Top_)

_htop_ komutunun daha modern ve detaylı bir sürümüdür. Sistem kaynaklarını grafiksel bir şekilde izlemek için kullanılır.

-   `btop` → İşlemci, bellek, disk, ağ kullanımı ve işlemleri görselli bir arayüzde gösterir.  
    **Not:** _btop_ modern sistemlerde tercih edilen bir alternatiftir ve kurulumu için `sudo apt install btop` komutunu kullanabilirsiniz.
