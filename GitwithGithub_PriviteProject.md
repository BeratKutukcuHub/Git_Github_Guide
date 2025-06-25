### GitHub'a Repository Nasıl Gönderilir Rehberi : 

- Öncelikle GitHub'da bir repository oluştur ve vermiş olduğu HTTP adresini kopyala.

- Gönderilecek dosyaya git ile ulaş ve ardından ##git init (Git Yükle) , ##git add (Gönderilecek Dosyaları Belirle) , ##git commit -m "Açıklama" (Dosyaları takip et ve süreci kaydet) ardından ##git remote add origin "HTTP adresi" (Gönderilecek adrese bağlan) ve ##git push (Gönder)

- Bu işlemler sonrası Repositoryde dosyaların oluşmuş olacaktır.

### Böyle Sorunlar Olabilir

+ İsteğiniz gerçekleşti ve istenilen brancha dahil edildi bu gibi sebeplerden ötürü şöyle bir durum da mevcut.

  + Sizin lokalinizde yazmış olduğunuz kodlar geride kalmış olabilir bu nedenle pull request kabul edildikten sonra commitleri takip etmemiz gerekmektedir bu ne demektir? 

    - Ana sunucuda kabul gören pull request branche dahil edilir ve proje büyümüş olabilir bunu önlemek için ##git checkout origin/"dahil edilen branch" 'e bağlanarak ##git fetch ile güncellememiz gerekmekte böylelikle son commitleri ana sunucudan çekebiliriz. Ancak bu geçiçi bir 'branch' olduğundan dolayı commit, push gibi eylemler yapamayız sadece 'readonly' görebiliriz. Kendi lokalimize checkout/switch attığımızda güncel commitleri tekrar göremeyiz çünkü lokaldeyiz.

    - Ama diyorsak ki kendi lokalimizde de güncel commit üzerinde çalışmak istiyoruz yani commitleri kendi lokalimizde görelim o kodlar tam olarak ekranımda yazsın güncel şekilde takip edeyim diyorsanız! ##git pull işlemini yapmamız gerekmektedir