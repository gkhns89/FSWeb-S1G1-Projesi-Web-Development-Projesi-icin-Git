Gökhan
# Araştırma Soruları

Artık yeni iş yerindeki ilk görevini gerçekleştirmek için hazırsın! Kullandığımız araçları biraz daha iyi anlama zamanı. Yapman istenilen şey, bu dokümanı güncelleyerek, aşağıdaki soruları soruları cevaplaman. Böylece Git yapısına biraz daha aşina olmaya başlayacaksın.

Soruları cevaplarken takıldığın yerlerde [GitHub docs](https://docs.github.com/en)'u kullanabilirsin. Docs, (ingilizce documentation'ın kısaltılmış halidir) bir programı veya dilin nasıl kullanılacağını anlatan dokümandır. Yazılım dünyasında sıkça kullanılır. Bir yazılımcı olarak _zamanınızın büyük çoğunluğu da bu tarz dokümanları okumakla ve üzerinde çalışmakla geçecek_.

![READ THE DOCS](https://github.com/Workintech/FSWeb-S1G1-Projesi-Web-Development-Projesi-icin-Git/blob/main/read-the-docs-wit.gif?raw=true)

Eğer aradığın soruların cevapları GitHub docs'ta yoksa, Google'lama becerileriniz size yardımcı olacak. Google'ı iyi kullanabilmek de aslında büyük bir dikkat ve çalışma gerektiriyor. Zamanla bu konuda da daha iyileştiğini göreceksin :)

## Sorular

1. Git nedir?
Açık kaynak olarak geliştirilen proje dosyalarının merkezi olarak kronolojik kontrol mekanizmasına sahip şekilde geliştirilmesine olanak sağlayan sistemin bütünüdür.
2. Git ile GitHub arasında ne fark var?
GitHub; git sisteminin kullanımı için bulut tabanlı proje geliştiricilerinin kodlarını barındırarak tek veya ekip olarak geliştirilmesine kolaylık sağlayan şirkettir.
3. Neden bir branch oluşturuyoruz?
Merkezi sistemde geliştirilen projenin lokal ortamda üzerinde çalışırken ayrı bir deneme/geliştirme yapılırken ana bütünü bozmama nedeni ile yeni bir branch oluşturmak ihtiyacı duyarız.
4. Pull Request'in amacı nedir?
Fork edilen bir çalışmada yapılan değişikliklerin proje sahibine geri ileterek sahibin bu değişiklikleri kendisine almasını sağlamaktır.
5. Bir Branchten diğerine geçmek için kullandığın KOMUT nedir? Mesela `isim-soyisim` branch'inde çalıştığını hayal et ve main branch'ine geçmek istiyorsun, ne yaparsın?
git checkout master

6. `git fetch`, `git merge` ve `git pull` arasındaki farklıarı açıklayınız. Bu konutlar ne yapar açıklayınız.
"git fetch" komutu yereldeki depomuzu uzaktaki depo içeriği ile güncelleme anlamına gelirken "git pull" komutu ise bunun tersi olarak uzaktaki içeriğin yerel depomuza getirirken kullanırız. "git merge" komutu ise x bir branch üzerinde yapmış olduğumuz değişikliklerin master branch ile entegre/birleştirme işleminde kullanılmaktadır. 
7. Merge conflict nedir?
Merge conflict olayı aynı dosyanın farklı kullanıcılar tarafından işlem yapılması sonucunda birleştirme işlemi gerektiği zaman karşılaşılan bir durumdur.
8. Merge conflict'i nasıl çözeriz?
MErge conflict durumu gerçekleşmeden önce veya sonra yapılacak yollar mevcuttur. Kısaca gerçekleşmeden önce bunun önüne geçebilmek için branch imizi master üzerinden rebase komutu kullanarak güncelleştirmek olabilir. Çakışma ihtimaline karşılık rebase işlemi öncesi stash komutu ile değişikliklerimizi koruma altına alabiliriz. Eğer conflict durumu gerçekleştiyse kullanıcının bu çakışan bölümü tespit etmesi gerekmektedir. Ardından ise bu bölümler manuel olarak düzeltilip korunması gereken yerler belirlenerek tekrardan birleştirme işlemi uygulanabilir.