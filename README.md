# hse_hw1_meth
Изучение глобального изменения уровня CpG метилирования ДНК при раннем эмбриональном развитии мыши.

## Ссылка на Google Colab
[Methylation](https://colab.research.google.com/drive/1Yy5UmCxmQv71WKLueuSOW7T8VM9urvIa?usp=sharing)
## Задание 1
Сравним отчеты по анализу QC прямых прочтений для домашней мышки (Mus musculus) образца [SRR5836473_1](https://www.ebi.ac.uk/ena/browser/view/SRR5836473?show=reads) (**8cell**) и [SRR3414629_1](https://www.ebi.ac.uk/ena/browser/view/SRR3414629?show=reads) (**RNA-Seq**) 

8cell – 8-клеточный эмбрион, примерно 2.25 дня после оплодотворения яйцеклетки

RNA-Seq - последовательность РНК уже взрозлой мышки. 

| **8cell**     |           **RNA-Seq**            |
|----------------------------|---------------------------|
|Per sequence GC content     | Per sequence GC content    |
|![SRR5836473_GC](https://user-images.githubusercontent.com/60792064/154817884-2676a33f-5f97-4b54-8f17-67e0978c6207.png) | ![SRR3414629_GC](https://user-images.githubusercontent.com/60792064/154817893-478fc873-6147-4343-bd1a-ecfc1a73b38c.png)|

Видим практически индентичный уровень GC, т.к. на стадии развития 8cell метилирование ещё на низком уровне. 

## Задание 2
### Число ридов, закартированных на участки 11 хромосомы:
|                 | Epiblast | 8cell | ICM |
|-----------------|:---------|:------|:-----|
|11347700-11367700|2328      |1090   |1456 |
|40185800-40195800|1062      |464    |630  |

### Процентов дуплицированных прочтений в каждом из образцов:
|                 | Epiblast | 8cell | ICM |
|-----------------|:---------|:------|:-----|
|% дуплицированных|2.92%    |18.31%   |9.08% |

### M-Bias Plot
|                 | Epiblast | 8cell | ICM |
|-----------------|:---------|:------|:-----|
|![Bismark M-bias Read 1 (1)](https://user-images.githubusercontent.com/60792064/155027279-21b34b58-c5b3-4708-8b3c-2f3c370906e2.png)|![Bismark M-bias Read 1](https://user-images.githubusercontent.com/60792064/155027233-a789414b-1390-428c-8951-af82872cd9ef.png)  |![Bismark M-bias Read 1 (2)](https://user-images.githubusercontent.com/60792064/155027309-eb0ab5a4-c9e9-4225-a80a-9b68d03acddf.png) |
На графиках можем наблюдать, что 


### Уровень метилирования и покрытия для каждого образца:
![image_cov_9](https://user-images.githubusercontent.com/60792064/155025544-0f9ce294-f1dc-483c-ad6e-d29c39c224d1.png)
На графиках наблюдаем, что покрытие сконцентрировано в райноне 11 хромосомы. Уровень метилирования в случае Эпибласта выше, чем в двух двугих.
