* Class yapmak istediğimiz işlemleri gruplara ayırmak için kullanıldığı düşünülebilir. O grup üzerinden işlemler yapılır.
* İki tür class vardır. Global ve lokal olarak bulunur.

Se24 üzerin de oluşturulup diğer programlara entegre edilip kullanılabilir.SE80 üzerinde create, class library, class
Şeklinde de oluşturulabilir.

# Global Class
* Class isimlendirilirken cl şeklinde kullanılır. Description kısmın da class'ın açıklaması yapılır.
* Instantiation kısmında class'ın erişebilirliğini gösterir. Public ,protected ,private ,abstract  bulunur.
* Public ile class her yerden erişilebilir.
* Private class'ın kendi dışın da bir yerde erişilmemesi için kullanılır.
* Protected: class'ın kendisinden ve classtan inheritance edilmiş diğer classlar tarafından erişilebilir.
* Abstract Soyut sınıf oluşturmak için kullanılır. 
* Class oluşturulduktan sonra 8 toolbar bulunmaktadır.
  
![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/37152898-d04c-4413-94bf-d05711a71869)

* Properties oluşturduğumuz class'ın özelliklerini gösterir.

## 1-Method
Methodları perform gibi düşünebiliriz. O zaman methodları anlatmaya başlayalım.
1.1-Level: Method un static veya instance olacağı bu kısımda belirlenir.
  *  Instance: Çağrılmadan önce sınıftan bir nesne oluşturulması gerekmektedir. Yani sınıftan nesne oluşturulduktan sonra
çağırılır.
  * Static Bir sınıf nesnesi oluşturulmadan çağırılır. Class'ın static niteliklerine erişebilirler. Yalnız static olayları tetiklemeye
izin verirler.
1.2-Visibility: Method'un erişilebilirlik düzeyini gösterir.
    * Public: Method erişilebilirdir.
    *  Private Method erişilemezdi
    * Protected: Method'un sadece o class içerisinde erişilebilir.
1.3-Method Type Event ile tanımlandığında bu kısımda bir işaret çıkar.
1.4-Description: Method açıklama yazmak için kullanılır.

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/f96c41d5-e7c2-4d45-b49f-805f1d772fb6)

Method oluşturulduktan sonra methodların parametrelerini ve exceptionlarını girmemiz gerekmektedir.

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/17da275d-22b2-40ec-b0cb-4a1e3b6d8a65)


Parameters 
 *Type
     Importing: Parametreyi classa vereceksek kullanılır.
     Exporting: Eğer methoddan veri dönülürse kullanılır.
     Changing Parametremiz class da değişip geliyorsa kullanılır.
     Returning içerisinde veri döndürülüyorsa kullanılır.
 *Pass By Value: parametrelerin içeriğinin değiştirilip değiştirilmeyeceği gösteren kısımdır.
  *Optional: Parametre gönderilmek zorunda değilse isaretlenir.
  *Associated Type: Verinin Tipi gösterir
  *Default Value:  Varsayılan değer isteğe bağlı bir şekilde eklenebilir.
  * Description oluşturulan parametreye açıklama yapmak için kullanılır.
   * Expection Programda olaşılabilecek hataları belirli bir kod şeklinde verebileceğimiz kısımdır.
   * Source kod methodla ilgili kodun yazıldığı yerdir. Method source kod açtığımız zaman 
Parametrelerimizi görmek istersek signature kısmına tıklanır.

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/9aa4f16d-1998-410e-b7dd-df418988bd5e)

## 2-Types:
Class için de kullanacağımız tipleri yönetebileceğimiz kısımdır.

## 3-Attributes:
Data olarak tanımlayacağımız içerikleri bu kısma yazarız. Belli parametreleri önceden tanımlamaya
yarayan alandır.
  3.1-Level 
     *Instance attributes, static attributes yukarıdaki kısımlara benzemektedir. Constant ise sabit ve 
değişmeyen ifadelerde kullanılır.
 3.2-Visibility :Erişim belirteci yukarıda yaptığımız gibidir.
 3.3-Read Only sadece okunabilir içeriktir.
3.4-Typing: (TYPE LIKE REF TO gibi yapılardan hangisini kullancaksak seçeceğim yer)
3.5-Associated Type: Verinin Tipi   (INT4)
3.6-Description: Açıklama
3.7-Inıtial Value: Sabit değişkenlere zorunlu değer vermelisin.
***Tanımlanan attribute herhangi bir method dan direk erişebilir.
![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/575bed2b-b0a2-4fd1-8639-ee0e318f5e63)

## 4-Friends
Başka bir classın methodlarını kullanmamıza yarayan yapıdır,
Methodunu kullanmak istediğimiz class ın friend kısmına hangi class
Da kullanacaksak o class ismi yazılır.

## 5-EVENTS

 Herhangi bir koşul karşılandığında, nesne bir olay oluşturabilir. Ör. Zamanlayıcının süresi doldu,

Interface
Bir temel nesne oluşturup bütün nesnelerden implemente etmek demektir.



