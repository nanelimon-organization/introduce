<h1 align = 'Center'>Nane&Limon 🐍 Teknofest 2023 TDDİ | Introduce</h1>

| No | Aşamalar | Açıklama |
| --- | --- | --- |
| 1 | [Model Baseline](https://github.com/Teknofest-Nane-Limon/model-baseline-insult/blob/main/baseline_model.ipynb) | [Model Baseline](https://github.com/Teknofest-Nane-Limon/model-baseline-insult/blob/main/baseline_model.ipynb), veri setinin temel özelliklerine göre oluşturulan ve kullanılan ilk modeldir. Bu model, daha sonra geliştirilen diğer modellerin performanslarının ölçülmesi ve karşılaştırılması için referans olarak kullanılmıştır. Model Baseline üzerinde yapılan deneylerde, veri seti üzerindeki temel özelliklerin ve veri ön işleme adımlarının etkileri incelenmiştir. Bu çalışmalar sonucunda, en iyi performans elde edebilmek için veri ön işleme adımlarının belirli bir sırayla uygulanması ve belirli parametre değerlerinin seçilmesi gerektiği belirlenmiştir. Model Baseline, diğer modellerin geliştirilmesi sürecinde bir referans noktası olarak kullanılarak, çalışmanın başarısına önemli katkılar sağlamıştır.| 
| 2 | [Exploratory Data Analysis](https://lookerstudio.google.com/reporting/92fe0588-0ada-4e17-9aaf-d988e430d88d) |Bu aşamada, veri seti analiz edilerek, veri seti hakkında önemli bilgiler elde edilmiştir. Bu bilgiler ışığında belirli iç görüler doğrultusunda veri ön işleme adımında gerekli reaksiyonlar alınmıştır. Ayrıca, veri setinde bulunan özellikler (features) kullanılarak Google Data Studio aracılığıyla bir dashboard raporu hazırlanmıştır. |
| 3 | [Mintlemon Turkish NLP](https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp) |[Mintlemon Turkish NLP](https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp) Kütüphanesi, henüz geliştirme aşamasında olan bir kütüphanedir. Bu kütüphane, yarışma kapsamında veri ön işleme adımlarının gerçekleştirilmesi için kullanılmıştır. Veri ön işleme aşamasında Normalizer modülü, mintlemon-turkish-nlp kütüphanesine eklenmiştir. Normalizer modülü, Türkçe metinlerdeki yazım hatalarını düzeltmek ve metinleri belirli bir formata getirmek için kullanılmıştır. Böylece, veri seti daha homojen ve işlenebilir bir hale getirilmiştir. Yarışmanın ardından da kütüphaneye katkı sağlamaya devam edeceğiz ve open-source olarak herkesin kullanımına açık bir kaynak haline getireceğiz. Bu sayede, geliştirmiş olduğumuz kütüphane, insanlar tarafından kullanılarak Türkçe doğal dil işleme alanında daha fazla gelişme kaydedebilecek. Amacımız, Türkçe doğal dil işleme alanına değerli bir kazanım sağlamak ve bu alanda çalışan herkesin işini kolaylaştırmak. |
| 4 | [Preprocessing Micro Service](https://github.com/Teknofest-Nane-Limon/preprocessing-micro-service) |[Preprocessing Micro Service](https://github.com/Teknofest-Nane-Limon/preprocessing-micro-service), parametrik hale getirilen bir FastAPI servisi olarak geliştirilmiştir ve Mintlemon Turkish NLP kütüphanesi kullanılarak Türkçe metinlerin çeşitli veri ön işleme adımlarından geçirilmesini sağlar. Bu araç, sayısal metinlerin normalleştirilmesi, noktalama işaretlerinin kaldırılması, Türkçe karakterlerin normalleştirilmesi, karakterlerin küçük harfe çevrilmesi ve kısa metinlerin kaldırılması gibi çeşitli veri ön işleme adımlarını içerir. Ayrıca, veri ön işleme adımları, kullanıcıların tercihlerine göre özelleştirilebilir ve Türkçe metinlerin özelliklerine uygun bir şekilde işlenmesi sağlanır. Bu sayede, Flask API servisi olarak geliştirilen Preprocessing Micro Service, Türkçe doğal dil işleme alanında verimli bir veri ön işleme aracı sunarak, Türkçe metinlerin daha etkili bir şekilde işlenebilmesine katkı sağlamayı hedefler.|
| 5 | [Preprocessing Micro Service ~ Params Tuning](https://github.com/Teknofest-Nane-Limon/preprocessing-micro-service/blob/main/README.md) |[Preprocessing Micro Service](https://github.com/Teknofest-Nane-Limon/preprocessing-micro-service/blob/main/README.md), parametrik yapısı kullanılarak, yarışma kapsamında paylaşılan veri kümesi üzerinde, baseline bir modelin hangi veri ön işleme adımları kullanıldığında daha iyi sonuçlar elde edildiği ile ilgili bir çalışma yürütülmüştür. Çalışma kapsamında, elde edilen sonuçlar doğrultusunda,  veri kümesine ve modelin hedeflerine uygun en iyi veri ön işleme adımları seçilmiştir. Bu sayede, daha verimli ve doğru sonuçlar elde etmek mümkün olmaktadır. | 
| 6 | [SHAP Analysis](https://github.com/Teknofest-Nane-Limon/nlp-shap-exploration-teknofest-2023)| Bu çalışmada [Shap Analizi](https://github.com/Teknofest-Nane-Limon/nlp-shap-exploration-teknofest-2023) yöntemi kullanılarak modelin sınıflandırma performansı incelenmiştir. Analiz sonucunda paylaşılan veri setinin ekstra veriler ile desteklenmesi sonucunda model perfomransının artacağı belirlenmiştir. Bu sayede modelin daha doğru tahminler yapabilmesi hedeflenmektedir.
| 7 | Veri Setini Güçlendirmek| Veri setini güçlendirme aşamasında, mevcut veri setine ekstra metin verileri eklenmiştir. Bu işlem sonucunda, 12438 adet veriye ek olarak 2578 adet yeni veri eklenmiştir. Bu sayede, veri seti daha zengin hale getirilmiş ve modelin öğrenme sürecine daha fazla veri eklenmiştir. Eklenen bu veriler sayesinde, model daha çeşitli örnekler gördüğü için daha genel bir öğrenme yapmıştır. Sonuç olarak, modelin performansı artmış ve daha doğru tahminler yapması sağlanmıştır. Toplam gözlem birimi sayısı sayısı 15016'ya yükseltilmiştir.| 
| 8 |[Multilabel Model](https://github.com/Teknofest-Nane-Limon/model-baseline-insult/blob/main/multi_label_BERT_model.ipynb)|[Multilabel Model](https://github.com/Teknofest-Nane-Limon/model-baseline-insult/blob/main/multi_label_BERT_model.ipynb) Aşaması, daha önceki aşamalarda kullanılan modellerin geliştirilmesi ve iyileştirilmesi için gerçekleştirilmiştir. Bu çalışmanın başarı oranını artırmıştır ve veriler üzerinde daha doğru sonuçlar elde edilmesini sağlamaktadır. Ayrıca, modelin daha önceki aşamalara göre daha doğru sonuçlar vermesi, çalışmanın genel başarı oranını artırmıştır. |
| 9 | [TDDI Model Service](https://github.com/Teknofest-Nane-Limon/tddi-model-service) | [TDDI Model Service](https://github.com/Teknofest-Nane-Limon/tddi-model-service), modelin deployment (dağıtım) işlemleri için oluşturulmuş bir Flask API servisidir. Bu servis, oluşturulan modelin deploy edilmesiyle birlikte, modeli kullanarak tahmin yapabilme imkanı sağlar. Yani, bu servis üzerinden gelen istekler doğrultusunda, modelin tahmin yeteneği etkinleştirilerek, belirtilen girdilerle ilgili tahminler üretilir. 


---

## İçerik Analizi Uygulamasının Yaşam Döngüsü 

![App Diagram](https://user-images.githubusercontent.com/83168207/230263726-4862b2a5-dca4-4981-a41d-41078f2cfc37.jpeg)

