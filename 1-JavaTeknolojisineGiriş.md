# Bilgisayar Programları Nasıl Çalışır
1. Bilisayar programları kullanıcıdan giriş alır
2. Bu girişlere göre veriler üzerinde işlemler yapılır
3. Gerekliyse bu sonuçlar ara yüzde gösterilir

# Program Nedir ?
 Program, günlük hayatta bir sorunu bilgisayar ile çözmek, rutin işlemleri kolaylaştırmak için yazılan kodlardır

# Programlama Dili Nedir ?
 Programlama Dilleri programcının bilgisayar programı yazarken kullandığı özel dillere denilmektedir
 Yazılan programlar bir derleyici vasıtası ile Makine diline çevrilir varsa hataların bulunmasını sağlar ve yazılımcı bu hataları düzeltir
 
# Programlamanın Tarihçesi
1990’li yıllar ve sonrası internetin yaşamımıza girmesiyle programlama dilleri gelişmiştir . JAVA (1991), JavaScript (1995), PHP (1995), C# (2001).

# Programlamanın Temelleri
Başarılı bir programlama için aşağıdaki adımlar izlenmelidir:
1. Problemin anlaşılması, programın giriş ve çıkışlarının belirlenmesi
2. Problemin çözümü için gerekli bileşenlerin belirlenmesi
3. Programın anahtar özelliklernin belirlenmesi, akış diyagramı ve sözde kodun oluşturulması
4. Programın her bir parçasının belirlenmesi ve test edilmesi
5. Sonraki versiyonlar için gereksinimlerin belirlenmesi ve önceki adımların tüm versiyonlar için tekrarlanması

# İyi Bir Yazılımın Özellikleri
- Doğruluk(Correctness): Bir projeye başlamadan önce beklentilerin belirlenmesi gerekir. Proje bittikten sonra beklentiler tam olarak sağlanmış olmalı
- Dayanıklılık(Robustness): Program iyi yönde bile olsa kendinden beklenmeyen işlemler yapmamalı
- Genişleyebilme(Extendibility): İleri aşamalarda projede değişiklik veya ilave işlemler yapılabilmeli
- Tekrar Kullanma(Reusability): Bir projede kullanılan elemanlar başka bir projedede kulanılabilmeli
- Uygunluk(Compatibility): Farklı bilgisayar sistemlerinde aynı ortak özelliklere sahip olunmas
- Kaynakların Kullanımı (Efficiency): Bir yazılımın belirlenen şartlar altında kullanılan kaynakların miktarına bağlı olarak uygun performansı sağlaması

# Programlama Dillerinin Seviyeleri ve Özellikleri
- Bilgisayarlar gibi programlama dilleri de çeşitli süreçlerden geçerek çeşitli seviyelere ulaşmışlardır
- Yüksek seviyeli diller insan algısına daha yakınken, düşük seviyeli diller ise bilgisayarların doğal
çalışmasına daha yakındır.
- Üst seviyeli diller donanıma en uzak dillerdir. Hatta donanım hakkında hiç bir bilgi bilmeyi bile gerektirmez. Hazır
kütüphanesi, sınıfı ve fonksiyonu vardır (Java, C#, Delphi)
- Orta Seviyeli diller hem donanıma hitap eder, hem de uygulama geliştirme de kullanılır. Aslında daha çok uygulama programları ile makine arasında aracı görevi görür(C, C++). Orta Seviyeli diller Alt seviyeli diller ile yazılır(C dili, Makine Kodu ve Assembly ile; Java Runtime, Net Framework de C)
- Alt seviyeli diller donanıma en yakın dillerdir. Donanım hesaba katılarak programlama yapılır. Daha fazla programcılık becerisi gerektirir (Assembly, Makine Kodu)
-  Programla dillerinde seviye yükseldikçe programcının kod yazma işi de kolaylaşır
-  Bilgisayarlar en temelde 0 ve 1 ’lerden oluşan kodları anlayabilmektedirler Bir programcı yüksek seviyeli bir dilde kod yazdığında bu kodların bilgisayar tarafından yorumlanıp çalıştırılması için o kodların makine dilene çevrilmesi gereklidir.

# Bilgisayar Programlarının Çalışma Prensibi
Yüksek seviyeli dille yazılmış kaynak kodun makine diline çevrilmesine derleme denilmektedir
- Kaynak kod -> Derleyici -> Makine kodu

# Programlama Dillerinin Türleri
Makine Dili:
- Bilgisayarın doğal dilidir
- Bilgisayarın donanımsal tasarımına bağlıdır
- "01010101" gibi ifadelerden oluşan komutlardır
- Makine dili işlemci türüne özel olarak yazılmaktadır. Bu nedenle, bir işlmeci türü için makine dili ile yazılmış program, diğer işlemciler için uygun olmamaktadır

Assembly Dili Programlama:
- Assembly insanlar tarafından anlaşılması zor olan makina dilinin sayısal ifadelerini, insanlar tarafından anlaşılarak programlanması daha kolay olan alfabetik ifadelerle değiştirerek düşük seviyede programlama için bir ortam oluşturur
- Bir assembly dil programı, çevirici (assembler) olarak adlandırılan faydalı bir program tarafından hedef
bilgisayarın makine koduna çevrilir

Yapısal Programlama:
- Yapısal programlamada problem çözümü daha kolay alt modüllere bölünür. Her bir alt modül daha düşük seviyedeki alt seviyelere bölünür.
- Uzun ve karmaşık programların, modüllere ayrılarak daha kolay biçimde yazılabilmesini mümkün kılar.
- Programcılar büyük kod parçalarını daha kısa ve dolayısıyla anlaşılırlığı yüksek alt yordamlar halinde yazarlar.

# Yorumlayıcı(Interpreter) ve Derleyici(Compiler) Nedir ?
Yüksek seviyeli dil ile yazılmış olan programa kaynak kodu denir. Kaynak kodunun bilgisayarda çalıştırılabilmesi için makine koduna dönüştürülmesi gerekir. İşte bu iş ya Derleyici (Compiler) ya da Yorumlayıcı (Interpreter) tarafından gerçekleştirilir.

|Derleyici   |Yorumlayıcı   |
|---|---|
|Tüm programı tarar ve bir bütün olarak makine koduna çevirir   |Programı satır satır işler   |
|Kaynak kodun analizi için büyük zaman harcar. Ancak genel yürütme süresi daha hızlıdır.   |Kaynak kodu analiz etmekle zaman harcamaz. Ancak genel yürütme süresi daha yavaştır.   |
|Tüm kaynak kodu taradıktan sonra hata mesajı üretir. Bu nedenle hata ayıklama nispeten zordur.   |Herhangi bir hata olana kadar programı çalıştırır. İlk hata gördüğü yerde durur. Bu nedenle hata ayıklama kolaydır.   |
|C, C++ gibi diller derleyici kullanır.   |Python, Ruby, Java gibi diller yorumlayıcı kullanır.   |

## Derleyici (Compiler)
Derleyici (Compiler), girdi olarak yüksek seviyeli programlama diliyle yazılmış kaynak kodu alan, makinenin mimarisine göre makine dilinde çıktı üreten bir programdır. 

Örnek olarak; Java derleyicisi **javac** verilebilir. **Javac**, .java uzantılı **kaynak dosyasını** Java Sanal Makinesi (Java Virtual Machine)  olarak bilinen bir hayali makine için  makine dili olan Java bytecode ile yazılmış **.class** dosyasına dönüştürür.

## Yorumlayıcı (Interpreter)
Yorumlayıcı (Interpreter), girdi olarak program için olan verilerle birlikte kaynak kodu olan, ve kaynak programı satır satır yürüten bir programdır.

Örnek olarak Java yorumlayıcısı java verilebilir. Java .class uzantılı dosyayı üzerinde çalıştığı makinede çalıştırılabilecek olan doğal makine kodlarına çevirir.

Java’da derleyici ve yorumlayıcı beraber çalışır. Yani, önce oluşturulan kaynak koddan bir ara kod (bytecode) üretilmek için derlenir. Daha sonra bu derlenen bytecode Java Sanal Makinesi (JVM) üzerinde yorumlanarak yürütülür. Bu bazı avantajları da beraberinde getirir. En önemlisi platform bağımsızlığıdır.

JVM çalışan her makinede bytecode’larımız sorunsuz çalışacaktır. İkinci avantajı ise Java bytecode’umuz bir sanal makine üzerinde çalıştığı için kötü amaçlı programlara karşı koruma sağlayan bir güvenlik katmanı ile korunmuş oluruz.

Java bytecode ve java yorumlayıcısı sadece Java dilinde kullanılmaz. Örnek olarak, Jython’u Python dilinden Java bytecode’una derlemek için kullanabiliriz ve daha sonra da yorumlamak için java‘yı kullanabiliriz. 

# Java Programlama Dili

Java, Sun Microsystems mühendislerinden James Goslingfikri;
- C++’da bir program yazdığınızda, 10 tane cihazınız varsa her seferinde derleyip yazmak zorunda
kalınıyordu.
- O zaman bununla uğraşacağıma üstene yorumlayıcı bir dil yazılsın. Programcılar ilgili programı ortak yazsın işlemciye göre çevirme işini Java Sanal Makinesi yapsın denmiştir.
Bu fikirden sonra javanın temelleri atılmaya başlanmıştır

## Neden Java ?
- Açık kanak kodlu
- Nesne yönelimli
- Platform bağımsız
- Yüksek performanslı
- Çok görevli
- Yüksek seviyeli
- Adım adım işletilen(yorumlanan-interpreter) bir dildir

## Java Sanal Makinesi (Java Virtual Machine)

Birçok programlama dilinde derlenen program, bu işlemin gerçekleştirildiği makinedaki komut setine göre bağlanır.
Makinadaki komut seti işlemci mimarisine ve işletim sistemine göre değişmektedir.
Bu durumda derlenip bağlanarak yürütülebilir hale getirilen programlar sadece işlem yapılan makina üzerinde mi çalışacaktır?

## Java'nın Çalışma Prensibi Nasıldır
1. Yazılan java kodu önce compiler(javac) ile derlenerek bytecode'a (.class) dönüştürülür
2. Ardından bytecode Java Virtual Machine (JVM) ile tüm platformlarda kodu çalışacak hale getirir (makine diline dönüşür)

![image H1RQ01](https://user-images.githubusercontent.com/113630029/222278389-b55ab0fb-35dd-4e42-9854-afef0afd78be.png)

## Java-Temel Özellikler
- Platform bağımsız; “Bir kez yaz ve her yerde çalıştır” (“write once, run anywhere”)
- Otomatik Çöp Toplama ("garbage collection")
- Sun, Kasım 2006’da Java bilesenlerini, “GNU General Public Licence” altında açık kaynak
olarak yayınladı

## Java Runtime Environment-JRE
Java uygulamalarının bilgisayar üzerinde koşturulmasını sağlayan yazılımdır.
Java Çalıştırma Ortamı iki kısımdan oluşur :
- Java Sanal Makinesi (“Java Virtual Machine” JVM)
- Uygulama Programlama Ara yüzü (“Application Programming Interface ”
API)

JVM ve API birbirine tutarlıdır ve bu yüzden JRE altında birleştirilmiştir

JRE'nin Java uygulamalarını çalıştıran sanal bir bilgisayar olduğunu düşünürsek; JVM işlemci, API kullanıcı arayüzü olur

![image](https://user-images.githubusercontent.com/113630029/222314435-638664a9-cb59-4ba8-a546-78b645726f3f.png)


## Application Programming Interface - API
Java API, Java yazılımlarında kullanılan yazılım kütüphanelerine genel olarak verilen isimdir.
- Java API ile disk, grafik, ağ, veri tabanı, güvenlik gibi yüzlerce konuda kullanıcılara erişim
imkanı sunulur.
- Java API, J2SDK’nın (“Java2 Software Development Kit”) bir parçasıdır.
Sun, farklı uygulama ortamlarını desteklemek için, farklı API’lar tanımlamıştır
- Java Platform, Micro Edition (Java ME): Avuçiçi aygıtlar gibi kısıtlı kaynaga sahip ortamlar
için
- Java Platform, Standard Edition (Java SE): Masaüstü bilgisayarlar ve is istasyonları için
- Java Platform, Enterprise Edition (Java EE): Genis dagıtık sistemler ve web sunucuları için

![image](https://user-images.githubusercontent.com/113630029/222314756-74ddcfff-1a66-4e75-a533-babf2c1f8faf.png)

## Java Kaynak Dosyasının Yapısı 
- Programlamada kodların yazıldığı dosyalara kaynak dosyası denilmektedir
- Java kaynak dosyaları **.java** uzantısı ile oluşturulurlar
- Java kaynak dosyaları oluşturulurken dikkat edilecek ilk kural, kaynak dosyaların içerisinde dosyayla aynı adı taşıyan bir sınıf ya da arayüz bulunması gerekliliğidir
- Bir java kaynak dosyası üç ana bölümden oluşur: paket bildirimi, kütüphane ekleme, kod bloğu

## Paket Bildirimi
- Java’da kaynak dosyalar veya derlenmiş halleri bilgisayarımızdaki dosya sistemine benzer bir hiyerarşide tutulurlar
- Nasıl ki bilgisayarımızdaki tüm dosyalar bir dizinde tutuluyorsa kaynak dosyalarımız da mutlaka bir paket içerisinde tutulmalıdır
- Paketler başka paketlerin içerisinde bulunabilirler
- Örneğin java’da dosya işlemlerini yapan File java kaynak dosyası java paketinin içerisindeki io paketine aittir Bu nedenle File java dosyasının en üst kısmında **Package java.io;** ifadesi bulunur 
- Bir kaynak dosya sadece bir pakete ait olabilir dolayısıyla kaynak dosyasında sadece bir adet paket bildirimi olur.

## Kütüphane Ekleme
- Daha önceden yazılmış ve programcının kullanımına sunulmuş kaynak dosyalar ya da bunların derlenmiş haline kütüphane denilmektedir
- Java'da kütüphane bildirimi, paket bildirminin ardından yapılmaktadır
- Yukarıda bahsettiğimiz File java kaynak dosyasından üretilmiş File sınıfını yeni yazacağımız kodda kullanmak istersek **import java.io.File;** ifadesini kullanmamız gerekir

## Java'da İsimlendirme 
- Dosya ve sınıf isimlendirmede bütün kelimelerin ilk harflari büyük olmaldır (Araba.java , IlkProje.java)
- Metot ismlerinin ilk harfleri küçük olarak yazılırken, bir den fazla kelime olması durumunda ilk kelime hariç bütün kelimelerin ilk harfi büyük yazılır (merhaba.java , javaOgreniyorum.java)
- Paket isimleri tamamen küçük harf ile oluşmalıdır, ayrıca alt paketler **.** ile birbirinden ayrılır (java.io , java.sql)
- Değişken isimleri küçğük hafler başlar. Değişken ismi birden fazla sözcükten oluşuyorsa, sözcükler arasında boşluk bırakmadan ilk sözcük hariç diğer tüm sözcüklerin ilk harfi büyük olacak şekilde isimlendirilir (dogumYeri , adi)
- Java’da sabit isimleri büyük harflerden oluşur. Sabit ismi birden fazla sözcükten oluşuyorsa, sözcükler arasında “_” karakteri konularak isimlendirilir (RAKIM - PI_SAYISI)
- Java **case sensitive** programlama dilidir "toplam", "Toplam" ve "TOPLAM" birbirinden farklıdır
- Java programları fonksiyonlar halinde yazılır
- Tüm fonksiyonlar, bir isme, data gönderme ve data döndürme özelliklerine sahiptir
- Fonksiyonlar programın işlevlerini gerçekleştirir
- Java programlarının başlangıç noktası main() fonksiyonudur

> Java dili ile programlama yapabilmek için "JDK" ve "IDE" kurulmalıdı
