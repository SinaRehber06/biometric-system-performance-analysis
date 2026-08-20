Biometric Authentication Analysis

Bu proje, biyometrik kimlik doğrulama sistemlerinin performansını değerlendirmek amacıyla geliştirilmiştir. Çalışmada biyometrik özellik vektörleri kullanılarak gerçek kullanıcı (Genuine) ve sahte kullanıcı (Imposter) skorları hesaplanmakta ve sistemin doğrulama performansı analiz edilmektedir.

Kullanılan Yöntemler

Projede biyometrik özellikler üzerinde aşağıdaki işlemler gerçekleştirilmektedir:

Biyometrik özelliklerin yüklenmesi
Özelliklerin [0,1] aralığında normalize edilmesi
Öklid mesafesi kullanılarak benzerlik skorlarının hesaplanması
Genuine ve Imposter skorlarının oluşturulması
FAR (False Acceptance Rate) hesaplanması
FRR (False Rejection Rate) hesaplanması
EER (Equal Error Rate) değerinin belirlenmesi
EER eşik değerinin hesaplanması
DET eğrisinin oluşturulması
Kullanılan Teknolojiler
Python
NumPy
Matplotlib
SciPy
Jupyter Notebook
Veri Seti

Analiz sırasında biyometrik özellikleri içeren Features.npz dosyası kullanılmaktadır.

Veri güvenliği ve dosya boyutu nedeniyle veri seti repository içerisinde bulunmayabilir.

Performans Metrikleri
FAR – False Acceptance Rate

Yetkisiz bir kullanıcının sistem tarafından kabul edilme oranını ifade eder.

FRR – False Rejection Rate

Yetkili bir kullanıcının sistem tarafından reddedilme oranını ifade eder.

EER – Equal Error Rate

FAR ve FRR değerlerinin birbirine eşit veya en yakın olduğu noktadır. Biyometrik sistemlerin performansını karşılaştırmak için kullanılan önemli metriklerden biridir.

DET Curve

FAR ve FRR arasındaki ilişkiyi göstererek biyometrik doğrulama sisteminin hata performansının görselleştirilmesini sağlar.

Örnek Sonuç

Çalışma sonucunda elde edilen örnek değerler:

EER Değeri: 0.0292
Eşik Değeri: 0.776

Bu sonuçlara göre sistem için yaklaşık %2.92 EER değeri elde edilmiştir.

Grafikler

Çalışma sonucunda üç farklı analiz grafiği oluşturulmaktadır:

Genuine ve Imposter skor dağılımları
FAR-FRR değişimi ve EER noktası
DET eğrisi

Oluşturulan grafik:

biometric_analysis_results.png

Proje Yapısı
biometric-authentication-analysis/
│
├── biometric_analysis.ipynb
├── Features.npz
├── biometric_analysis_results.png
└── README.md
