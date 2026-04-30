#  BIST100 Monte Carlo Risk Analizi

Geometric Brownian Motion (GBM) ile BIST100 üzerinde Monte Carlo simülasyonu.

##  Proje Hakkında
- 2020–2024 gerçek BIST100 verisi kullanıldı
- 10.000 senaryo × 30 günlük fiyat yolu simüle edildi
- VaR ve CVaR ile risk ölçümü yapıldı

##  Bulgular (100.000 TL yatırım, 30 gün)
| Metrik | Değer |
|--------|-------|
| Beklenen değer | 105.306 TL |
| VaR %95 | -11.154 TL |
| CVaR %95 | -14.761 TL |
| Kâr olasılığı | %68 |

##  Temel Parametreler
| Parametre | Değer |
|-----------|-------|
| Yıllık getiri (μ) | %43.35 |
| Yıllık volatilite (σ) | %28.92 |
| Kurtosis | 4.53 (kalın kuyruk!) |
| Skewness | -0.72 (sola çarpık) |

##  Kullanılan Teknolojiler
![Python](https://img.shields.io/badge/Python-3.x-blue)
![NumPy](https://img.shields.io/badge/NumPy-✓-blue)
![Pandas](https://img.shields.io/badge/Pandas-✓-blue)
![Matplotlib](https://img.shields.io/badge/Matplotlib-✓-blue)

## Yöntem
Geometric Brownian Motion:

$$S_{t+\Delta t} = S_t \cdot \exp\left[(\mu - \frac{\sigma^2}{2})\Delta t + \sigma\sqrt{\Delta t}\cdot\varepsilon\right]$$


