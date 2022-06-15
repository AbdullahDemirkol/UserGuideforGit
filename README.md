# Guide To Using Git (Git için Kullanma Kılavuzu)

"git" komutu bize git help dökümantasyonu getirir.
![git-command]()

"git --version" komutu bize gitin versiyonunu getirir.
![git-version-command]()

"git config --global user.name "kullanıcı adı" " komutu ile kullanıcı adı kaydediyoruz.
"git config user.name" komutu ile de koyduğumuz kullanıcı adını görebiliyoruz.
![git-username-command]()

"git config --global user.email "email adresi" " komutu ile email adresini kaydediyoruz.
"git config user.email" komutu ile de koyduğumuz email adresini görebiliyoruz.
![git-email-command]()

"git status" komutu gitin durumu gösterir.
Eğer klasörün herhangi bir repository ile bağlantısı yok ise bu durumda "git init" komutunu kullanıyoruz.
![git-status-and-git-init-command]()

"git add dosya adi" komutu o dosyayı kommitlemeye hazırlar.
"git add ." komutu bütün dosyaları kommitlemeye hazırlar.
![git-add-command]()

"git commit -m "yorum" " komutu kommite yorum ekler ve her kommite bir hash değeri atar.
![git-commit-command]()

"git log" komutu ile kommitimizin kayıtları gösterir.
![git-log-command]()

"git add ." komutu ile ekleme yaparken diyelim bir dosyayı eklemek istemiyoruz. Böyle bir durumda ilk olarak yapılıcak şey ".gitignore" isimli bir dosya oluşturuyoruz. Bundan sonra eklenmek istemeyen dosyayının ismini ".gitignore" dosyasının içine yazıyoruz. Sonra işlemimize devam ediyoruz ve eklenmek istemeyen dosya eklenmemiş oluyor.
gitignore template ile tarayıcıda bir arama yaparsak önümüze örnek gitignore klasörleri çıkıcaktır. Bizde kendi yazdığım dile uygun olanı alıp kendimize göre uygulayabiliriz.
![git-ignore-file]()

"git branch branchadi" komutu ile yeni bir branch açabiliriz.
![git-branch]()
![git-branch-command]()

"git switch master" komutu ile headimizi master'a taşıyoruz.
![git-switch]()
![git-switch-command]()

"git merge branchadi" komutu bulunduğumuz branch ile yazdığımız branchadi  Bu bize branchadi ve bulunduğumuz branchi birleştiriyoruz.
![git-merge]()
![git-merge-command]()
![git-merge-command2]()
![git-merge-command3]()

Eğer ana branchde hiçbirşey yapmayıp yeni bir branchden ilerleyip ana branchle yeni branchi merge edersek bu işleme "Fast Forwarding" denir.
![fast-forwarding]()
![fast-forwarding2]()
![fast-forwarding-command]()

"git checkout hashdegeri" komutu yardımıyla istediğimiz git loguna dönüş yapabiliriz. Geri gittiğimiz yerden devam etmek istiyosak yeni bir branch oluşturup devam edebiliriz.
![git-checkout]()
![git-checkout2]()
![git-checkout3]()
![git-checkout-command]()

"git reset hashdegeri" komutu bizim verdiğimiz hash değeri kommitine gider fakat değişiklikleri silmez. Tekrardan kaydetme komutlarıyla yaptığımız değişiklikleri kaydedebiliriz.
![git-reset-command]()

"git reset --hard hashdegeri" komutu bizim verdiğimiz hash değeri kommitine gider ve değişiklikleri silip o hash değerinde kommitin aynısına dönmüş olur.
![git-reset-hard]()
![git-reset-hard-command]()

"git revert hashdegeri" komutu bizim verdiğimiz hash değerinin kommitini geri alır fakat yeni bir kommit ekleyerek bu işlemi yapar. Yani reset gibi hikayeyi geri sarmaz.
![git-revert]()
![git-revert-command]()

"git diff" komutu bizim yaptığımız değişiklikleri gösterir.
![git-diff-command]()

"git diff HEAD" komutu bizim yaptığımız değişikliklerle HEAD'in bulunduğu kommitin değişikliklerini karşılaştırır.
![git-diff-head-command]()

"git diff hashdegeri hashdegeri2" komutu vermiş olduğumuz hash değerleri arasındaki farkları karşılaştırır.
![git-diff-hashdegeri-command]()

"git diff branch1 branch2" komutu branchler arasındaki farkı gösterir.
![git-dif-branch-command]()

"git rebase branchadi" komutu hikaye örgüsünü düzeltmemize yarar. Fakat bu komutu eğer sizin branchinizi kullanan kimse yok ise uygulayın aksi halde çok büyük sorunlar ortaya çıkabilir.
![git-rebase]()
![git-rebase-command]()
![git-rebase-command2]()

## Merge Conflict
Bir örnek üzerinde inceleyip sorunu çözelim. 
İlk adım bir java dosyasına email adresimizi kaydediyoruz.
![Merge-conflict]()

İkinci adım yeni bir branch açıyoruz.
![Merge-conflict2]()

Üçüncü adım yeni branchin içinde kayıtlı email adresini değiştirip kaydediyoruz.
![Merge-conflict3]()
![Merge-conflict4]()

Dördüncü adım olarak master branchimize geçiyoruz ve email adresini silip kaydediyoruz.
![Merge-conflict5]()
![Merge-conflict6]()
![Merge-conflict7]()

Beşinci adım master branchi ile diğer branchi merge etmeye çalışıyoruz. Fakat hata veriyor ve bize birini seçmemiz gerektiğini belirtiyor.
![Merge-conflict8]()
![Merge-conflict9]()

Altıncı adım ise birini seçip kaydediyoruz ve merge conflict sorununu çözmüş oluyoruz.
![Merge-conflict10]()
![Merge-conflict11]()

## Git Stash
Başka bir branchdeyken yaptığımız değişikliği kommitlicek kadar emin olmadığımız için bu değişikliği "git stash" komutu yardımıyla depolayabiliyoruz.
![git-stash-command]()

"git stash pop" komutuyla yaptığımız değişikliği bize geri getirir.
![git-stash-pop-command]()

"git stash list" komutuyla kaç tane stash işlemi yapılmış bunu görebiliyoruz.
![git-stash-list-command]()

"git stash apply stashismi" komutuyla stashismi olan değişikliği bize getiriyor.
![git-stash-apply-command]()

