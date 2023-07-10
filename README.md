## Proje Açıklaması

İnternet Kullanım Raporu Programı, kullanıcının belirli bir süre boyunca hangi sitelere girdiğini takip eder ve bu verileri analiz ederek bir rapor oluşturur. Rapor, en çok zaman geçirilen siteleri belirtir ve pasta dilimi grafiğiyle birlikte Word belgesine aktarılır.

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





[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Bu projeyi [MIT Lisansı](https://opensource.org/licenses/MIT) altında lisansladık. Lisansın tam açıklamasını burada bulabilirsiniz.
