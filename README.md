## Proje Açıklaması

Bu proje, Python kullanarak bir internet kullanım raporu hizmeti oluşturmayı amaçlamaktadır. Hizmet, kullanıcının hangi sitelere ne kadar zaman harcadığını izler ve günlük raporlar oluşturur. Raporlar, masaüstüne tarihle birlikte kaydedilir ve her gün yeni bir rapor oluşturulur.


## Kullanım

1. Python kodunu çalıştırın: `python internet_kullanim_raporu.py`
2. Program arka planda çalışmaya başlar ve belirtilen süre boyunca kullanıcının gezdiği siteleri kaydeder.
3. Belirtilen süre sonunda, rapor oluşturulur ve `internet_kullanim_raporu.docx` adlı Word belgesine kaydedilir.
4. Word belgesini açarak, en çok zaman geçirilen siteleri ve pasta dilimi grafiğini görebilirsiniz.

## Gereksinimler

Programın çalışabilmesi için aşağıdaki Python kütüphanelerinin kurulu olması gerekmektedir:

- `win32gui`
- `win32process`
- `matplotlib`
- `docx`

Gerekli kütüphaneleri yüklemek için aşağıdaki komutu kullanabilirsiniz:

  ```python
    pip install pywin32 matplotlib python-docx
  ```

## AlwaysUp ile Hizmet Olarak Kullanma

1. [AlwaysUp](https://www.coretechnologies.com/products/AlwaysUp/) adlı aracı indirin ve bilgisayarınıza kurun.

2. AlwaysUp'ı çalıştırın ve **Add Application** düğmesini tıklayın.

3. **Application** sekmesinde aşağıdaki ayarları yapın:

   - **Application Path** kısmına Python yolunu ekleyerek `main.py` dosyasının tam yolunu girin.

   - **Start In** kısmına projenin dizin yolunu girin.

   - **Arguments** kısmını boş bırakın.

4. **Service** sekmesinde aşağıdaki ayarları yapın:

   - **Service Name** kısmına "Internet Kullanım Raporu Hizmeti" adını girin.

   - **Startup** bölümünde **Automatic** seçeneğini seçin.

5. **Save** düğmesini tıklayarak yapılandırmayı kaydedin.

6. "Internet Kullanım Raporu Hizmeti"ni seçin ve **Start** düğmesini tıklayarak hizmeti başlatın.

Hizmet şimdi AlwaysUp aracılığıyla çalışacak ve her gün yeni bir rapor oluşturarak masaüstüne kaydedecektir. Raporlarınızı "internet_kullanim_raporu_<tarih>.docx" dosyaları olarak masaüstünde bulabilirsiniz.

**Not**: Python dosyasını EXE'ye dönüştürmek gerekebilir. EXE dosyasını oluşturmak için aşağıda ki adımları takip ediniz:

1. Terminali açın ve projenin bulunduğu dizine gidin:

   ```bash
   cd /path/to/project
    ```

2.Gerekli paketi yükleyin:
 ```bash
  pyinstaller --onefile main.py
```
3.Python dosyasını EXE'ye dönüştürmek için aşağıdaki komutu çalıştırın:
 ```bash
pyinstaller --onefile main.py
```

4. İşlem tamamlandığında, dist adlı bir dizin oluşturulacak ve EXE dosyası bu dizinde bulunacaktır.

5. EXE dosyasını kullanmak için, bu dosyayı başka bir yere taşıyabilir veya paylaşabilirsiniz.

6. Artık Python dosyanızı bir EXE dosyasına dönüştürdünüz. Bu şekilde Python çevresi veya paket gereksinimlerine ihtiyaç duymadan projeyi çalıştırabilirsiniz.


## Lisans

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Bu projeyi [MIT Lisansı](https://opensource.org/licenses/MIT) altında lisansladık. Lisansın tam açıklamasını burada bulabilirsiniz.
