# Güvenlik

## Bir açık buldunuz mu?

Lütfen herkese açık bir issue **açmayın**. Bunun yerine GitHub'ın özel bildirim özelliğini kullanın: deponun **Security** sekmesi → **Report a vulnerability**. Bildirim yalnızca depo sahibine görünür.

## Bu projede alınan önlemler

- **Gizli anahtarlar depoda yok.** `.env`, anahtar ve sertifika dosyaları `.gitignore` ile dışarıda tutulur. GitHub secret scanning ve push protection açıktır; yanlışlıkla anahtar yüklemek engellenir.
- Bu depo yalnızca statik dosyalardan oluşur; sunucu ya da veritabanı sırrı içermez.
- Bağımlılıklar için Dependabot uyarıları açıktır.
