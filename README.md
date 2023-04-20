<h1 align = 'Center'>Nane&Limon 🐍 Teknofest 2023 TDDİ | Introduce</h1>

- Kullanılan model, huggingface üzerinden paylaşılmıştır. Modelin huggingface adresi, [buradan](https://huggingface.co/nanelimon/bert-base-insult-model/tree/main) erişilebilir.
- Kullanılan veri kümesi, huggingface üzerinden paylaşılmıştır. Veri kümesinin huggingface adresi, [buradan](https://huggingface.co/datasets/nanelimon/insult-dataset) erişilebilir.
- **Proje sunumu, Canva adlı çevrimiçi tasarım aracı kullanılarak hazırlanmıştır. Sunuma** [buradan](https://www.canva.com/design/DAFY4qojNxE/6cArTkFzRoPnZ8tsQW15ug/watch?utm_content=DAFY4qojNxE&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink) **erişilebilir.**


| No | Aşamalar | Açıklama |
| --- | --- | --- |
| 1 | [Exploratory Data Analysis](https://lookerstudio.google.com/reporting/92fe0588-0ada-4e17-9aaf-d988e430d88d) |Bu aşamada, veri seti analiz edilerek, veri seti hakkında önemli bilgiler elde edilmiştir. Bu bilgiler ışığında belirli iç görüler doğrultusunda veri ön işleme adımında gerekli reaksiyonlar alınmıştır. Ayrıca, veri setinde bulunan özellikler (features) kullanılarak Google Data Studio aracılığıyla bir dashboard raporu hazırlanmıştır. |
| 2 | [Model Baseline](https://github.com/Teknofest-Nane-Limon/model-baseline-insult) | [Model Baseline](https://github.com/Teknofest-Nane-Limon/model-baseline-insult/blob/main/baseline_model.ipynb), veri setinin temel özelliklerine göre oluşturulan ve kullanılan ilk modeldir. Bu model, daha sonra geliştirilen diğer modellerin performanslarının ölçülmesi ve karşılaştırılması için referans olarak kullanılmıştır. Model Baseline üzerinde yapılan deneylerde, veri seti üzerindeki temel özelliklerin ve veri ön işleme adımlarının etkileri incelenmiştir. Bu çalışmalar sonucunda, en iyi performans elde edebilmek için veri ön işleme adımlarının belirli bir sırayla uygulanması ve belirli parametre değerlerinin seçilmesi gerektiği belirlenmiştir. Model Baseline, diğer modellerin geliştirilmesi sürecinde bir referans noktası olarak kullanılarak, çalışmanın başarısına önemli katkılar sağlamıştır.| 
| 3 | [Mintlemon Turkish NLP](https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp) |[Mintlemon Turkish NLP](https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp) Kütüphanesi, henüz geliştirme aşamasında olan bir kütüphanedir. Bu kütüphane, yarışma kapsamında veri ön işleme adımlarının gerçekleştirilmesi için kullanılmıştır. Veri ön işleme aşamasında Normalizer modülü, mintlemon-turkish-nlp kütüphanesine eklenmiştir. Normalizer modülü, Türkçe metinlerdeki yazım hatalarını düzeltmek ve metinleri belirli bir formata getirmek için kullanılmıştır. Böylece, veri seti daha homojen ve işlenebilir bir hale getirilmiştir. Yarışmanın ardından da kütüphaneye katkı sağlamaya devam edeceğiz ve open-source olarak herkesin kullanımına açık bir kaynak haline getireceğiz. Bu sayede, geliştirmiş olduğumuz kütüphane, insanlar tarafından kullanılarak Türkçe doğal dil işleme alanında daha fazla gelişme kaydedebilecek. Amacımız, Türkçe doğal dil işleme alanına değerli bir kazanım sağlamak ve bu alanda çalışan herkesin işini kolaylaştırmak. Mint & Lemon Turkish NLP Kütüphanenin dökümantasyonuna ulaşmak için [tıklayınız.](https://mintlemon-turkish-nlp.readthedocs.io/en/latest/)|
| 4 | [Preprocessing Micro Service](https://github.com/Teknofest-Nane-Limon/preprocessing-micro-service) |[Preprocessing Micro Service](https://github.com/Teknofest-Nane-Limon/preprocessing-micro-service), parametrik hale getirilen bir FastAPI servisi olarak geliştirilmiştir ve Mintlemon Turkish NLP kütüphanesi kullanılarak Türkçe metinlerin çeşitli veri ön işleme adımlarından geçirilmesini sağlar. Bu araç, sayısal metinlerin normalleştirilmesi, noktalama işaretlerinin kaldırılması, Türkçe karakterlerin normalleştirilmesi, karakterlerin küçük harfe çevrilmesi ve kısa metinlerin kaldırılması gibi çeşitli veri ön işleme adımlarını içerir. Ayrıca, veri ön işleme adımları, kullanıcıların tercihlerine göre özelleştirilebilir ve Türkçe metinlerin özelliklerine uygun bir şekilde işlenmesi sağlanır. Bu sayede, FastAPI servisi olarak geliştirilen Preprocessing Micro Service, Türkçe doğal dil işleme alanında verimli bir veri ön işleme aracı sunarak, Türkçe metinlerin daha etkili bir şekilde işlenebilmesine katkı sağlamayı hedefler.|
| 5 | [Preprocessing Micro Service ~ Params Tuning](https://github.com/Teknofest-Nane-Limon/preprocessing-micro-service/blob/main/README.md) |[Preprocessing Micro Service](https://github.com/Teknofest-Nane-Limon/preprocessing-micro-service/blob/main/README.md), parametrik yapısı kullanılarak, yarışma kapsamında paylaşılan veri kümesi üzerinde, baseline bir modelin hangi veri ön işleme adımları kullanıldığında daha iyi sonuçlar elde edildiği ile ilgili bir çalışma yürütülmüştür. Çalışma kapsamında, elde edilen sonuçlar doğrultusunda,  veri kümesine ve modelin hedeflerine uygun en iyi veri ön işleme adımları seçilmiştir. Bu sayede, daha verimli ve doğru sonuçlar elde etmek mümkün olmaktadır. | 
| 6 | [SHAP Analysis](https://github.com/Teknofest-Nane-Limon/nlp-shap-exploration-teknofest-2023)| Bu çalışmada [Shap Analizi](https://github.com/Teknofest-Nane-Limon/nlp-shap-exploration-teknofest-2023) yöntemi kullanılarak modelin sınıflandırma performansı incelenmiştir. Analiz sonucunda paylaşılan veri setinin ekstra veriler ile desteklenmesi sonucunda model perfomransının artacağı belirlenmiştir. Bu sayede modelin daha doğru tahminler yapabilmesi hedeflenmektedir.
| 7 | Veri Setini Güçlendirmek| Veri setini güçlendirme aşamasında, mevcut veri setine ekstra metin verileri eklenmiştir bu veriler 2022 Teknofest sürecinde takımımız Nane&Limon tarafından hazırlanıp public paylaşılmış olan [turkish-social-media-bullying-dataset](https://huggingface.co/datasets/nanelimon/turkish-social-media-bullying-dataset). Bu işlem sonucunda, 12438 adet veriye ek shap analizi göz önünde bulundurularak 2578 adet yeni veri eklenmiştir. Bu sayede, veri seti daha zengin hale getirilmiş ve modelin öğrenme sürecine daha fazla veri eklenmiştir. Fakat eklenen verilerin modelin başarısını olumlu etkilemesi beklenirken model başarısını daha da düşürdüğü gözlemlenmiştir. Bunun nedeninin veri setinde yer alan çok sayıda yanlı veri olduğu düşünülmek ile birlikte test edilecek verinin yaklaşımı bilinmediği için ekleme yapılan veriseti yerine yarışmada paylaşılmış olan veri seti modelde kullanılmıştır. 
| 8 |[Multilabel Model](https://github.com/Teknofest-Nane-Limon/model-baseline-insult/blob/main/multi_label_BERT_model.ipynb)|[Multilabel Model](https://github.com/Teknofest-Nane-Limon/model-baseline-insult/blob/main/multi_label_BERT_model.ipynb) Aşaması, daha önceki aşamalarda kullanılan modellerin geliştirilmesi ve iyileştirilmesi için gerçekleştirilmiştir. Bu çalışmanın başarı oranını artırmıştır ve tam olarak %97 F-1 Macro Oranı yakalanmıştır. Bu başarı veriler üzerinde daha doğru sonuçlar elde edilmesini sağlamaktadır. Ayrıca, modelin daha önceki aşamalara göre daha doğru sonuçlar vermesi, çalışmanın genel başarı oranını artırmıştır. |
| 9 | [TDDI Model Service](https://github.com/Teknofest-Nane-Limon/tddi-model-service) | [TDDI Model Service](https://github.com/Teknofest-Nane-Limon/tddi-model-service), modelin deployment (dağıtım) işlemleri için oluşturulmuş bir FastAPI servisidir. Bu servis, oluşturulan modelin deploy edilmesiyle birlikte, modeli kullanarak tahmin yapabilme imkanı sağlar. Yani, bu servis üzerinden gelen istekler doğrultusunda, modelin tahmin yeteneği etkinleştirilerek, belirtilen girdilerle ilgili tahminler üretilir. 
| 10 | [Social Content Analysis Application](https://github.com/Teknofest-Nane-Limon/social-content-analysis-app) | [Sosyal medya içerik analizi uygulaması](https://github.com/Teknofest-Nane-Limon/social-content-analysis-app) , sosyal medya platformlarında paylaşılan içeriklerin analiz edilmesini sağlayan bir araçtır. Bu uygulama, belirli anahtar kelimeleri, hashtagleri ve marka isimlerini takip ederek, sosyal medya hesaplarına yapılan tüm paylaşımları izleyebilir ve analiz edebilir. Bu uygulamanın firmalar için önemi oldukça büyüktür örneğin firmalar, markaları hakkında sosyal medyada ne kadar bahsedildiğini, hangi konularda en çok konuşulduklarını, hangi kullanıcıların markalarıyla ilgilendiğini, ne tür bir etkileşim aldıklarını ve hangi kampanyaların en başarılı olduğunu öğrenebilirler. Bu bilgiler, firmaların pazarlama stratejilerini oluştururken ve mevcut stratejilerini geliştirirken yol gösterici olabilir. Firmalar ayrıca, sosyal medya içerik analizi uygulamaları ile rakiplerini de takip edebilirler. Bu sayede rakiplerinin ne tür kampanyalar yürüttüklerini, nasıl bir etkileşim aldıklarını ve hangi konularda daha başarılı olduklarını öğrenerek, kendi pazarlama stratejilerini rakiplerine göre ayarlayabilirler. Bu proje kapsamında yukarıdaki bütün adımlardan yararlanılarak ortaya bir ürün çıkarılmıştır. Verilerin toplaması için bir hastag takip job'ı yazılmıştır. [Buradan Twitter Hashtag Following Stream Job Çalışmasına ulaşabilirsiniz.](https://github.com/Teknofest-Nane-Limon/twitter_hashtag_following)
---
