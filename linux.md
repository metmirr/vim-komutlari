**systemctl**

Linux'de yazdigim servislerden calisanlari listelemek icin:

    $ systemctl | grep running | myservice
  
yukaridaki komut calisan servislerin icerisinden "myservice" kelimesi olan servisleri gosterir.

**scp**

Bir makineden baska bir makineye dosya gondermek veya almak icin kullanilan komuttur.

    $ scp metmirr@1.1.1.1:/home/metmirr/Desktop/names.json Desktop/data/

yukaridaki komut *1.1.1.1* ip adresindeki makineye *metmirr* kullanicisi ile baglanip, */home/metmirr/Desktop/names.json* dizinindeki dosyayi bu komutun yazildigi bilgisayara kopyalar.

**service**

Sisteminizdeki servisleri calistirmak, durdurmak ve durumlarini ogrenmek icin kullanirsiniz:

    $ service mongod status

*mongod* isimli servisin durumunu gosterir.

**rm**

Bir dosyayı veya klasörü silmek için kullanırsınız. Eğer klasör siliyorsanız `rf` seçeneğini de belirtmelisiniz (rf: remove force - silmeye zorla).

    $ rm test.md
    $ rm -rf myfolder

yukarıdaki örneklerden biri dosyayı siler diğeri de klasörü siler. Klasörünüz boş ise klasörü silmek için `rmdir` komutunu da kullanabilirsiniz.

**touch**

Boş bir dosya oluşturmanızı sağlar.

    $ touch example.py
    
**mv**

Bir klasörü taşımak için veya bir dosyayı yeniden isimlendirmek için kullanılabilir.

    $ mv file1 file2

`file1` isimli dosyayı file2 olarak isimlendirir.

    $ mv Desktop/config.json Projects/myapp
    
 `Desktop` dizininde bulunan `config.json` dosyasını `Projects/myapp` dizinine taşır
 
 **mkdir**
 
 Klasör veya klasörler oluşturmak için kullanılır.
 
     $ mkdir myfiles

`myfiles` isminde bir dizin oluşturur

    $ mkdir dir1 dir2

`dir1`, `dir2` isminde iki dizin oluşturur. *mkdir* komutu ile birden fazla dizin oluşturabilirsiniz.

**cp**

Dosyaları veya klasörleri kopyalamanızı sağlar.

    $ cp file1 file2
    
`file1`'i `file2` dosyasına kopyalar; file2 isminde bir dosya mevcut değilse oluşturur ve file1'in içerisiğini kopyalar, eğer dosya varsa sadece içeriği kopyalar.

    $ cp file1 file2 dir1
    
`file1` ve `file2` yi `dir1` isminde bir klasöre kopyalar.

    $ cp file1 dir1 dir2
    
 `file1` ve `dir1`'ı `dir2` isminde bir klasöre kopyalar.

**apt**

Debian tabanlı işletim sistemleri için paket yönetimi aracıdır.

    $ apt update

kurulu olan ve güncellenmesi bulunan paketleri günceller.

    $ apt search {{package_name}}

verilen paket ismi için arama yapar.

    $ apt show {{package}}
    
verilen paket ismindeki paketin bilgilerini görüntüler.

