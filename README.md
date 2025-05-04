readme_tr = """
# Tweet Temizleme Pipeline (Türkçe)

Bu proje, [Sentiment140](http://help.sentiment140.com/for-students) veri kümesinden alınan 100 tweet örneği üzerinde 11 aşamalı bir metin ön işleme sürecini içermektedir. Bu işlemler, doğal dil işleme (NLP) görevleri öncesinde veriyi uygun hale getirmeyi amaçlamaktadır.

## Uygulanan 11 Adım:

1. **Küçük Harfe Çevirme (Lowercasing)**  
2. **HTML Etiketlerini Kaldırma**  
3. **URL Temizleme**  
4. **Noktalama İşaretlerini Kaldırma**  
5. **ChatWords Dönüştürme**  
6. **Yazım Düzeltme (ilk 10 tweet)**  
7. **Stopword Temizliği**  
8. **Emoji Temizliği**  
9. **Tokenizasyon**  
10. **Stemming (Kök Bulma)**  
11. **Lemmatizasyon**

## Kullanılan Araçlar:
- Python
- Pandas, re
- NLTK, TextBlob, emoji

## Nasıl Kullanılır:
1. Colab ortamında çalıştırın.
2. Gerekli paketleri yükleyin.
3. `training.1600000.processed.noemoticon.csv` dosyasını Google Drive'a yükleyin.
4. Notebook'u adım adım çalıştırın.

"""

readme_en = """
# Tweet Preprocessing Pipeline (English)

This project demonstrates an 11-step text preprocessing pipeline on a sample of 100 tweets from the [Sentiment140](http://help.sentiment140.com/for-students) dataset. These steps aim to prepare text for natural language processing (NLP) tasks.

## 11 Steps Applied:

1. **Lowercasing**  
2. **Removing HTML Tags**  
3. **Removing URLs**  
4. **Removing Punctuation**  
5. **ChatWords Normalization**  
6. **Spelling Correction (first 10 tweets)**  
7. **Stopwords Removal**  
8. **Emoji Removal**  
9. **Tokenization**  
10. **Stemming**  
11. **Lemmatization**

## Tools Used:
- Python
- Pandas, re
- NLTK, TextBlob, emoji

## How to Use:
1. Open in Google Colab.
2. Install required packages.
3. Upload `training.1600000.processed.noemoticon.csv` to your Google Drive.
4. Run the notebook step by step.
"""

# Kaydet
with open("/mnt/data/README_TR.md", "w", encoding="utf-8") as f:
    f.write(readme_tr.strip())

with open("/mnt/data/README_EN.md", "w", encoding="utf-8") as f:
    f.write(readme_en.strip())
