Git Branch Nedir?
Git Branch dallar arasında gezinmemizi sağlar burada yeni dal oluşturmak için git branch 'Yeni Dal İsmi' 
Branch sayesinde ana projeden koparak üzerinde oynamalar yapabiliriz bu sayede ana projeye zarar verilmemiş olur biz de dilediğimiz gibi proje üzerinde oynamalar yaparak ilerleyebiliriz. 
Diyelim ki evet ana projenin üzerine bir sürü şey ektik ve projeyi büyüttük veya bizden istenilenleri yaptık işte şimdi merge zamanı.

Git Merge Nedir? 
Git Merge oluşturulan veya varolan dalları birleştirmeye yarar evet branch ile ayrı bir dala geçtik üzerinde uğraştık ve eskisinden yeni gıcır gıcır bir proje oldu çok iyi! İşte bunu birleştirerek ana proje haline getirmeye daha doğrusu ana proje branchini değiştirmeye merge denir. bu işlem için öncelikle ana proje branchine geçerek git merge 'Ana Projeye Eklenecek Branch Adı' şeklinde yapmamız gerekir ama dikkat! Merge ettiktten sonra Yeni oluşturulmuş ve ana projeye dahil edilmiş branch içerikleri silinecektir. Daha sıkıntı yaşatabilecek şey ise Yan dalda değiştirilen ve aynı satıra gelen iki farklı kod merge edildiğinde çakışır yani birini tercih et ana dala o kodları yazayım der burada kod editörünüzde Head(Yani Şu An Üzerinde Bulunduğunuz Branch) ve altta da 'Merge Etmek istediğiniz Branch Adı' birisini silmeli ve Commit işlemi yapmalısınız bu durumda çakışma sorunları ortadan kalkacaktır!

Git Ignore Nedir?
Git Ignore bazı dosyaların commit ederken takip edilmesinin önüne geçmek için oluşturulan gitignore uzantılı bir dosyadır bu dosyanın içerisine yazılan dosya adları (uzantısıyla) takip edilmeyecektir yani commit ederken veya status kontrolünde ele alınmayacak görünmeyecektir.

Git Remote Neidr? 
Git Remote branchin önceki haline getirmek için kullanılan bir yöntemdir eğer başka bir branchda çalışırken bir anda Commit etmeden ana branche geçtiğimizde yan branchda yazdığımız kodlar ana brancha geçecek ve büyük bir soruna davet çıkaracaktır ama ana brancha geçtiğimizde ##"git remote add" dersek bu durumda ana branch eski formuna dönecektir ancak yan dalda yazdığımız kodların hepsi de uçacaktır. Bunu önlemek için stash kullanmak durumunda kalabiliriz.

Git Stash Nedir? 
Git Stash yazılan kodları yani remote ile önceki sürüme çekmeye çalıştığımız kodlar elimde kalsın bunları yan branchda kullanmaya ve takip etmeye üzerinde çalışmaya devam edeyim dediğimiz durumlarda veya veriler indexlensin kaybolmasın sonrasında istediğim zaman çekerek üzerinde çalışayım dediğimiz durumlarda kullanılır. ##git stash dediğimizde bizim yazmış olduğumuz 