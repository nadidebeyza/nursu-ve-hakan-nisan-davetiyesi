# GitHub Pages Kurulum Talimatları

## Sorun
GitHub Pages Jekyll kullanmaya çalışıyor ama proje statik HTML/CSS/JS.

## Çözüm 1: GitHub Pages Ayarlarını Değiştir (ÖNERİLEN)

1. GitHub repository'nize gidin
2. Settings > Pages bölümüne gidin
3. "Source" kısmında "Deploy from a branch" seçin
4. Branch: "main" (veya "master")
5. Folder: "/ (root)" seçin (docs değil!)
6. Save'e tıklayın

Bu şekilde root klasöründeki dosyalar kullanılacak ve Jekyll devre dışı kalacak.

## Çözüm 2: Docs Klasörünü Kullanmaya Devam Et

Eğer docs klasörünü kullanmak istiyorsanız:
- Tüm dosyalar zaten docs/ klasöründe
- .nojekyll dosyası docs/ klasöründe
- _config.yml dosyası oluşturuldu

Ancak GitHub Pages hala Jekyll build yapmaya çalışıyor. 
Bu durumda GitHub Pages ayarlarında "Source" olarak "root" seçmek daha iyi.
