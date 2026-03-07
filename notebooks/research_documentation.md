Author: Tuncay Şahin  
Project: Turkey Macro VAR Project  
Tools: Python, pandas, statsmodels  
Period: 2019–2025

Macroeconomic Determinants of Consumer Confidence in Turkey:
A VAR Analysis (2019–2025)

# Introduction / Giriş

## English

Consumer confidence is widely regarded as an important indicator of households’ expectations about future economic conditions. Changes in consumer sentiment can influence consumption behavior, savings decisions, and overall economic activity.

In emerging economies such as Turkey, macroeconomic volatility, exchange rate movements, inflation dynamics, and financial market conditions may significantly affect consumer expectations. Understanding the dynamic relationship between macroeconomic variables and consumer confidence therefore has important implications for economic policy and forecasting.

This study investigates the dynamic interactions between consumer confidence and selected macroeconomic indicators in Turkey over the period **2019–2025**. Using a **Vector Autoregression (VAR) model**, the analysis examines whether macroeconomic shocks—such as exchange rate movements, inflation changes, production dynamics, financial market fluctuations, and interest rate adjustments—have predictive power over consumer confidence.

The analyzed period includes major macroeconomic disturbances such as the **COVID-19 pandemic**, episodes of **exchange rate volatility**, and significant **shifts in monetary policy stance in Turkey**. These structural developments provide a valuable environment to analyze how consumer confidence responds to macroeconomic and financial shocks.

The study contributes to the literature by providing a **Python-based reproducible econometric analysis** using recent Turkish macroeconomic data.

---

Türkiye’de Tüketici Güveninin Makroekonomik Belirleyicileri:
VAR Analizi (2019–2025)

## Türkçe

Tüketici güveni, hanehalklarının gelecekteki ekonomik koşullara ilişkin beklentilerini yansıtan önemli göstergelerden biridir. Tüketici beklentilerindeki değişimler tüketim davranışını, tasarruf kararlarını ve genel ekonomik faaliyetleri etkileyebilmektedir.

Türkiye gibi gelişmekte olan ekonomilerde döviz kuru hareketleri, enflasyon dinamikleri, finansal piyasa koşulları ve makroekonomik dalgalanmalar tüketici beklentilerini önemli ölçüde etkileyebilmektedir. Bu nedenle makroekonomik değişkenler ile tüketici güveni arasındaki dinamik ilişkilerin anlaşılması ekonomik politika ve tahminler açısından büyük önem taşımaktadır.

Bu çalışma **2019–2025** döneminde Türkiye’de tüketici güveni ile seçilmiş makroekonomik göstergeler arasındaki dinamik ilişkileri incelemektedir. Analizde **Vector Autoregression (VAR) modeli** kullanılarak döviz kuru, enflasyon, sanayi üretimi, finansal piyasalar, işsizlik ve faiz oranlarındaki şokların tüketici güveni üzerindeki etkileri araştırılmaktadır.

Analiz edilen dönem aynı zamanda **COVID-19 pandemisini**, önemli **döviz kuru oynaklıklarını** ve Türkiye’de **para politikası yöneliminde yaşanan değişimleri** içermektedir. Bu yapısal gelişmeler tüketici güveninin makroekonomik ve finansal şoklara verdiği tepkilerin incelenmesi açısından önemli bir analiz ortamı sunmaktadır.

Bu çalışma ayrıca güncel Türkiye verilerini kullanarak **Python tabanlı tekrarlanabilir bir ekonometrik analiz** sunarak literatüre katkı sağlamaktadır.

---

# Data / Veri

## English

The dataset used in this study consists of monthly macroeconomic observations for Turkey covering the period **January 2019 – December 2025**. The data were collected from official statistical sources and financial databases.

The variables included in the analysis are:

| Variable     | Description                          |
| ------------ | ------------------------------------ |
| TGE          | Consumer Confidence Index            |
| USDTRY       | Exchange Rate                        |
| CPI          | Consumer Price Index                 |
| IPI          | Industrial Production Index          |
| UNEMPLOYMENT | Unemployment Rate                    |
| BIST         | Borsa Istanbul Stock Market Index    |
| TLREF        | Turkish Lira Reference Interest Rate |

To ensure stationarity, all variables were transformed using **log-difference transformations**, which represent growth rates or percentage changes.

---

## Türkçe

Bu çalışmada kullanılan veri seti **Ocak 2019 – Aralık 2025** dönemini kapsayan aylık makroekonomik gözlemlerden oluşmaktadır. Veriler resmi istatistik kaynakları ve finansal veri tabanlarından elde edilmiştir.

Analizde kullanılan değişkenler aşağıdaki gibidir:

| Değişken     | Açıklama                        |
| ------------ | ------------------------------- |
| TGE          | Tüketici Güven Endeksi          |
| USDTRY       | Döviz Kuru                      |
| CPI          | Tüketici Fiyat Endeksi          |
| IPI          | Sanayi Üretim Endeksi           |
| UNEMPLOYMENT | İşsizlik Oranı                  |
| BIST         | Borsa İstanbul Endeksi          |
| TLREF        | Türk Lirası Referans Faiz Oranı |

Zaman serilerinin durağanlığını sağlamak amacıyla tüm değişkenler **logaritmik fark dönüşümü (log-difference)** kullanılarak büyüme oranlarına dönüştürülmüştür.

---

# Methodology / Metodoloji

## English

To analyze the dynamic relationships between the variables, a **Vector Autoregression (VAR) model** is employed.

The VAR framework allows each variable in the system to be explained by its own past values and the past values of all other variables.

The empirical analysis follows these steps:

1. Data collection and preprocessing  
2. Stationarity testing using the **Augmented Dickey–Fuller (ADF) test**  
3. Log-difference transformations  
4. Lag order selection using **information criteria (AIC, BIC, HQIC)**  
5. Estimation of the VAR model  
6. Granger causality analysis  
7. Impulse Response Functions (IRF)  
8. Forecast Error Variance Decomposition (FEVD)

All computations are implemented in **Python using pandas, numpy, and statsmodels libraries**.

---

## Türkçe

Değişkenler arasındaki dinamik ilişkileri incelemek amacıyla **Vector Autoregression (VAR) modeli** kullanılmıştır.

VAR modeli, sistemdeki her değişkenin hem kendi gecikmeli değerleri hem de diğer değişkenlerin gecikmeli değerleri tarafından açıklanmasına olanak sağlar.

Ampirik analiz aşağıdaki adımlardan oluşmaktadır:

1. Veri toplama ve ön işleme  
2. **Augmented Dickey–Fuller (ADF) testi** ile durağanlık analizi  
3. Logaritmik fark dönüşümü  
4. **Bilgi kriterleri (AIC, BIC, HQIC)** kullanılarak gecikme seçimi  
5. VAR model tahmini  
6. Granger nedensellik analizi  
7. Impulse Response Fonksiyonları (IRF)  
8. Varyans ayrıştırması (FEVD)

Tüm hesaplamalar **Python ortamında pandas, numpy ve statsmodels kütüphaneleri kullanılarak gerçekleştirilmiştir.**

---

# Results / Bulgular

## English

The Granger causality test results indicate that the set of macroeconomic variables jointly Granger-cause changes in consumer confidence at the **5% significance level**.

Impulse response analysis shows that shocks to financial variables, particularly **exchange rates and stock market movements**, generate noticeable responses in consumer confidence. These effects tend to be strongest in the short run and gradually dissipate over time.

Variance decomposition results reveal that most of the forecast error variance in consumer confidence is explained by its own shocks, indicating strong persistence. However, exchange rate and financial market variables contribute non-negligibly to the variation in consumer sentiment.

---

## Türkçe

Granger nedensellik testi sonuçları, makroekonomik değişkenlerin birlikte ele alındığında **%5 anlamlılık düzeyinde tüketici güvenini Granger anlamında etkilediğini** göstermektedir.

Impulse response analizi, özellikle **döviz kuru ve borsa hareketlerindeki şokların** tüketici güveninde belirgin tepkiler oluşturduğunu göstermektedir. Bu etkiler genellikle kısa dönemde güçlü olup zamanla sönümlenmektedir.

Varyans ayrıştırması sonuçları, tüketici güvenindeki değişimlerin büyük kısmının kendi şoklarından kaynaklandığını göstermektedir. Bununla birlikte döviz kuru ve finansal piyasa değişkenleri tüketici güvenindeki dalgalanmaların önemli bir bölümünü açıklamaktadır.

---

# Conclusion / Sonuç

## English

This study examines the dynamic relationship between consumer confidence and key macroeconomic variables in Turkey using a VAR framework.

The results suggest that consumer confidence responds to macroeconomic developments, particularly those related to financial markets and exchange rate dynamics.

Overall, the findings highlight the importance of financial stability and macroeconomic expectations in shaping consumer sentiment in emerging economies.

---

## Türkçe

Bu çalışma Türkiye’de tüketici güveni ile temel makroekonomik değişkenler arasındaki dinamik ilişkileri VAR modeli kullanarak incelemiştir.

Elde edilen bulgular, tüketici güveninin özellikle finansal piyasalar ve döviz kuru hareketleri gibi makroekonomik gelişmelere duyarlı olduğunu göstermektedir.

Sonuç olarak finansal istikrar ve makroekonomik beklentilerin gelişmekte olan ekonomilerde tüketici güveninin şekillenmesinde önemli bir rol oynadığı söylenebilir.

---