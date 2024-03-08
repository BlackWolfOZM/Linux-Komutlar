# Linux-Komutlar
Disk boyutu öğrenme
Disk boyutunu öğrenmek için df komutu h parametresi kullanılır.

df -h
Ram kullanımı öğrenme
Ram kullanımını öğrenmek için free komutu h parametresi kullanılır.

df -h
Açılış zamanını öğrenme
Sistemin açılış zamanından itibaren geçen zamanı, işlemci kullanımı bilgilerini öğrenmek için uptime komutu kullanılır.

uptime
Çalışılan dizini öğrenme
İçerisinde bulunan dizini öğrenmek için pwd komutu kullanılır.

pwd
Aktif kullanıcıyı öğrenme
Mevcut kullanıcıyı öğrenmek için whoami, id veya logname komutu kullanılır.

whoami
logname
id
Belirli bir kullanıcı bilgisini almak için parametre olarak kullanıcı adı yazılabilir.

id root
Sistem bilgilerini öğrenme
Sistem bilgilerini öğrenmek için uname komutu a parametresiyle kullanılır.

uname -a
Sistemdeki bios, ram vb. parçaların detaylı bilgisini almak için dmidecode komutu kullanılır.

dmidecode
Sistem adını almak
Sistem adını almak için hostname komutu kullanılır.

hostname
Sistem açılış bilgisini almak
Sistemin son olarak başlatıldığı veya yeniden başlatıldığı bilgisini almak için last komutu kullanılır.

last
Sistem olay bilgisini almak
Sistem ile ilgili açılıştan itibaren uyarı, hata vb. bilgileri almak için dmesg komutu kullanılır.

dmesg
Aktif kullanıcıları listeleme
Aktif kullanıcıları listelemek için w veya who komutu kullanılır.

who
w
Zaman bilgisini öğrenme
Zaman bilgisini öğrenmek için date takvim bilgisi için cal komutu kullanılır.

date
cal
Takvimi yıla göre listelemek için yılın parametre olarak verilmesi yeterli olacaktır.

cal 1453
Takvim bilgisini 3 aylık almak için 3, yıllık almak için y parametresi kullanılır.

cal -3
cal -y
Dosya bilgisini almak
Dosya bilgisini almak için file komutu kullanılır.

file /etc/passwd
İşlemci bilgisini almak
İşlemci bilgisini almak için lscpu komutu kullanılır.

lscpu
Yüklü modülleri listelemek
Yüklü modülleri listelemek için lsmod komutu kullanılır.

lscpu
Dağıtım bilgisini almak
Dağıtım bilgisini almak, dağıtıma göre değişiklik gösterir.

Debian tabanlı dağıtım bilgisini almak için lsb_release komutu a parametresiyle kullanılır.

release -a
Red Hat tabanlı dağıtım bilgisini almak için lsb_hostnamectl komutu kullanılır.

hostnamectl
Red Hat tabanlı işletim sistemlerinde ayrıca /etc dizinindeki release dosyalarına bakarakta öğrenilebilir.

cat /etc/*release*
Ayrıca /proc dizinindeki version dosyasına da bakılabilir.

cat /proc/version
Yüklü modülleri listelemek için lsmod komutu kullanılır.

lscpu
Ortam değişkenlerini listeleme
Tanımlı sistem değişkenlerini listelemek için env komutu kullanılır.

env



Screen Kullanımı 
sudo apt-get install screen  #kurulum

screen --version    #version

screen                         #Screen üzerinde yeni bir konsol açmak için;

screen -S "oturum_ismi"        #Screen komutunu girdiğiniz anda, terminal üzerinde sanal olarak bir tane daha oturum açılır ve artık yeni oturumda işlemlerinizi yaparsınız. -S parametresi ile beraber, yeni bir oturum açılır ve oturuma isim verilir.

ctrl+a+d                       #Ana ekrana dönmek için;

screen -xS oturum_ismi         #Açtığınız oturuma tekrar dönmeniz için;

screen -r  oturum ismi        #tekrar bağlantı

screen -X -S oturum ismi kill or quit  #kapatma silme

Bunun dışında, normal Linux konsolunda CTRL +D ile logout olabilirsiniz.

screen -list veya screen -ls    #Screen ile açılmış oturumları görmek için aşağıdaki komut kullanılır.

screen -a -r 20358              #Daha önceden oluşturduğumuz screen oturumuna bağlanmak için screen -list komutundan aldığımız screen id si ile aynı oturuma tekrar bağlanabiliriz. Bunun için ise aşağıdaki komut kullanılmaktadır.

CTRL + a + n : Bir sonraki oturuma bağlanır.
CTRL + a + p : Bir önceki oturuma geri döner.    #Oturumlar arasında geçmek için,


screen -wipe      #Öldürülen screen alanlarını listeden kaldırmak için aşağıdaki gibi screen komutuna seçenek olarak “-wipe” kullanabilirsiniz.




