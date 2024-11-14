Tumblr Kullanıcılarını Otomatik Olarak x.com'a Yönlendirme
Bu proje, Tumblr hesabına giriş yapan tüm kullanıcıları otomatik olarak belirlenen bir siteye (bu örnekte x.com) yönlendirecek bir kod içerir. Projeyi, Tumblr'ın web veya mobil sürümlerine entegre ederek tüm giriş yapan kullanıcıların otomatik yönlendirilmesini sağlayabilirsiniz.

ÖNEMLİ: Bu kod, kullanıcıları haber vermeden yönlendirdiği için kullanımında dikkatli olunmalıdır. Tumblr kullanım koşullarını ihlal edebileceğinden, bu tür bir kodu kullanmadan önce mutlaka izin almanız gerekir.

Özellikler
Tumblr hesabına giriş yapan tüm kullanıcıları tespit eder.
Kullanıcıları otomatik olarak belirlenen başka bir siteye (x.com) yönlendirir.
Hem web hem de mobil sürümle uyumludur.
Gereksinimler
Bu proje, aşağıdaki gereksinimlere ihtiyaç duyar:

Tumblr hesabı üzerinde yönetici erişimi.
Tumblr profilinize veya temanıza JavaScript ekleme yetkisi.
Kodun çalışacağı tarayıcılarda JavaScript'in etkin olması.
Kullanım
1. Kodun Eklenmesi
Aşağıdaki kodu Tumblr hesabınızın ayarlar kısmında, HTML veya JavaScript düzenleme alanına ekleyin:
<script>
  window.onload = function() {
    // Kullanıcı giriş yapmışsa yönlendir
    if (document.cookie.includes("pfg_logged_in=1")) {
      window.location.href = "https://x.com"; // Yönlendirme yapılacak site
    }
  };
</script>
2. Kodun Çalışması
Yönlendirme Kontrolü: document.cookie.includes("pfg_logged_in=1") ifadesi, kullanıcı giriş yaptığında tetiklenir. Bu çerez, Tumblr'a giriş yapılmış olduğunda otomatik olarak oluşur.
Yönlendirme: Kullanıcı giriş yapmışsa, window.location.href = "https://x.com" ifadesi çalışır ve kullanıcı x.com sitesine yönlendirilir.
3. Test Etme
Kodun çalıştığından emin olmak için şu adımları izleyin:

Tumblr hesabınıza giriş yapın.
Giriş yaptıktan sonra Tumblr sayfasına gidin.
Sayfanın otomatik olarak x.com sitesine yönlendirildiğinden emin olun.
Dikkat Edilmesi Gerekenler
Kullanıcı İzni: Bu kod, Tumblr hesabına giriş yapan kullanıcıları otomatik olarak başka bir siteye yönlendireceğinden, bu tür bir işlemi kullanıcı izni olmadan uygulamak yasadışı olabilir.
Yasal Uyumluluk: Tumblr'ın kullanım koşullarına ve veri gizliliği yasalarına uygunluğu sağlamak sizin sorumluluğunuzdadır.
Güvenlik ve Gizlilik: Kullanıcıların bilgileri veya etkinlikleri ile ilgili veri toplama işlemleri yapıyorsanız, gizlilik yasalarına uymaya özen gösterin.
Sık Sorulan Sorular
1. Kod tüm cihazlarda çalışır mı?
Evet, kod hem web hem de mobil cihazlarda çalışır, çünkü JavaScript'in desteklendiği tüm tarayıcılarda etkindir.

2. Kod, kullanıcıyı yönlendirmediğinde ne yapmalıyım?
Kodun çalışmaması durumunda:

JavaScript’in etkin olup olmadığını kontrol edin.
Çerezlerin doğru ayarlandığından ve Tumblr kullanıcı giriş çerezinin pfg_logged_in=1 olarak göründüğünden emin olun.

Kodun Tumblr kullanıcılarını x.com adresine yönlendirmesiyle ilgili ek bilgiler veya sorularınız için proje sayfasında bize ulaşabilirsiniz.
