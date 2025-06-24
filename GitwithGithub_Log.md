## 🚀 Projeyi GitHub'a Gönderme Rehberi

## ✅ Terminali aç ve Git başlat:  
git init

## 📦 Tüm dosyaları Git takibine al: 
git add .

## 📝 İlk commit'i oluştur:
git commit -m "İlk commit"

## 🌐 GitHub’da boş bir repo oluştur (README ekleme!) ve uzak bağlantıyı ekle:
git remote add origin https://github.com/KULLANICIADINIZ/REPO-ADI.git

## 🌿 Ana branch’i “main” olarak ayarla:
git branch -M main

## 🚀 Projeyi GitHub'a gönder (push):
git push -u origin main

## 🔁 Her yeni değişiklikte şu üç adımı tekrar et:

git add .
git commit -m "Açıklama"
git push
## 🛑 Notlar:

node_modules, dist gibi klasörleri .gitignore içine eklemeyi unutma.

Git boş klasörleri takip etmez. Takip etmek istersen içine .gitkeep koy.

Terminali temizlemek için:

Windows: cls

macOS / Linux / PowerShell: clear