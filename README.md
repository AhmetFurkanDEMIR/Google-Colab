# Google Colab

![1*Lad06lrjlU9UZgSTHUoyfA](https://user-images.githubusercontent.com/54184905/83964957-ece37580-a8b8-11ea-909d-2a5a00292f73.png)

* Colaboratory veya kısaca "Colab", tarayıcınıza Python kodları yazmanıza ve yürütmenize olanak tanır.
Öğrenci, veri bilimcisi veya yapay zeka araştırmacısı iseniz Google Colab işinizi kolaylaştırır.

      Sıfır yapılandırma gerekli.
      
      GPU'lara ücretsiz erişim.
      
      Kolay paylaşım.


# Yeni bir notebook oluşturalım (CPU)

* Google Colab sayfasına ilerleyin : https://colab.research.google.com/notebooks/intro.ipynb#recent=true
* Burada, sağ aşağıda bulunan "NEW NOTEBOOK" 'a tıklayınız.
* Google sizin için yeni bir notebook oluşturur ve bu notebook 'u artık Google 'ın bilgisayarlarından kullanırsınız.

![Screenshot_2020-06-07_12-21-04](https://user-images.githubusercontent.com/54184905/83965030-6bd8ae00-a8b9-11ea-8a90-6736c35cb474.png)

* CPU destekli bir bilgisayara uzaktan bağlandınız. Artık Jupyter-Notebook 'da yapabildiğiniz her şeyi bu notebookda da yapabilirsiniz. Python kodlarınızı bu bilgisayarda yazıp çalıştırabilirsiniz.
(İlk satıra "!nvidia-smi" yazıp Shift+Enter 'e basıp test edebilirsiniz.)


# Oluşturduğumuz Notebook 'a GPU Desteği Sağlayalım

* Neden GPU ?
* Bilgisayar dünyası derin öğrenme ve yapay zeka ile inanılmaz bir değişim yaşıyor. Derin öğrenme, hem eğitim hem de çıkarım için GPU hızlandırmasına dayanır.

![index](https://user-images.githubusercontent.com/54184905/83965577-40f05900-a8bd-11ea-9cf4-500251a89b6e.png)

* Sol üstte bulunan Edit sekmesine gidiniz, oradan "Notebook settings" e tıklayınız

![Screenshot_2020-06-07_12-28-05](https://user-images.githubusercontent.com/54184905/83965309-68debd00-a8bb-11ea-92ce-1a5ab599854d.png)

* Açılan pencereden "Hardware accelerator" sekmesini "GPU" olarak değiştirin.
* Runtime shape sekmesini Standart olarak bırakabilirsiniz. (yüksek bellek kullanımı isteyen kodlar için "High-RAM" olarak seçiniz.)

![Screenshot_2020-06-07_12-40-51](https://user-images.githubusercontent.com/54184905/83965398-3a151680-a8bc-11ea-8836-c4ab94030916.png)

* Ardından Save 'e basınız. Google bilgisayara GPU desteği sağlar ve Cihaza yeniden kurulum yapılır.

![Screenshot_2020-06-07_12-51-07](https://user-images.githubusercontent.com/54184905/83965633-a93f3a80-a8bd-11ea-9d5e-3f922cb609b3.png)

* Ücretsiz bir şekilde bir GPU sahibi oldunuz :)

### Önemli bir bilgi

* Google Colab 'ın ücretsiz versiyonunu kullanıyorsanız K80 ve P100 GPU 'larını kullanabilirsiniz. Bu GPU 'lara öncelikli Erişiminiz yoktur. Eğer PRO versiyonunu kullanıyorsanız T4 ve P100 GPU 'larını öncelikli olarak kullanabilirsiniz.
           
      Google Colab PRO : https://colab.research.google.com/signup
      

# Oluşturduğumuz Notebook 'a TPU Desteği Sağlayalım

* TPU nedir ?

* -Tensor Processing Unit- yani Tensör İşlem Birimi dört bağımsız çipten oluşmaktadır. Her bir çip, Tensör Çekirdek (Tensor Core) adı verilen iki hesaplama çekirdeğinden oluşur. Bir Tensör Çekirdek, skaler, vektör ve matris birimlerinden (MXU) oluşur.

* Ayrıca, her Tensör Çekirdeği ile 8 GB’lık çip bellek (HBM) ilişkilendirilmiştir. TPU üzerindeki 8 çekirdeğin her biri, kullanıcı hesaplarını (XLA ops) bağımsız olarak yürütebilir.
Yüksek bant genişliğine sahip ara bağlantı yolları, çiplerin birbirleriyle doğrudan iletişim kurmasını sağlar. XLA, Tensorflow backend için deneysel bir JIT(Just in Time) derleyicisidir. CPU (Merkezi İşlem Birimi) ve GPU (Grafik İşlem Birimi)’dan en önemli farkı ve özelliği derin öğrenmenin yapı taşı olan lineer cebir yani matris işlemlerinin paralel olarak ve çok boyutlu olarak gerçekleşmesi için tasarlanmış spesifik bir donanım olmasıdır.

Hatta buna matris ya da tensör makinesi (matrix/tensor machine) de denmektedir.

2015 yılında Google ilk TPU merkezini kurmuştur. Çünkü Google Aramalar, Çeviri, Fotoğraflar, E-posta ve Bulut gibi uygulamalarının tamamında derin öğrenme ve dolayısyla tensör işlemler uygulamaktadır.

* Google’ın sunduğu bu teknolojinin arkasındaki ekibe göre, “Yapay sinir ağları temelinden faydalanan üretilen yapay zeka uygulamalarını eğitmek için kullanılan TPU’lar, CPU ve GPU’lara göre 15 ila 30 kat daha hızlıdır!”

* ALINTI orjinal içerik : https://medium.com/@ayyucekizrak/ad%C4%B1m-ad%C4%B1m-google-colab-%C3%BCcretsiz-tpu-kullan%C4%B1m%C4%B1-621dc6e5487d

* Şimdi TPU 'yu devreye sokalım.
* Sol üstte bulunan Edit sekmesine gidiniz, oradan "Notebook settings" e tıklayınız
* Açılan pencereden "Hardware accelerator" sekmesini "TPU" olarak değiştirin.
* Runtime shape sekmesini Standart olarak bırakabilirsiniz. (yüksek bellek kullanımı isteyen kodlar için "High-RAM" olarak seçiniz.)

![Screenshot_2020-06-07_13-06-28](https://user-images.githubusercontent.com/54184905/83965922-cffe7080-a8bf-11ea-81d2-a2a2fcbb9eb7.png)

* Ardından Save 'e basınız. Google bilgisayara TPU desteği sağlar ve Cihaza yeniden kurulum yapılır.

* Ücretsiz bir şekilde bir TPU sahibi oldunuz :)

# Oluşturduğumuz Notebook hakkında bilgi

* Oluşturduğunuz Notebookları 12 saat boyunca açık bırakabilirsiniz. Eğer Colab PRO kullanıyorsanız 24 saat boyunca CPU/GPU/TPU desteği alabilirsiniz.

* Jupyter-Notebook da yapabildiğiniz her şeyi burada da yapabilirsiniz.

* Oluşturduğunuz notebookları indirebilirsiniz veya Python scripti haline getirip indirebilirsiniz.

# Veri setlerimizi nasıl kullanacağız ?

* 1-) Sol tarafta bulunan Files kısmından Upload 'a basınız açılan pencereden verilerinizi seçip upload edebilirsiniz.

![Screenshot_2020-06-07_13-14-19](https://user-images.githubusercontent.com/54184905/83966150-2b7d2e00-a8c1-11ea-9cac-169b97994320.png)

* 2-) Verilerinizi Google Drive 'a yükleyip oradan import edebilirsiniz.
* Verilerinizi Drive upload ettikten sonra notebookumuzdan Sol tarafta bulunan Files kısmından Mount drive 'e basınız açılan pencereden "CONNECT TO GOOGLE DRİVER" kısmına basınız, artık Drive 'ınızda bulunan herşeyi kodunuzda kullanabilirsiniz.

![Screenshot_2020-06-07_13-20-55](https://user-images.githubusercontent.com/54184905/83966301-13f27500-a8c2-11ea-912d-69b0fd2b5ca7.png)

* "%cd /content/drive/My Drive/..." şeklinde istediğiniz klasöre ilerleyebilirsiniz.
* "!ls" şeklinde klasörünüzdeki verileri inceleyebilirsiniz.

![Screenshot_2020-06-07_13-25-15](https://user-images.githubusercontent.com/54184905/83966366-7ea3b080-a8c2-11ea-9c91-23e80ce91e4c.png)

# CPU vs GPU vs TPU
*
