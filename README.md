# Degisken-Turleri
C programlama dilinde, programda kullanılan değişkenler (variables), programın
başında kullanılmadan önce tanımlanmalıdır. C programlama dilinde 4 temel veri
tipi vardır. 
Bunlar: karakter (character) tipi, tamsayı (integer) tipi, kayan noktalı
(floating point) sayı tipi ve büyük kayan noktalı (double floating point) sayı tipidir.
Yukarıda sıralanan temel veri tipleri sırasıyla char, int, float ve double
sözcükleriyle tanımlanırlar.
int tipi değişkenler, tamsayı tipi ve belirli sınırlar arasında
büyüklüğe sahip sayıları tutar.tam sayıları kapsadığı için negatif sayıları da kapsar. 
unsigned int değişkenleri pozitif tamsayı tipi ve belirli sınırlar arasında
büyüklüğe sahip sayıları tutar.
char tipi değişkenler, ASCII tipi, örneğin ‘A’, ‘B’ ve ‘C’ gibi karakterleri
tutmakta kullanılır.
float ve double tipi değişkenler, kesirli ve/veya tamsayı tipinden daha geniş sınırlar arasındaki sayıları tutmakta kullanılırlar.
float ile double tipi değişkenler arasındaki fark, tuttukları sayıların değişik
büyüklükte olmasıdır. double tipi değişkenler, float tipi değişkenlerin tuttuğu
sayıların yaklaşık 10 katı büyüklüğündeki sayıları tutabilir.double daha hassas çalışırlar float a göre
Değişkenlerin Tanımlanması
Programda kullanılan değişkenler, aşağıdaki genel formatla tanımlanır.
tip değişken/ler;
Tip, C’de tanımlı olan değişken tiplerinden biri olmalıdır. Aynı tipte tanımlanan değişkenler birden fazla ise, birbirlerinden virgül (,) ile ayrılırlar. Aşağıda, bazı değişken tanımlamaları görülmektedir.
int x, y, z;
short int t;
double j;
Değişkenlerin, programların hangi bölümlerinde tanımlanacağı, ilerleyen konularda
daha ayrıntılı olarak anlatılacaktır. Ancak burada da kısaca değineceğiz. Değişkenler, programın 3 değişik yerinde tanımlanabilir. İlk olarak, programın başında
main() fonksiyondan önce tanımlanabilir. Burada tanımlanan değişkenler
GLOBAL değişken olarak adlandırılırlar ve programda yer alan, main()
fonksiyonu ve diğer fonksiyonlarda da kullanılabilirler. main() fonksiyonu ve diğer
fonksiyonlar içersinde tanımlanan değişkenler ise LOKAL değişkenler olarak
adlandırılır ve sadece tanımlandığı fonksiyon içersinde kullanılabilir.
2. static Tipi Değişkenler
Herhangi bir değişken static tip değiştirici sözcüğü kullanılarak tanımlanırsa,
içinde tanımlandığı fonksiyon ana program tarafından birden fazla çağrıldığında,
her çağrılışında daha önce tuttuğu değeri korur.
static int x;
3. register Tipi Değişkenler
Diğer bir önemli tip değiştirici register olarak adlandırılır ve bu sözcük sadece
int ve char tipi değişkenlere uygulanır. Bir değişken register tipinde
tanımlanırsa bu değişken, RAM bellekte değil, mikroişlemcinin registerinde yer alır.
Bu nedenle register tipinde tanımlanmış değişkenlerin kullanıldığı programlar
diğer programlara göre daha hızlı çalışır. Çünkü registerde bulunan değişkenlere,
bellekte bulunan değişkenlerden daha hızlı ulaşılır.
|  Tip              |SINIRLARI                   |Bellekte alanı|
|-------------------|----------------------------|--------------|
|char               | -128   +127                |   8 bit      |            
| unsigned char     |  0   +255                  |   8 bit      |
|signed char        |-128   +127                 |   8 bit      |
|int                |-32768 +32767 veya          |  16 bit veya |
|                   |-2147483648  +2147483647    |  32 bit      |
|unsigned int       | 0 ... +65535 veya          |  16 bit veya |
|                   |0 ... +4294967294           |  32 bit      |
|signed int         |-32768 ... +32767 veya      |  16 bit veya |       
|                   |-2147483648 ... +2147483647 |  32 bit      |
|short int          |-32768 ... +32767             16 bit       | 
|unsigned short int |   0 ... +65535 16 bit             |
|signed short int   | -32768 ... +32767 16 bit          |
|long int           |-2147483648 ... +2147483647 32 bit |
|signed long int    |-2147483648 ... +2147483647 32 bit |
|unsigned long int  |0 ... +4294967294 32 bit           |
|float              | ±3.4E-38 ... ±3.4E+38 32 bit      |
|double             |±1.7E-308 ... ±1.7E+308 64 bit     |
|long double        |±1.7E-308 ... ±1.7E+308 64 bit veya|
|                    | ±3.4E-4932 ... ±1.1E+4932 80 bit  |                                            
