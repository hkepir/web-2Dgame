* AI Prompt
**Kullanilan promptlar
1) "Kütüphane kullanmadan, saf JavaScript ve HTML5 Canvas kullanarak fizik mekanizmaları gerektiren oyun nasıl yapılabilir?"
 ---
2) "Blueprint Bob gibi bir oyun yapmak istiyorum. Bir inşa aşaması (Blueprint Mode) ve bir de platform aşaması (Real Mode) olan bir oyun mu tasarlamalıyım?"
---
3)	"Oyunun fizik motoru için bize gereken temel yapıtaşları şunlar: Koordinatları hafızada tutan bir fonksiyon, kullanıcı ve obje hareketlerini kontrol eden bir fonksiyon, objelerin birbiriyle temasını algılayacak bir çarpışma fonksiyonu, kulenin yıkılıp yıkılmayacağını hesaplayacak bir denge kontrol fonksiyonu, temel mekanik hesaplamalarını yapan bir fonksiyon ve her şeklin düşmesini belirleyen bir fonksiyon. Bu modüllere ek olarak sence sağlam bir fizik motoru için başka nelere ihtiyacımız var?"
---
4)	"Bizim geliştirmek istediğimiz bu 2D denge oyununun fizik motoru için hangi temel fonksiyonlara ihtiyacımız olduğunu söyler misin? Amacım o videolardaki kodları doğrudan almak yerine, bu fonksiyonların arkasındaki mantığı öğrenmek ve kendi sistemimizi adım adım yazmak."
---
5)	"Şu ana kadar nesnelerin temel hareketlerini ve birbirlerine değip değmediklerini kurguladık. Peki, daha önce konuştuğumuz detaylara ve sana gönderdiğim eğitim videolarındaki kaynaklara dayanarak, bu fizik motoruna başka neler ekleyebiliriz? Örneğin, objelerin çarpıştıklarında birbirlerine gerçekçi bir şekilde hız ve enerji gibi etkileşimleri profesyonel bir seviyeye taşıyacak hangi fonksiyonlara ihtiyacımız var?"
---
6) "Collision detection nedir? Bloklar iç içe geçmeden çarpışabilir mi?"
---
7)	"Testler sırasında blokların ara sıra birbirinin içine geçtiğini ve sonrasında uçmaya başlıyorlar. Ben blokların bu şekilde hatalı davranışlarını değil, sadece oluşan doğal dengesizliklerinden ötürü gerçekçi bir şekilde devrilmelerini istiyorum. Bu iç içe geçme ve patlama döngüsünü kırmak için fizik motorundaki ayrışma değerlerini normalde olması gerektiği gibi nasıl güncelleyebiliriz?"
---
8) "Blokların birbirini gereksiz yere fırlatmasını (pop etkisi) engellemek için itme kuvvetlerini (impulse) optimize et."
---
9)	"Bloklardaki titreme sorununu profesyonelce çözmek için matter-js/examples/mixed.js at master · liabru/matter-js linkindeki kaynak kodlarınını inceledim. Bu kütüphanenin fizik hesaplamalarından ve mimarisini kullanarak, bizim sistemimize entegre edebileceğimiz kodlar veya algoritmalar çıkarabilir miyiz? Özellikle bu profesyonel motorların objeleri dengede tutmak için kullanılan yöntemleri kendi kodumuza uyarlamak istiyorum. "
---
10)	"Fizik dünyasına blok eklerken yaşadığımız fırlama sorunlarını çözmek için sana xi/trickytowers build.js dosyasının GitHub linkini incelemeni istiyorum.? Bu tarz kule dizme oyunlarında blokların düşme, birbirleriyle olan etkileşimlerinin nasıl olduğunu öğrenmek ve oradaki mantığı kendi oyunumuza uyarlamak istiyorum."
---
11)	"Oyunun şu anki güncel kodu (index4.html) ekte yer alıyor. Senden isteğim, az önce GitHub üzerinden incelediğimiz yaklaşımları doğrudan bu koda nasıl entegre edileceğini göstermen. Özellikle blokların ağırlık merkezini doğru hesaplayarak o pervane gibi dönüp fırlama sorununu kalıcı olarak nasıl çözebiliriz?"
---
12)
<img width="499" height="464" alt="image" src="https://github.com/user-attachments/assets/da0f4487-015d-4547-a324-51677040159e" />

"Görseldeki blokların bu şekilde havada asılı kalması gerçek fizik kurallarına aykırı, bu denge sorununu düzeltmeliyiz. Ayrıca karakter kontrollerinde bir hata var; sadece sağ-sol tuşlarıyla yürümüyor."

---

13)
<img width="534" height="458" alt="image" src="https://github.com/user-attachments/assets/2849d907-315f-457f-a4d3-793aca52e135" />

"Görseldeki fizik kurallarına aykırı o asılı kalma durumunu düzeltelim ve dengeyi gerçek hayattaki gibi yapmayı deneyelim. Ayrıca karakter kontrollerinde hala bir sorun var; Karakter şekilleri duvar olarak görmüyor, içlerinden geçip gidiyor."

---
14)"Karakterin yönüne göre görseli aynala (flip effect). Sağa giderken sağa, sola giderken sola baksın."

---
15) "Bu oyunların nasıl yapıldığı hakkında bilgi veren bir kaynak ya da açık kodlu yazılımlar var mı"
    
---
16) "Bu oyunu mobilde çalışması için nasıl bir yol izlemeliyiz?"

---
17) "Kullanıcıdan belirli bir süre içerisinde istediği mimariyi yapmasını isteyeceğiz. Nasıl yapabiliriz?"

---
18) "Oyun ilk açıldığında oyuncuyu doğrudan menüye atmak istemiyoruz. Bize 5-6 saniye boyunca ekranda kalacak, oyunun adının ve yükleme animasyonlarının olacağı bir giriş sayfası yapmak istiyoruz. Süre bitince otomatik olarak bizim hazırladığımız ana menüye geçmesi gerekiyor. Nasıl yapabiliriz?"

---
19) <img width="528" height="385" alt="image" src="https://github.com/user-attachments/assets/12b3d53e-a960-4662-8e10-0da89ca457ae" />

 Oyun moduna geçtiğimizde ekrandaki bu rastgele blok dağılımını kod tarafında oluşturacağımız fonksiyonlarla algoritmik olarak nasıl sağlayabiliriz? Her seferinde farklı boyut ve tiplerde objeler üretecek o mimariyi nasıl kurmalıyız? 

20) "[Blueprint Bob](https://suumpmolk.itch.io/blueprint-bob) oyunundan esinlendiğimiz ama Tetris mekaniklerini de barındıran bir oyun tasarlamak istiyorum. Oynanış akışı şöyle olacak: Önce kullanıcı 3 kareden oluşan kendi şeklini çizecek. Şekil tamamlanınca bir tuşa basacak ve şekil hareket ederken zemin zıt yöne kayacak, oyuncu zamanlamayı ayarlayıp şekli bırakacak. Kullanıcı bu şekilde kuleyi dizecek. İnşa bitip onay tuşuna basıldığında fizik kuralları devreye girecek ve kule yerçekimiyle baş başa kalacak. Son aşamada ise karakterimiz sahneye girip bu kulenin en üstündeki hedef çizgisini geçmeye çalışacak. Eğer karakter yukarıda 3 saniye devrilmeden durabilirse bölüm geçilmiş sayılacak. Bu mekaniği nasıl kodlarız?"

21) "Referans aldığımız oyunundaki gibi bir yapı kurmak istiyorum. Çizdiğimiz şekiller 3 yerine 4 kareden de oluşabilir, buna sonra karar veririz ama kesinlikle kullanıcının kendi şeklini çizmesini istiyorum. Zemin ve şekil zıt yönlere hareket ederken kullanıcı bunları üst üste dizecek. Ancak şu anki kodda oluşan parçalar oyun moduna girince birbirinden kopup dağılıyor. Ben kullanıcının çizdiği o bütün şeklin tek parça halinde kalmasını istiyorum. Eğer kule dengedeyse şekil bütün olarak dengede kalsın, denge bozulursa da parçalanmadan tek bir blok halinde devrilmesi gerekiyor. Nasıl yapılabilir?"

22) "Ben bu oyunda enter'a bastıktan sonra grid mantığını bırakmasını ve gerçek dünyada nasıl davranması gerekiyorsa o şekilde davranmasını istiyorum. Şekili yerleştirmek isterken grid mantığını nasıl bırakabiliriz?"  


