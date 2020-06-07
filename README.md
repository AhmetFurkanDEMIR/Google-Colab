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
* Ardından Save 'e basınız. Google bilgisayara GPU desteği sağlar, Cihaza yeniden kurulum yapılır.

![Screenshot_2020-06-07_12-40-51](https://user-images.githubusercontent.com/54184905/83965398-3a151680-a8bc-11ea-8836-c4ab94030916.png)

* Ücretsiz bir şekilde bir GPU sahibi oldunuz :)
