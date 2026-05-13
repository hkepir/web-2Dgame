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


