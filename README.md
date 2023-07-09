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

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Bu projeyi [MIT Lisansı](https://opensource.org/licenses/MIT) altında lisansladık. Lisansın tam açıklamasını burada bulabilirsiniz.
