# Java Programının Temel Formatı
- Java case sensitive programlama dilidir
- Programlar fonksiyonlar kullanılarak yazılırlar
- Tüm fonksiyonlar, veri gönderme ve veri döndürme özelliklerine sahiptir
- Java programlama dilinin başlangıç noktası main() fonksiyonudur
- **import java.util.*;** ön işlemci direktifidir
- Önişlemci direktifleri compiler’a komutlar gönderir
- java.util bir kütüphanedir. Klavyeden okuma ve ekrana yazma için gerekli deyimleri bulundurur
- import deyimi ile compiler’a java.util araçlarının kullanılacağı bildirilmiştir
- Java çok sayıda kütüphaneye ve araca sahiptir
- Java fonksiyonları kullanılacağı zaman uygun kütüphanenin programa import edilmesi gerekir

# Giriş Çıkış İşlemleri
- Scanner sınfı klavyeden veri okumayı sağlar
- Scanner sınıfı java.util kütüphanesinin içinde yer alır: **import java.util.Scanner;**

![image](https://user-images.githubusercontent.com/113630029/223825438-b9eb5117-0d2a-448f-9898-3e3e58d9bf2a.png)

- Scanner sınıfından üretilen nesne ve System.in sınıfı kullanılarak klavyeden okuma tamamlanır

```java
Scanner tarayici = new Scanner(System.in);
int i = tarayici.nextInt();
double j = tarayici.nextDouble();
```
# Özel Atama İşaretleri
- sayac = sayac + 1;  >> sayac += 1;
- sayac = sayac - 1;  >> sayac -= 1;
- sayac = sayac / 2;  >> sayac /= 2;
- sayac = sayac * 2;  >> sayac *= 2;
- sayac = sayac % 2;  >> sayac %= 2;

Aşağıdaki sırada atama yapılırsa dönüşüm kendiliğinden yapılır
- byte > short > int > long > float > double

# Veri Türünün Dönüştürülmesi
Aşağıdaki kod'da string değişkenin değeri int değişkene aktarılmıştır
```java
String dokuzStringi = “9”;
int a = new Integer(dokuzStringi)
// veya
int b = Integer.parseInt(dokuzStringi);
```
# Uygulamalar
## 8452 Sayısının Basamakları Toplamını Bulan Program
```java
        int sayi = 8452, toplam, binlerBasamagi, yuzlerBasamagi, onlarBasamagi, birlerBasamagi;

        binlerBasamagi = sayi / 1000;
        sayi = sayi - binlerBasamagi * 1000;

        yuzlerBasamagi = sayi / 100;
        sayi = sayi - yuzlerBasamagi * 100;

        onlarBasamagi = sayi / 10;
        sayi = sayi - onlarBasamagi * 10;

        birlerBasamagi = sayi / 1;
        sayi = sayi - birlerBasamagi * 1;

        toplam = binlerBasamagi + yuzlerBasamagi + onlarBasamagi + birlerBasamagi;

        System.out.println("Basamaklar Toplamı: "+ toplam);
```
## Bir Sayının Tersini Ekrana Yazdıran Program
```java
        Scanner scan = new Scanner(System.in);

        System.out.print("Bir Sayı Giriniz: ");
        int sayi2 = scan.nextInt();

        System.out.print("Girdiğiniz Sayının Tersten Yazılışı: ");

        while(sayi2 > 0) {

            System.out.print(sayi2 % 10);
            sayi2 /= 10;
        }
```
## Kullanıcıdan 5 Tane Tam Sayı Alan ve Bu Sayıların Ortalamasını Bulup Ekrana Yazdıran Program
```java 
        int s1, s2, s3, s4, s5;
        double ortalama;

        Scanner inp = new Scanner(System.in);

        System.out.print("Art arda 5 sayı giriniz: ");

        s1 = inp.nextInt();
        s2 = inp.nextInt();
        s3 = inp.nextInt();
        s4 = inp.nextInt();
        s5 = inp.nextInt();

        ortalama = (s1+s2+s3+s4+s5) / 5;

        System.out.println("Girdiğiniz Sayıların Ortalması: " +ortalama);
```
