# NLP FUN - Doğal Dil İşleme Uygulamaları

![NLP FUN Logo](https://static.vecteezy.com/system/resources/previews/008/505/801/non_2x/artificial-intelligence-robot-brain-logo-template-illustration-design-vector.jpg)

## Proje Hakkında
NLP FUN, Doğal Dil İşleme (Natural Language Processing - NLP) teknolojilerini kullanıcıların kolay ve hızlı bir şekilde deneyimleyebilmesini sağlayan web tabanlı bir Django uygulamasıdır. 

Bu platform, modern arayüzü ile kullanıcılara üç temel NLP hizmeti sunmaktadır:
- **Metin Özetleme**: Uzun metinleri otomatik olarak kısaltarak ana fikirlerini çıkarır
- **Duygu Durum Analizi**: Metinlerdeki duygusal tonu algılar (pozitif, negatif, nötr)
- **Sohbet Botu**: Kullanıcıyla doğal dilde iletişim kuran yapay zeka asistanı

## Doğal Dil İşleme Nedir?

Doğal dil işleme (natural language processing), bilgisayarlara insan dilini okuma, anlama ve yorumlama yeteneği veren bir yapay zeka uygulamasıdır. Bilgisayarların, insan duygularını ölçmesine ve insan dilinin hangi bölümlerinin önemli olduğunu belirlemesine yardımcı olur.

NLP teknolojileri günümüzde:
- Sesli asistanlar
- Otomatik çeviriler
- Spam filtreleri
- Arama motorları
- Müşteri hizmetleri botları
- Duygu analizi araçları
ve daha pek çok alanda kullanılmaktadır.

## Teknoloji Altyapısı

Proje aşağıdaki teknolojileri kullanmaktadır:
- **Django**: Web uygulaması backend çatısı
- **HTML/CSS/JavaScript**: Frontend geliştirmesi
- **Bootstrap**: Responsive tasarım için CSS framework'ü
- **Hugging Face Transformers**: NLP modellerinin uygulanması için
- **AOS**: Sayfa animasyonları için JavaScript kütüphanesi
## Kullanılan Modeller

### 1. Metin Özetleme Modeli
Bu projede Türkçe metinleri özetlemek için **[mrm8488/bert2bert_shared-turkish-summarization](https://huggingface.co/mrm8488/bert2bert_shared-turkish-summarization)** modeli kullanılmıştır.

Bu model, BERT mimarisini temel alan ve Türkçe metinler üzerinde eğitilmiş bir yapay zeka modelidir. Uzun metinlerdeki ana noktaları belirleyerek bunları daha kısa ve öz bir özet haline getirir.

### 2. Duygu Analizi Modeli
Duygu analizi için **[savasy/bert-base-turkish-sentiment-cased](https://huggingface.co/savasy/bert-base-turkish-sentiment-cased)** modeli kullanılmıştır.

Bu model özellikle Türkçe metinlerdeki duygusal tonu analiz etmek için optimize edilmiştir. Bir metni pozitif, negatif veya nötr olarak sınıflandırabilir ve analiz sonucunun güven skorunu yüzde olarak verir.

### 3. Sohbet Botu Modeli
Sohbet botu özelliği için **[facebook/blenderbot-400M-distill](https://huggingface.co/facebook/blenderbot-400M-distill)** modeli kullanılmıştır.

**Not:** Sohbet botunun hali hazırda Türkçe ile eğitilmiş bir versiyonu olmadığı için projede Python'un "googletrans" kütüphanesi entegre edilmiştir. Kullanıcı tarafından girilen Türkçe cümle önce İngilizce'ye çevrilmekte, model İngilizce olarak cevap vermekte ve sonra bu cevap tekrar Türkçe'ye çevrilerek kullanıcıya sunulmaktadır.

## Proje Ekibi
Bu uygulama Murat Yıldız tarafından geliştirilmiştir.

---

© 2025 NLP FUN - Tüm hakları saklıdır.
