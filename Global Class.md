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




