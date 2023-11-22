# LOCAL CLASS
Sadece tanımlandığı programda kullanılan classlar dır.
Local class defination ve Implementation şeklinde tanımlanır.
Defination Class içerisin de kullanılacak dataları ve methodları tanımlamak için kullanılır.
Implementation : Defination içerisin de tanımladığımız method ve data işlevsellik kazandırmak için
Kullanılır.

### Defination

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/bfe311a7-1e1d-4fab-bef8-3d3f8ddf1017)

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/59c1906d-8c00-44da-a19a-1cc14b1f375a)

### Implementation kısmında methodların kodları yazılır.

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/ab076c69-e7a9-4ad3-8eb3-02f6bc161c70)

### Static ve Instance Data ve Method Tanımlama
Static olarak tanımlamak istersek method veya data önüne class getirmeliyiz.

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/5e051c56-d9ec-4e4d-965e-d62c68bd8094)

### Local Olarak tanımlanan class proje de kullanımı

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/b29ddb7e-ba71-4c70-a11d-31189a22872f)

Local olarak tanımladığımız class programda kullanabilmek için data sonra class vermek
İstediğimiz isim ve type ref to ile oluşturduğumuz local class ismi yazılır.
Classımız da instance method lar olduğu için de  create ile obje tanımlanır.

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/0cbce460-bd27-4e4a-8e91-2daeb60761fd)


Class da implementation kısmında tanımladığımız tüm değişkenlere erişebiliriz .
(public protected private)

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/94f83683-ecb4-4dd3-9974-93c47015c756)

Ama program da obje oluşturup çağırmak isterse de sadece public olan içerikler görünür.

### Inheritance ve Encapsulation

Bir classın içinde bulunan data , method  ve interfaceleri farklı bir classın  içerisin de kullanmaya 
Yarayan yapı inheritance dir.
Class içinde tanımlanan data , method , interfacelerin , program için de veya diğer classlar da kullanıp
Kullanmayacağımızı encapsulation da kullanılır.

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/a44c7d21-bfd0-4c1b-a72e-1516c6d93741)

Bu kısım da class defination  kısmında  inheritance  from yazarak hangi class dan 
Miras alınacağı yazılır.
Implementation kısmında tanımladığımız (public , protected ) erişilebilir.

Program da nesne oluşturup çağırdığımız zaman ise public değişkenler görünmektedir.
![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/5a1657e3-30d5-4b48-8076-8e2b9355e36b)

### Constructors
Program üzerinde bir sınıftan nesne oluşturulduğu zaman veya nesne oluşturmadan(static) 
Çalıştırılacak olan ilk methoddur.
Static constructure tanımlandı ise instance constructorden önce çalışır.
Static Constructors için asla bir arayüz yoktur bu yüzden hiçbir parametre kullanılmaz.
Static Constructors sınıfların yalnızca statik niteliklerine erişebilir.

#### Static Constructors
Genellikle sınıfın veya nesnelerin öznitelikleri için tanımlanmış bir başlangıç değeri ayarlamak için
Kullanılan özel yöntemlerdir.
Dahili bir oturumda bir sınıf ilk kez çağrıldığında, örneğin bir sınıfın örneği oluşturulduğunda veya bir bileşen kullanıldığında, Her sınıf için otomatik olarak ve hemen bir kez çağrılır.

#### Instance Constructors
Constructor Bir ifadenin parçası olarak önceden tanımlanmış ad kullanılarak METHODS bildirilir. Küresel sınıflar söz konusu olduğunda, yalnızca genel görünürlük bölümünde bildirilebilir.
Bir sınıf başlatıldığında ve bir örnek oluşturulduğunda otomatik olarak çağrılır.
Parametrelere sahip olabilir IMPORTING ve istisnalar oluşturabilir.

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/c678a0b0-fed2-4ffd-b975-37c18dbe5dec)

### Abstract Class (Soyut Sınıf)

Direk obje tanımlanarak kullanılmayan ,bir alt sınıf tarafından inherit edilerek kullanılabilen yapılardır.
İçerisinde değiştirilebilen methodlar ve subclass üzerinde tanımlanması zorunlu methodlar barındırır.
Ortak özelliği olan sınıflar için kullanılır.
Method soyut sınıf tanımlamak istiyorsak bu method hangi class için de ise o class abstract olmalıdır.

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/6aba63a0-4739-4601-a45d-04033f85ee91)

Class da definition kısmında abstarct yazılır.
Method tanımlanırken inherit edilecek class lar içerisin de özelleştirmesi zorunlu olan method örneğimiz de bağlamdır.
Definition kısmında method abstarct vermezsek o zaman implementation kısmında özellik vermeliyiz.

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/966edef3-da7c-42c7-8559-4902396d57d5)

Başka bir sınıf abstract olarak oluşturduğumuz sınıfı kalıtı (inheritance ) alırsa miras aldığımız sınıfta abstract olarak tanımladığımız method yani baglan yanına redefinition yazılır .Daha özelleştirip implementation kısmın da baglan metoduna işlev katılır.

Biz abstract class da abstract olarak tanımladığımız methodları bu classtan inheritance alan sınıflarda
Zorunlu olarak bu metodları tanımlamarı gerekmektedir ve yanına da redefinition yazılmalıdır .Diğer metodları tanıtmasak da o zamanda miras aldığımız sınıfta bu metod nasıl tanımlandı ise o şekilde gelir.

### Interface(Arayüz)

Class içerisine yerleştiribilen ,sınıfın işlevselliğini arttırmak için kullanılan yapılardır. Bir classta birden fazla interface tanımlanabilir.Interfacede ki metodlara herhangi bir şey yazılmaz. Interface içerisine alan class da bu metodlar düzenlenir.

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/fcb96446-4aa0-42fb-ae01-86d06ae769ba)

Interface tanımlanırken ve kullanılırken defination ve implemention kullanılmaz.
Class da defination kısmında interface  tanımlanır. Implementation kısmında işlevsellik kazandırılır.

![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/75239fbb-d825-4387-9db8-f1f60dc45380)

Interface deki method kullanacaksak o zaman method interface_name~interface_method_name
Şeklinde çağrılır. Class da interface içerisindeki bir değişken method gibi içerikleri kullanmak için önce interface ismi yazıp daha sonra ~ daha sonra kullanacağımız içeriğin ismi yazılır.


Bir interface birçok sınıf tarafından kullanılabilir.
Interface ve abstract farkı bir class sadece bir tane abstract class inherit edilebilirken ,interfaceler 
İse birden çok sayıda olabilir.

### Polymorphism (Çok Biçimcilik)
![image](https://github.com/sumeyyaakbulut/ABAP-Class/assets/62395974/6225fada-0961-4970-bebc-138232b7917e)

Cl_message_subclass ,cl_message class inheritance alırsa mesaj yaz methodu miras aldığımız 
Sınıfta nasıl tanımlandı ise biz de kendi classımızda öyle gelecektir. Bu method içeriğini
Değiştirmek için polymorphism kullanılır. Method yanına redefinition yazılarak method içeriği değiştirilebilir.

### Final Class

Bir sınıfın artık kalıtım için uygun değil ise uygun olmadığını final class olarak adlandırılır.
Final class alt sınıfı yoktur.
