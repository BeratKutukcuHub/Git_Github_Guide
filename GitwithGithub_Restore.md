### Git Restore Nedir?
Git Restore komutu eğer bir dosya seçersek yani ##git restore "Dosya Adı" durumunda önceki haline getirecektir dosyayı yani son commit haline dönecektir ancak ##git restore dersek tüm proje önceki komut haline dönecektir çok dikkat edilmesi gerekmektedir eğer ki böyle bir şey yapacaksak ##git slash ile commit öncesi dosyaları kaydedersek kurtarma şansımız olacaktır ##git slash pop ile son commitleri tekrar projemize getirebiliriz.

### Git Checkout Nedir?
Git Checkout komutu istenilen commitler arasında dolaşmamıza yarar bunun için commit'in unique kodunu kopyalayarak yapıştırmak yeterli olacaktır ##git log ==> commit listesinden istenilen commit'in unique kodunu kopyala ve ##git checkout "unique kodu yapıştır" ve o commite dönerek işlemlere devam edebilirsin bu sayede bir çok sorunu revize etmek yerine daha temiz bir kod inşaa edebilirsin.
Dikkat! Bu işlemden sonrasında branch'dan bağı kopartırız ve sadece başıboş şekilde geçmişte oluruz. Bunun için de yeni bir branch oluşturulup ana branche sonradan merge edebiliriz! bunun için ==> ##git branch "X(Konmak İstenen Branch Adı)" ve sonrasında ##git switch "X" şeklinde branche geçerek çektiğimiz commiti bu branche kaydedebiliriz ve devamında merge ederek bu branchı ana branch edebiliriz.

### Git Reset Nedir? 
Git Reset komutu Checkout gibidir ancak! bu komutu kullandığımızda head yani üzerinde olduğumuz branchten kopmayız ve istediğimiz commite dönebiliriz evet ama bu döndüğümüz comitten sonra atılmış olan commitler atlanır yani 2 adet commitimiz var 1. Adı İlk Commit 2. Adı İkinci Commit ve son atılmış commit de 2. Commit olsun. Bu durumda biz 1. Commite dönersek! 2. Commit silinecektir ve 1. Committen kodlamaya devam edebileceğiz ancak 2. committeki kodlar bu committe gözükecektir ve bu durumda bulunduğumuz branchden kopmayacağız. ##git reset "Commit unique kodu" şeklinde çalıştırarak geri dönebiliriz.
!! Dikkat eğer diğer commitler değersizse ve silinmek istiyorsa ve 1. commite tam anlamıyla dönülmek isteniyorsa ##git reset --hard "Unique Commit" şeklinde yaparız bu durumda bulunmak istediğimiz committen sonra atılan commitler ve içerisindeki bulunan kodlar silinecektir.

### Git Revert Nedir?
Git Revert komutu ##git reset ile aynı mantıktadır ancak! burada doğrudan 2. commite geçilir branchdan kopmayız ve bunun yanında diğer sonradan atılan commitler de silinmez. Burada işlemlere devam edebilir ayrı bir branche geçebilir buradan da merge edebiliriz. Ancak bu durumda direkt istenilen committeki bilgiler gelecektir son committe yapılan bilgiler size gelmeyecektir doğrudan o committe ne bilgiler, kodlar varsa onları görebileceksiniz aslında bulunduğumuz committen geçmise doğrudan gider ve orada bulunuruz ama diğer committeki bilgiler, kodlara zarar gelmez ama ilişiğimizi keseriz. Kullanımı => ##git revert "Unique Commit"

### Git Diff Nedir?
Git Diff komutu branchler, commitler, kaydedilen dosyalar gibi neredeyse her şeyi kıyaslamaya yarayan bir komuttur geçmişte yapılanlar ile şimdi yapılmış olan işlemleri birbiriyle kıyaslayarak ne tür değişimler olduğunu gözlemlememize olanak sağlar. Bu işlem geçmiş commite dönmeden görmek için. Silmiş olduğuna bakmak için dönüp görmek için vs. her türlü kontrolü sağlamamıza olanak sağlayan komuttur.
=>> ##git diff "İstenilen Branch" "Diğer Branch",
=>> ##git diff "Commit".."Diğer Commit" (arasına '..' konulur)

