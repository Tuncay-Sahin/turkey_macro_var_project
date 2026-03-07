# Ekonometrik Analiz Yorumları

Bu doküman, çalışmada tahmin edilen VAR modelinden elde edilen sonuçların ekonomik yorumunu sunmaktadır.

Analiz, **2019–2025** döneminde Türkiye’de tüketici güveni ile seçilmiş makroekonomik değişkenler arasındaki dinamik ilişkileri incelemektedir.

---

# Modelde Kullanılan Değişkenler

Analizde aşağıdaki değişkenler kullanılmıştır:

- TGE (Tüketici Güven Endeksi)
- USDTRY (Döviz kuru)
- CPI (Tüketici Fiyat Endeksi)
- IPI (Sanayi Üretim Endeksi)
- UNEMPLOYMENT (İşsizlik oranı)
- BIST (Borsa İstanbul endeksi)
- TLREF (Türk lirası referans faiz oranı)

Model durağanlaştırılmış seriler kullanılarak **VAR modeli** ile tahmin edilmiştir.

---

# Granger Nedensellik Sonuçlarının Yorumu

Granger nedensellik testi sonuçları, makroekonomik değişkenlerin birlikte ele alındığında **tüketici güvenini istatistiksel olarak anlamlı şekilde etkilediğini** göstermektedir.

Bu sonuç, makroekonomik gelişmelerin tüketici beklentileri üzerinde bilgi içerdiğini ve tüketici güveninin makroekonomik ortamdan bağımsız olmadığını göstermektedir.

---

# Impulse Response (IRF) Sonuçlarının Yorumu

IRF analizi, makroekonomik değişkenlerde meydana gelen şokların tüketici güveni üzerindeki dinamik etkilerini göstermektedir.

Genel olarak sonuçlar, şokların etkisinin **kısa dönemde ortaya çıktığını ve zamanla sönümlendiğini** göstermektedir.

## Döviz Kuru Şoku (USDTRY → TGE)

Döviz kuru şoklarının tüketici güveni üzerinde **kısa dönemde negatif bir etki oluşturduğu** görülmektedir.

Kur artışı genellikle enflasyon beklentilerini artırmakta ve ekonomik belirsizliği yükseltmektedir. Bu durum hanehalkı beklentilerinin bozulmasına neden olabilmektedir.

## Enflasyon Şoku (CPI → TGE)

Enflasyon şoklarının tüketici güveni üzerindeki etkisi **kısa süreli olup zamanla azalmaktadır**.

Bu durum tüketicilerin enflasyon gelişmelerine zaman içinde uyum sağlayabildiğini göstermektedir.

## Sanayi Üretimi Şoku (IPI → TGE)

Sanayi üretimindeki şokların tüketici güveni üzerindeki etkisi **görece sınırlı ve kısa sürelidir**.

Bu sonuç reel sektör gelişmelerinin tüketici beklentilerine dolaylı yoldan yansıdığını göstermektedir.

## İşsizlik Şoku (UNEMPLOYMENT → TGE)

İşsizlik oranındaki değişimlerin tüketici güveni üzerindeki etkisi **orta düzeyde ancak geçicidir**.

İşgücü piyasası gelişmeleri tüketici beklentileri açısından önemli olmakla birlikte finansal değişkenlere kıyasla daha zayıf etki göstermektedir.

## Finansal Piyasa Şoku (BIST → TGE)

Borsa şoklarının tüketici güveni üzerinde **kısa dönemli etkiler** yarattığı görülmektedir.

Finansal piyasalar ekonomik beklentiler açısından önemli bir gösterge niteliği taşımaktadır.

## Faiz Şoku (TLREF → TGE)

Faiz oranı şoklarının tüketici güveni üzerindeki etkisi **görece sınırlıdır**.

Türkiye’de tüketici güveninin çoğu zaman döviz kuru ve enflasyon gelişmelerine daha duyarlı olduğu gözlenmektedir.

---

# Varyans Ayrıştırması Yorumu

Varyans ayrıştırması sonuçları, tüketici güvenindeki değişimlerin büyük kısmının **kendi şokları tarafından açıklandığını** göstermektedir.

Bu durum tüketici güveninin belirli bir **kalıcılık (persistence)** özelliğine sahip olduğunu göstermektedir.

Bununla birlikte döviz kuru ve finansal değişkenlerin de tüketici güvenindeki dalgalanmaları açıklamada belirli bir rol oynadığı görülmektedir.

---

# Analiz Döneminin Ekonomik Bağlamı

Analizde kullanılan **2019–2025** dönemi Türkiye ekonomisi açısından oldukça önemli gelişmeleri içermektedir.

Bu dönemde:

- **COVID-19 pandemisi**
- önemli **döviz kuru oynaklıkları**
- yüksek **enflasyon süreçleri**
- **para politikası yöneliminde değişimler**

gözlenmiştir.

Bu nedenle analiz edilen dönem, tüketici güveninin makroekonomik ve finansal şoklara verdiği tepkilerin incelenmesi açısından önemli bir bağlam sunmaktadır.

---

# Genel Değerlendirme

Elde edilen sonuçlar, Türkiye’de tüketici güveninin özellikle **finansal değişkenlere ve döviz kuru hareketlerine duyarlı olduğunu** göstermektedir.

Sonuçlar ayrıca makroekonomik istikrarın ve ekonomik beklentilerin tüketici davranışlarının şekillenmesinde önemli bir rol oynadığını ortaya koymaktadır.

---

English

# Econometric Analysis Interpretation

This document provides an economic interpretation of the results obtained from the VAR model estimated in this study.

The analysis investigates the dynamic relationship between consumer confidence and selected macroeconomic variables in Turkey over the period **2019–2025**.

---

# Variables Used in the Model

The following variables are included in the analysis:

- TGE (Consumer Confidence Index)
- USDTRY (Exchange Rate)
- CPI (Consumer Price Index)
- IPI (Industrial Production Index)
- UNEMPLOYMENT (Unemployment Rate)
- BIST (Borsa Istanbul Stock Market Index)
- TLREF (Turkish Lira Reference Interest Rate)

The model is estimated using **stationary transformed series within a Vector Autoregression (VAR) framework**.

---

# Interpretation of Granger Causality Results

The results of the Granger causality test indicate that the set of macroeconomic variables **statistically and jointly influence consumer confidence**.

This finding suggests that macroeconomic developments contain predictive information about consumer expectations and that consumer confidence does not evolve independently of the broader macroeconomic environment.

---

# Interpretation of Impulse Response (IRF) Results

Impulse Response Function (IRF) analysis illustrates the dynamic reactions of consumer confidence to shocks in macroeconomic variables.

Overall, the results suggest that the effects of shocks **emerge in the short run and gradually dissipate over time**, indicating a relatively stable adjustment process.

## Exchange Rate Shock (USDTRY → TGE)

Exchange rate shocks appear to generate a **negative short-run impact** on consumer confidence.

Currency depreciation often increases inflation expectations and economic uncertainty, which may weaken household sentiment and future expectations.

## Inflation Shock (CPI → TGE)

Inflation shocks have **temporary effects on consumer confidence that fade over time**.

This suggests that consumers may gradually adjust their expectations in response to inflation developments.

## Industrial Production Shock (IPI → TGE)

Shocks to industrial production have **relatively limited and short-lived effects** on consumer confidence.

This result may indicate that real sector developments influence household expectations indirectly.

## Unemployment Shock (UNEMPLOYMENT → TGE)

Changes in unemployment appear to have **moderate but temporary effects** on consumer confidence.

Although labor market conditions are important for expectations, their influence appears weaker compared to financial variables.

## Financial Market Shock (BIST → TGE)

Stock market shocks generate **short-term fluctuations** in consumer confidence.

Financial markets may influence expectations through wealth effects and signals about the overall economic outlook.

## Interest Rate Shock (TLREF → TGE)

Interest rate shocks appear to have **relatively limited effects** on consumer confidence.

In the Turkish context, consumer sentiment often reacts more strongly to exchange rate movements and inflation dynamics than to short-term interest rate adjustments.

---

# Interpretation of Variance Decomposition

Variance decomposition results indicate that a large portion of fluctuations in consumer confidence is explained by **its own shocks**.

This finding suggests that consumer confidence exhibits a degree of **persistence over time**.

However, exchange rate movements and financial variables also contribute to explaining variations in consumer sentiment.

---

# Economic Context of the Analysis Period

The **2019–2025** period analyzed in this study includes several important macroeconomic developments in Turkey.

These include:

- the **COVID-19 pandemic**
- significant **exchange rate volatility**
- periods of **high inflation**
- **changes in monetary policy stance**

These structural developments provide an important context for examining how consumer confidence responds to macroeconomic and financial shocks.

---

# Overall Assessment

The results suggest that consumer confidence in Turkey is particularly **sensitive to financial variables and exchange rate movements**.

Overall, the findings highlight the importance of macroeconomic stability and economic expectations in shaping consumer behavior in emerging economies.