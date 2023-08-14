# Guide To Using Git (Git için Kullanma Kılavuzu)

**"git"** komutu bize git help dökümantasyonu getirir.<br/>
>![git-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-command.jpg)

**"git --version"** komutu bize gitin versiyonunu getirir.<br/>
>![git-version-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-version-command.jpg)

**"git config --global user.name "kullanıcı adı" "** komutu ile kullanıcı adı kaydediyoruz.<br/>
**"git config user.name"** komutu ile de koyduğumuz kullanıcı adını görebiliyoruz.<br/>
>![git-username-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-username-command.jpg)

**"git config --global user.email "email adresi" "** komutu ile email adresini kaydediyoruz.<br/>
**"git config user.email"** komutu ile de koyduğumuz email adresini görebiliyoruz.<br/>
>![git-email-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-useremail-command.jpg)

**"git status"** komutu gitin durumu gösterir.<br/>
Eğer klasörün herhangi bir repository ile bağlantısı yok ise bu durumda "git init" komutunu kullanıyoruz.<br/>
>![git-status-and-git-init-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-status-and-git-init-command.jpg)

**"git add dosya adi"** komutu o dosyayı kommitlemeye hazırlar.<br/>
**"git add ."** komutu bütün dosyaları kommitlemeye hazırlar.<br/>
>![git-add-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-add-command.jpg)

**"git commit -m "yorum" "** komutu kommite yorum ekler ve her kommite bir hash değeri atar.<br/>
>![git-commit-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-commit-command.jpg)

**"git log"** komutu ile kommitimizin kayıtları gösterir.<br/>
>![git-log-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-log-command.jpg)

**"git add ."** komutu ile ekleme yaparken diyelim bir dosyayı eklemek istemiyoruz. Böyle bir durumda ilk olarak yapılıcak şey **".gitignore"** isimli bir dosya oluşturuyoruz. Bundan sonra eklenmek istemeyen dosyayının ismini **".gitignore"** dosyasının içine yazıyoruz. Sonra işlemimize devam ediyoruz ve eklenmek istemeyen dosya eklenmemiş oluyor.<br/>
**"gitignore template"** ile tarayıcıda bir arama yaparsak önümüze örnek gitignore klasörleri çıkıcaktır. Bizde kendi yazdığım dile uygun olanı alıp kendimize göre uygulayabiliriz.
>![git-ignore-file](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-ignore-file.jpg)

**"git branch branchadi"** komutu ile yeni bir branch açabiliriz.
>![git-branch](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-branch.jpg)<br/>

>![git-branch-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-branch-command.jpg)

**"git switch master"** komutu ile headimizi master'a taşıyoruz.
>![git-switch](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-switch.jpg)<br/>

>![git-switch-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-switch-command.jpg)

**"git merge branchadi"** komutu bulunduğumuz branch ile yazdığımız branchadi branchini birleştiriyor.
>![git-merge](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-merge.jpg)

>![git-merge-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-merge-command.jpg)<br/>

>![git-merge-command2](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-merge-command2.jpg)<br/>

>![git-merge-command3](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-merge-command3.jpg)

Eğer ana branchde hiçbirşey yapmayıp yeni bir branchden ilerleyip ana branchle yeni branchi merge edersek bu işleme **"Fast Forwarding"** denir.
>![fast-forwarding](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/fast-forwarding.jpg)<br/>

>![fast-forwarding2](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/fast-forwarding2.jpg)<br/>

>![fast-forwarding-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/fast-forwarding-command.jpg)

**"git checkout hashdegeri"** komutu yardımıyla istediğimiz git loguna dönüş yapabiliriz. Geri gittiğimiz yerden devam etmek istiyosak yeni bir branch oluşturup devam edebiliriz.
>![git-checkout](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-checkout.jpg)<br/>

>![git-checkout2](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-checkout2.jpg)<br/>

>![git-checkout3](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-checkout3.jpg)<br/>

>![git-checkout-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-checkout-command.jpg)

**"git reset hashdegeri"** komutu bizim verdiğimiz hash değeri kommitine gider fakat değişiklikleri silmez. Tekrardan kaydetme komutlarıyla yaptığımız değişiklikleri kaydedebiliriz.
>![git-reset-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-reset-command.jpg)

**"git reset --hard hashdegeri"** komutu bizim verdiğimiz hash değeri kommitine gider ve değişiklikleri silip o hash değerinde kommitin aynısına dönmüş olur.
>![git-reset-hard](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-reset-hard.jpg)<br/>

>![git-reset-hard-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-reset-hard-command.jpg)

**"git revert hashdegeri"** komutu bizim verdiğimiz hash değerinin kommitini geri alır fakat yeni bir kommit ekleyerek bu işlemi yapar. Yani reset gibi hikayeyi geri sarmaz.
>![git-revert](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-revert.jpg)

>![git-revert-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-revert-command.jpg)

**"git diff"** komutu bizim yaptığımız değişiklikleri gösterir.
>![git-diff-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-diff-command.jpg)

**"git diff HEAD"** komutu bizim yaptığımız değişikliklerle HEAD'in bulunduğu kommitin değişikliklerini karşılaştırır.
>![git-diff-head-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-diff-head-command.jpg)

**"git diff hashdegeri hashdegeri2"** komutu vermiş olduğumuz hash değerleri arasındaki farkları karşılaştırır.
>![git-diff-hashdegeri-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-diff-hashdegeri-command.jpg)

**"git diff branch1 branch2"** komutu branchler arasındaki farkı gösterir.
>![git-diff-branch-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-diff-branch-command.jpg)

**"git rebase branchadi"** komutu hikaye örgüsünü düzeltmemize yarar. Fakat bu komutu eğer sizin branchinizi kullanan kimse yok ise uygulayın aksi halde çok büyük sorunlar ortaya çıkabilir.
>![git-rebase](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-rebase.jpg)<br/>

>![git-rebase-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-rebase-command.jpg)<br/>

>![git-rebase-command2](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-rebase-command2.jpg)

## Merge Conflict
Bir örnek üzerinde inceleyip sorunu çözelim. 
**İlk adım** bir java dosyasına email adresimizi kaydediyoruz.
>![Merge-conflict](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/Merge-conflict.jpg)<br/>

**İkinci adım** yeni bir branch açıyoruz.
>![Merge-conflict2](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/Merge-conflict2.jpg)<br/>

**Üçüncü adım** yeni branchin içinde kayıtlı email adresini değiştirip kaydediyoruz.
>![Merge-conflict3](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/Merge-conflict3.jpg)<br/>

>![Merge-conflict4](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/Merge-conflict4.jpg)

**Dördüncü adım** olarak master branchimize geçiyoruz ve email adresini silip kaydediyoruz.
>![Merge-conflict5](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/Merge-conflict5.jpg)<br/>

>![Merge-conflict6](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/Merge-conflict6.jpg)<br/>

>![Merge-conflict7](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/Merge-conflict7.jpg)<br/>

**Beşinci adım** master branchi ile diğer branchi merge etmeye çalışıyoruz. Fakat hata veriyor ve bize birini seçmemiz gerektiğini belirtiyor.
>![Merge-conflict8](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/Merge-conflict8.jpg)<br/>

>![Merge-conflict9](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/Merge-conflict9.jpg)<br/>

**Altıncı adım** ise birini seçip kaydediyoruz ve merge conflict sorununu çözmüş oluyoruz.
>![Merge-conflict10](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/Merge-conflict10.jpg)<br/>

>![Merge-conflict11](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/Merge-conflict11.jpg)<br/>

## Git Stash
Başka bir branchdeyken yaptığımız değişikliği kommitlicek kadar emin olmadığımız için bu değişikliği **"git stash"** komutu yardımıyla depolayabiliyoruz.
>![git-stash-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-stash-command.jpg)

**"git stash pop"** komutuyla yaptığımız değişikliği bize geri getirir.
>![git-stash-pop-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-stash-pop-command.jpg)

**"git stash list"** komutuyla kaç tane stash işlemi yapılmış bunu görebiliyoruz.
>![git-stash-list-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-stash-list-command.jpg)

**"git stash apply stashismi"** komutuyla stashismi olan değişikliği bize getiriyor.
>![git-stash-apply-command](https://github.com/AbdullahDemirkol/UserGuideforGit/blob/main/Pictures/git-stash-apply-command.jpg)

**README.md** dosyası için yazı kuralları Markdown işaretleme dili kullanılır. Bunun için [Markdown İşaretleme Dili Rehberi](https://commonmark.org/help/) adresinden ulaşabilirsiniz.
