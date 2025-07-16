# 🧠 Sıfırdan TF-IDF ile Metin Sınıflandırıcı Yazmak - Bölüm 2

Bu proje, metin verileri üzerinde **TF-IDF (Term Frequency-Inverse Document Frequency)** algoritmasını sıfırdan anlamayı ve uygulamayı amaçlar.  
Notebook, Python kullanarak TF, IDF ve TF-IDF skorlarının manuel hesaplamasını öğretir ve ardından basit bir **Naive Bayes sınıflandırıcı** ile temel bir metin sınıflandırma yapılır.

---

## 📌 İçerik

- Küçük bir Türkçe cümle veri seti oluşturma  
- Metin temizleme ve tokenization  
- TF (Terim Frekansı) hesaplama  
- IDF (Ters Belge Frekansı) hesaplama  
- TF-IDF vektörlerinin oluşturulması  
- Cümleleri sayısal forma dönüştürme  
- `Multinomial Naive Bayes` modeliyle örnek sınıflandırma


# 🧠 Bölüm 3: scikit-learn ile TF-IDF ve Gerçek Model Eğitimi

Bu bölümde, önceki adımlarda öğrendiğimiz TF-IDF kavramını artık gerçek dünyaya daha yakın bir senaryo ile uyguluyoruz.

Bu kez:

    Daha geniş ve dengeli bir Türkçe veri seti kullanıyoruz (20 cümle)

    Verileri .csv yerine doğrudan Python içinde tanımlıyoruz

    TfidfVectorizer kullanarak TF-IDF vektörlerini otomatik oluşturuyoruz

    MultinomialNB algoritması ile modeli eğitiyoruz

    Eğitim/test bölmesi (train_test_split) ve doğruluk ölçümleri yapıyoruz

    Ek olarak: cross_val_score ile 5-Fold Cross Validation uygulanıyor

📋 Bu bölümde neler var?

    Genişletilmiş metin veri listesi (csv gerekmez)

    TF-IDF vektörleştirme (scikit-learn ile)

    Etiketlerin LabelEncoder ile sayısallaştırılması

    Eğitim/test ayrımı (train_test_split)

    Model eğitimi: Multinomial Naive Bayes

    Model değerlendirme:

        Accuracy

        Classification report

        5-Fold Cross Validation

    Test cümle tahmini ile gerçek zamanlı sınıflandırma


## 🚀 Çalıştırmak için


## 🔍 Neden Bu Ekstra Kod Var?

Önceki bölümlerde kullanılan küçük veri seti, modelin doğruluğunu tam anlamıyla değerlendirmeye uygun değildi.
Bu nedenle Bölüm 3'teki ek kod, daha geniş bir veri listesiyle şunları sağlar:

    Gerçekçi model değerlendirmesi

    Eğitim ve test için dengeli örnekler

    Farklı veri bölmelerinde başarımı test etme (Cross-Validation)

    Yeni cümlelerle sınıflandırmayı gözlemleme

## 📂 Dosya Açıklamaları (Güncel)
Dosya Adı	Açıklama
tfidf_text_classifier_bolum2.ipynb	TF, IDF ve TF-IDF'i sıfırdan hesaplayan notebook
tfidf_text_classifier_bolum3.ipynb	Geniş veriyle çalışan, scikit-learn destekli sınıflandırma
