Kelimeye Göre 301 Yönlendirme - index.php

Bu proje, belirli anahtar kelimelere göre 301 yönlendirmesi yapan basit bir PHP dosyasıdır. Web sitenize gelen trafiği, belirli kelimeler içeren URL'lere göre otomatik olarak yönlendirmek için kullanabilirsiniz.

Nasıl Çalışır?
index.php dosyası, URL'deki belirli anahtar kelimeleri kontrol eder. Eğer tanımlı bir kelimeyle eşleşme sağlanırsa, kullanıcıyı belirtilen yeni URL'ye 301 yönlendirme yöntemi ile yönlendirir. Bu özellik, arama motoru optimizasyonu (SEO) için faydalı bir çözüm sunar.

Özellikler
Anahtar Kelimelere Göre Dinamik Yönlendirme: URL içinde tanımlı anahtar kelimelerle eşleştiğinde çalışır.
SEO Dostu 301 Yönlendirmeler: Kalıcı yönlendirme yaparak SEO açısından fayda sağlar.
Kolay Yapılandırma: Hedef URL'leri ve anahtar kelimeleri yapılandırmak kolaydır.
Hafif ve Verimli: Düşük maliyetli ve performans dostu bir çözüm sunar.
Kullanım
1. index.php Dosyasını Yükleme
Proje dizininizin kök klasörüne index.php dosyasını ekleyin.

2. Yönlendirmeleri Tanımlama
index.php dosyasının içinde, yönlendirme yapılacak anahtar kelimeleri ve hedef URL'leri $redirects dizisi içinde tanımlayın.

Açıklamalar:
Anahtar Kelime: eski-kelime ve ornek-kelime gibi anahtar kelimeler, URL içinde kontrol edilecek ifadelerdir.
Yönlendirme URL'si: Anahtar kelime URL içinde bulunduğunda kullanıcıyı yönlendirecek olan URL (https://yeni-url.com gibi).
3. Çalıştırma
Web sitenize gelen bir istek belirli bir anahtar kelime içeriyorsa, ziyaretçi otomatik olarak yapılandırılmış yeni URL'ye yönlendirilir.
301 kalıcı yönlendirme kullanılarak SEO uyumlu bir şekilde yönlendirme yapılır.
Örnek Kullanım Senaryosu
Örneğin, https://siteniz.com/eski-kelime URL'sine gelen bir ziyaretçi, https://yeni-url.com adresine yönlendirilecektir.

Notlar:
Dikkat: strpos işlevi, anahtar kelimenin büyük/küçük harf duyarlı olduğunu unutmayın.
301 Yönlendirme: Yönlendirmeler 301 statü koduyla yapılır, bu kalıcı yönlendirmeler SEO'ya uygun olarak tercih edilmiştir.
