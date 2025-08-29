# TR-LLM Türkçe Performans Analizi

Beş güncel büyük dil modelinin (GPT-5 Thinking, Gemini 2.5 Pro, Claude 4 Sonnet, Grok 3, DeepSeek R1) **Türkçe dil becerileri**; yazım, dil bilgisi, anlama ve mantık boyutlarında **500 soruluk** bir çerçeve ile değerlendirilmiştir.

> Ayrıntılı metodoloji ve analiz: **Medium makalesi**  
> https://furkanaksoyy.medium.com/büyük-dil-modellerinin-türkçe-dil-becerileri-kapsamlı-bir-performans-analizi-13bdf5ff396f

---

## İçerik

- [Amaç ve Kapsam](#amaç-ve-kapsam)
- [Değerlendirilen Modeller](#değerlendirilen-modeller)
- [Test Tasarımı](#test-tasarımı)
- [Depo Yapısı](#depo-yapısı)
- [Hızlı Bakış: Sonuçlar](#hızlı-bakış-sonuçlar)
- [Kullanım / Yeniden Üretim](#kullanım--yeniden-üretim)
- [Planlananlar](#planlananlar)
- [Lisans](#lisans)
- [İletişim](#iletişim)
- [Alıntı (Citation)](#alıntı-citation)

---

## Amaç ve Kapsam

Türkçe; eklemeli (aglütinatif) yapısı, ses uyumu ve zengin ek sistemi nedeniyle LLM’ler için özgün zorluklar içerir.  
Bu çalışma, modellerin **temel kurallar** (yazım, dil bilgisi) ve **üst düzey beceriler** (kültürel dil, sözel/sayısal mantık, code-switching) üzerindeki yetkinliklerini karşılaştırmalı olarak ortaya koyar.

## Değerlendirilen Modeller

- **GPT-5 Thinking (OpenAI)**
- **Gemini 2.5 Pro (Google)**
- **Claude 4 Sonnet (Anthropic)**
- **Grok 3 (xAI)**
- **DeepSeek R1 (Open Source)**

## Test Tasarımı

Toplam **500 soru**, 6 ana başlıkta derlenmiştir:

1. **Kelime Yazım Doğruluğu**  
2. **Temel Dil Bilgisi** (7 alt kategori: *de/da, ki, mı/mi, ünlü uyumu, ünsüz benzeşmesi, noktalama–tarih–kesme, yapım/çekim ekleri*)  
3. **Kültürel Dil Becerileri** (*atasözleri, deyimler*)  
4. **Mantıksal Çıkarım** (*sözel mantık, sayısal mantık*)  
5. **Standart Sınav Performansı** (*TYT Türkçe denemesi*)  
6. **Anlama ve Yorumlama** (*code-switching senaryoları*)

Değerlendirmelerde **TDK Yazım Kılavuzu (2025)** referans alınmıştır. Ayrıntılı yönergeler ve örnekler için Medium makalesine bakınız.

## Depo Yapısı

- **Veri:** [`./data/`](./data/)
- **Görseller:** [`./images/`](./images/)
- **Sonuç & Metrikler:** [`./results/`](./results/)

## Hızlı Bakış: Sonuçlar

- **Genel tablo:** GPT-5 Thinking ve Gemini 2.5 Pro **dengeli ve yüksek** performans göstermiştir (≈ %91 civarı).  
- **Temel kurallar:** Tüm modeller yazım/dil bilgisi başlıklarında **yüksek doğruluk** sergilemiştir.  
- **Kültürel bağlam:** Atasözleri/deyimlerde **model bazlı farklılaşma** belirgindir.  
- **Mantık:** Sözelde ortalama; **sayısal mantıkta** bazı modellerde **belirgin düşüş** görülmüştür.  
- **Not:** Ayrıntılı metrik, örnek ve yorumlar için Medium makalesi ve [`results/`](./results/) klasörüne bakınız.

> Seçilmiş ekran görüntüleri: [`images/`](./images/)

## Kullanım / Yeniden Üretim

Bu depo şu an **sonuç ve materyal paylaşımı** amaçlıdır. Kod/araçlar eklenince aşağıdaki adımlar güncellenecektir:

1. `data/` içeriğini inceleyin (soru setleri ve yönergeler).
2. `results/` altındaki tablo/görseller ile bulguları karşılaştırın.
3. Ayrıntılı metodoloji ve yorumlar için Medium makalesini okuyun.

> İlerleyen sürümlerde: değerlendirme betikleri, puanlayıcı (scoring) yardımcıları ve yeniden üretim yönergeleri eklenecektir.

## Planlananlar

- [ ] Değerlendirme betiklerinin paylaşılması  
- [ ] Sonuçların `.csv`/`.xlsx` biçiminde standardizasyonu  
- [ ] Ek model/versiyonların eklenmesi  
- [ ] Uzun metin (doküman düzeyi) testleri

## Lisans

Bu proje **MIT Lisansı** ile lisanslanmıştır. Ayrıntı için bkz. [`LICENSE`](./LICENSE).

## İletişim

**Furkan Aksoy** — furkanaksoy178@gmail.com  
Medium: https://furkanaksoyy.medium.com/

## Alıntı (Citation)

Bu çalışmayı referans vermek isterseniz:
Aksoy, F. (2025). Büyük Dil Modellerinin Türkçe Dil Becerileri: Kapsamlı Bir Performans Analizi.
GitHub: https://github.com/FurkanAksoyy/tr-llm-turkce-performans-analizi

Medium: https://furkanaksoyy.medium.com/büyük-dil-modellerinin-türkçe-dil-becerileri-kapsamlı-bir-performans-analizi-13bdf5ff396f

