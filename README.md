# Denge

Pilates, yoga ve kalistenik antrenman uygulaması. Telefona kurulabilir web uygulaması (PWA); ilk açılıştan sonra internetsiz çalışır.

**Uygulama adresi:** https://tirsphone.github.io/denge/

## Telefona kurulum
- **iPhone:** Safari'de adresi aç → Paylaş → Ana Ekrana Ekle.
- **Android:** Chrome'da adresi aç → ⋮ → Uygulamayı yükle.

## Güncellemeler
Uygulama claude.ai'deki "Denge" artifact'ı ile birlikte geliştirilir.
Her güncellemede artifact'ın HTML'i bu depoya `index.html` olarak, PWA başlığı (manifest, simgeler, service worker kaydı) eklenerek yüklenir ve `sw.js` içindeki sürüm etiketi değiştirilir.
Uygulama internet varken her açılışta yeni `index.html`'i alır; telefonda ayrıca bir şey yapmak gerekmez.

Veriler yalnızca telefonun tarayıcı deposunda tutulur; bu depoda kişisel veri yoktur.
