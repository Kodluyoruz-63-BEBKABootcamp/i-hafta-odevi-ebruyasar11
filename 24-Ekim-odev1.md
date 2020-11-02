# **24 Ekim Ödevleri**
### **Github Hesabı:** https://github.com/ebruyasar11
### **Hackerrank Hesabı:** https://hackerrank.com/ebruyasar
### **StackOverFlow Hesabı:** https://stackoverflow.com/users/14515199/ebruyasar
### **Docker ve Docker'a Ait Kavramlar:**
Docker; *konteynerleştirme* olarak da bilinen işletim sistemi seviyesinde sanallaştırma sağlayan bir bilgisayar programıdır. Yazılımları kitaplıklar, sistem araçları, kod ve çalışma zamanı dahil olmak üzere yazılımların çalışması için gerekli her şeyi içeren konteyner adlı standartlaştırılmış birimler halinde paketler. Docker'ı kullanmanız kaynak kullanımını geliştirerek daha hızlı kod göndermenize, uygulama işlemlerini standart hale getirmenize, kodu sorunsuz bir şekilde taşımanıza ve tasarruf etmenize imkan tanır.

![image](https://docs.docker.com/engine/images/architecture.svg)

- **Container:**
    En basit hali ile imajların çalıştırılmış veya durdurulmuş halidir. Yazılımlarımızı paketleyip runtime bağımlılıklarını yönetebildiğimiz, işletim sisteminin sanallaştırmasını kullanmadan daha az kaynak tüketimi ile işlem izolasyonu sağlayan bir yapı parçacığıdır.

- **Docker Image:**
    Adından da anlaşılacağı gibi çalışacak uygulamanızın ve uygulamanızın altyapısında çalışan gerekli işletim sistemi kütüphanelerinin bulunduğu bir yapıdır. İmajları, container yaratmak için gereken talimatların bulunduğu bir şablon olarak düşünebiliriz. Docker image *build* komutu ile bir Dockerfile üzerinden oluşturduğumuz yapılardır.

- **Docker Registry:**
    İmajların tutulduğu ve dağıtıldığı bir ortamdır. Aynı Github’da olduğu gibi elimizdeki imajları docker registry’sine push edebilir veya daha önceden yüklenmiş olan bir docker imajı kendi localimize çekebiliriz. Bu sayede ihtiyaçlarınızı karşılayacak bir imaja çok hızlı bir şekilde erişebilir, gerekirse üzerinde değişiklik yapabilir ve tag’leyerek farklı bir versiyon olarak yeniden gönderebiliriz.

- **Docker Daemon:**
    Daemon (Server) sistemin kernel bölümüdür. Image, container, data volume, network gibi docker objelerini oluşturur ve yönetir. Bunu yapabilmek için Rest API taleplerini dinler.

- **Docker Client:**
    Konteynır oluşturmak, çalıştırmak, durdurmak, dağıtmak gibi işlevleri yerine getirmek için Docker Daemon ile konuşur. Server tarafına tüm komutar client üzerinden gönderilir. Docker’ın kullanıcı arayüzüdür.

### **.Net Versiyonları ve Aralarındaki Farklar:** 

- **Asp .Net Core 1.x:**
    Açık kaynak geliştirmeye yönelik çabaların getirdiği en önemli başarı Asp .Net Core 1.0'ın herkese açık olarak piyasaya sürülmesiydi. 2002 ve çekirdek mimarisinde önemli değişiklikler olmadan 4.6.2 sürümüne kadar gelişti; yepyeni çerçeve, MVC, Web API ve web sayfaları gibi önceki tüm web uygulama teknolojilerini, daha önce MVC6 olarak bilinen tek bir programlama modülünde  birleştirdi.

- **Asp .Net Core 2.x:**
    Yeni sürüm, son ikisini eskisi ile daha geriye dönük uyumlu hale getirmek için çoğunlukla .NET Framework, .NET Core ve .NET Standard arasında paylaşılan API'leri standartlaştırmayı amaçlayan çok sayıda önemli arabirim geliştirmesine sahipti: bunlar sayesinde mevcut .NET Framework projelerini .NET Core ve/veya .NET Standard'a taşıma çabaları, eskisinden çok daha kolay hale geldi ve birçok "geleneksel" geliştiriciye mevcut teknik bilgilerini kaybetmeden yeni paradigmayı deneme ve adapte etme şansı verdi.

- **Asp .Net Core 3.x:**
    Eylül 2019'da piyasaya sürüldü ve başka bir dizi performans ve güvenlik iyileştirmesi ve yeni özelliklerle birlikte geldi. Örneğin: Blazor, gRPC gibi yeni özellikler, Windows Forms ve Windows Presentation Foundation için gelişmiş içe aktarma yetenekleriyle  Windows masaüstü uygulamaları desteği, C# 8 desteği vb. 

    ASP .NET Core geliştirme ekibi, .NET Core 3.0 üzerinde .NET Core Docker deneyimini iyileştirmek için çok çaba sarf etti. Daha spesifik olarak, CoreCLR'yi daha verimli hale getirmek, Docker kaynak sınırlarını (bellek ve CPU gibi) varsayılan olarak daha iyi karşılamak ve daha fazla yapılandırma ayarı sunmak için önemli çalışma zamanı değişiklikleri içeren ilk sürümdür.

### **.Net 5 ve Yenilikleri:**
.Net 5 ile artık tek bir .Net olacak, yani Xamarin, Unity, ML .Net dahil olmak üzere tüm framework’ler tek bir çatı altında birleşiyor. 

Şimdiye kadar .Net Core için yazdığımız kütüphaneler .Net Framework’te çalışmayabiliyordu. .Net Framework ile yazılmış bir uygulamayı .Net Core’a geçirirken shared library olarak bazı tanımlamalar yapmak gerekebiliyor. Çözüm olarak tanımlamalarımızı .Net Standart ile geliştirmemiz gerekiyordu ancak .Net 5 ile birlikte artık tek bir Base Class Library olacak. Şu anda Xamarin uygulamaları Mono Base Class Library kullanırken artık .Net 5 ile .Net Core Base Class Library kullanabilecek.

BCL’de daha hızlı algoritmaların yanı sıra HTTP3 desteği de .Net 5 ile .Net dünyasına giriş yapacaktır.

ASP .NET Web Forms .NET 5'e gelmeyecek ve Microsoft, şu anda resmi olarak tanıtılan Blazor’ı öneriyor.

### **Markdown Yazımı ve Kullanımı:**
Markdown yazımı hakkında bilgiye [bu linkten](https://guides.github.com/features/mastering-markdown/) ulaşabilirsiniz. Bu ödev Visual Studio Code'da hazırlanmıştır.

### **Microsoft Azure Hizmetleri:**
- **Sanal makine hizmeti:** 
Microsoft Azure teknolojisi ile yeni sanal makineler oluşturabileceğiniz gibi var olan imaj dosyasından da sanal makinenizi kullanabilirsiniz. Azure IT çalışanlarına VHD galerisi sunmaktadır. Bu galerinin içerisinde Windows Server 2012, SQL Server gibi Microsoft ürünlerinin yanında Linux imajları da yer almaktadır.  Azure Premium depolama sayesinde giriş ve çıkış işlemlerini(I/O) çok hızlı şekilde yapmak ve performanstan ödün vermemek adına SSD depolama tabanını kullanmaktadır.

- **Web Barındırma Hizmeti:** 
Azure Web Siteleri, kurumsal düzeydeki web uygulamaları oluşturmanızı sağlar. Azure teknolojisini kullanarak; ASP .NET, Java, Node.js, C# gibi diller tercih edilebilir. Dil özgürlüğünün yanında WordPress, Joomla, Drupal gibi birçok web uygulamaları ve CMS çözümlerini de çalıştırmanıza olanak sağlıyor.

- **Veri Tabanı Hizmeti:** 
Verilerin saklanması ve verilerin yönetilmesi için Windows Azure teknolojisinde farklı teknolojiler kullanılır. Bunlardan birisi Windows Azure Virtual Machines ile oluşturulan SQL Server veya diğer DBMS çalıştırılmasıdır. Burada NoSQL teknolojisinin kullanılması da mümkündür. Verileri saklamak için kullanıcı kendi veri tabanını oluşturabilir ancak buranın yönetimini yine kullanıcıların kendilerinin yapması gerekir. Windows Azure bu iş içinde kullanıcılara üç farklı yöntem sunmuştur. Bunlar SQL Databases, Tables ve Blobs’tur.

- **Mobil Hizmetler:** 
Azure mobil hizmetinin en büyük özelliklerinin başında çapraz platforma sahip olmasıdır. Yani IOS, Android, Windows Phone, Mac ve Windows için aynı altyapıyı kullanan uygulama oluşturabilmeniz demektir. Diğer önemli özellik ise C# ve Node.js kullanarak uygulamanın uç kısmı olan sistemi yani back end sistemini oluşturabilirsiniz.

Azure’un sunmuş olduğu diğer önemli özelliklerden birisi de *Active Directory* özelliğidir. Bu özellik ile kullanıcıların kimliğini doğrulayıp, SQL Server, Share Point gibi çeşitli birçok özelliklere güvenli bir şekilde bağlanmasını sağlayabiliriz.

### **Kodun Kalitesinin Metrik Olarak Ölçülmesi:**
Maliyet, zaman, test, bakım, tasarım düzeni, kullanım kolaylığı ve anlaşılabilirlik bir yazılım için kalite ölçütleri olarak gösterilebilir.

**S.O.L.I.D** Robert C. Martin tarafından öne sürülen prensipler bütünüdür. Kısaltması Michael Feathers tarafından tanımlanan bu prensiplerin amacı; geliştirdiğimiz yazılımın gelecekte gereksinimlere en az değişimle kolayca adapte olması, yeni özellikleri kodda bir değişikliğe gerek kalmadan kolayca ekleyebilmek ve kod üzerinde sürekli düzeltme hatta yeniden yazma gibi sorunların yol açtığı zaman kaybını da minimuma indirmektir.

**Single-responsibility principle:** Bir sınıf (nesne) yalnızca bir amaç uğruna değiştirilebilir, o da o sınıfa yüklenen sorumluluktur, yani bir sınıfın(fonksiyona da indirgenebilir) yapması gereken yalnızca bir işi olması gerekir.
    
**Open-closed principle:** Bir sınıf ya da fonksiyon halihazırda var olan özellikleri korumalı ve değişikliğe izin vermemelidir. Yani davranışını değiştirmiyor olmalı ve yeni özellikler kazanabiliyor olmalıdır.

**Liskov substitution principle:** Kodlarımızda herhangi bir değişiklik yapmaya gerek duymadan alt sınıfları, türedikleri(üst) sınıfların yerine kullanabilmeliyiz.

**Interface segregation principle:** Sorumlulukların hepsini tek bir arayüze toplamak yerine daha özelleştirilmiş birden fazla arayüz oluşturmalıyız.

**Dependency Inversion Principle:** Sınıflar arası bağımlılıklar olabildiğince az olmalıdır özellikle üst seviye sınıflar alt seviye sınıflara bağımlı olmamalıdır.

### **Beğendiğim İş İlanları**

- [Monioo Teknoloji (Junior Software Developer)](https://tr.linkedin.com/jobs/view/junior-software-engineer-at-monioo-teknoloji-2220540621?refId=7ee6ac0b-62a3-4dc0-b085-10fec917fe72&position=1&pageNum=0&trk=public_jobs_job-result-card_result-card_full-click)

- [Defacto (Frontend Developer)](https://tr.linkedin.com/jobs/view/frontend-developer-%25100-remote-at-defacto-2011315715?refId=d6e498db-08df-4b30-9b52-d1afd396a2ba&position=2&pageNum=0&trk=public_jobs_job-result-card_result-card_full-click)

- [FineDine (Frontend Developer)](https://tr.linkedin.com/jobs/view/frontend-developer-react-js-at-finedine-digital-menus-for-restaurants-cafes-bars-2151136767?refId=e16eea42-7d68-4aae-87e5-51203c73875b&trk=public_jobs_topcard_title)

- [Retinadata (Software Engineer)](https://tr.linkedin.com/jobs/view/software-engineer-frontend-at-retinadata-2224728849?refId=70c39ced-d3a4-4206-84c0-b8e8be82a685&trk=public_jobs_topcard_title)

### **Yazılım Alanında Takip Ettiğim Kişiler**
- [Zafer Demirkol](https://tr.linkedin.com/in/zaferdemirkol)

- [Rodolfo De Nadai](https://github.com/rdenadai)
    
- [David J. Malan](https://github.com/dmalan)

- [Ahmet Alp Balkan](https://github.com/ahmetb)

- [Atıl Samancıoğlu](https://tr.linkedin.com/in/atıl-samancıoğlu-96028871)

### **Github ile Alakalı Üzerine Çalışılabilir Repository Listesi**

- https://github.com/rdenadai/sentiment-text-prediction-api

- https://github.com/btu-cse/bm_tanitim_bot

- https://github.com/ahmetkasif/passvault