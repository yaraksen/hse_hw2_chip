# HW2 Aksenov Yaroslav

[Ссылка на ноутбук](https://colab.research.google.com/drive/1ZmI5s741ohVx_3H157ZiU7nh8xiAt4ZY?usp=sharing)

Использовалась клеточная линия HCT116 и гистоновая метка H3K9me3.

[FastQC отчет на первую реплику ENCFF002AAK](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/reports/ENCFF002AAK_fastqc.html)

[FastQC отчет на вторую реплику ENCFF002AAM](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/reports/ENCFF002AAM_fastqc.html)

[FastQC отчет на контроль ENCFF000VCW](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/reports/ENCFF000VCW_fastqc.html)


## Статистика по выравниванию на 14 хромосому

|                           | ENCFF002AAK       | ENCFF002AAM       | ENCFF000VCW       |
|---------------------------|-------------------|-------------------|-------------------|
| Общее число ридов         | 38104646          | 36969802          | 992928          |
| Не выровнившиеся          | 30201511 (79.26%) | 29362191 (79.42%) | 19920257 (86.64%) |
| Выровнившиеся уникально   | 1793051 (4.71%)   | 1809562 (4.89%)   | 779679 (3.39%)    |
| Выровнившиеся неуникально | 6110084 (16.04%)  | 5798049 (15.68%)  | 92992 (9.97%)   |

### Графики из анализа

ENCFF002AAK | ENCFF002AAM | ENCFF000VCW
--- | --- | ---
![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/basic_ENCFF002AAK.png) | ![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/basic_ENCFF002AAM.png) | ![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/basic_ENCFF000VCW.png)

![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/perseq_quality_ENCFF002AAK.png) | ![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/perseq_quality_ENCFF002AAM.png) | ![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/perseq_quality_ENCFF000VCW.png)

![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/perbase_quality_ENCFF002AAK.png) | ![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/perbase_quality_ENCFF002AAM.png) | ![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/perbase_quality_ENCFF000VCW.png)

![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/perbase_content_ENCFF002AAK.png) | ![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/perbase_content_ENCFF002AAM.png) | ![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/perbase_content_ENCFF000VCW.png)

![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/per_seq_gc_content_ENCFF002AAK.png) | ![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/per_seq_gc_content_ENCFF002AAM.png) | ![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/per_seq_gc_content_ENCFF000VCW.png)

![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/per_base_n_content_ENCFF002AAK.png) | ![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/per_base_n_content_ENCFF002AAM.png) | ![image](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/per_base_n_content_ENCFF000VCW.png)

## Диаграммы Эйлера-Венна

### Пересечение пиков 1 реплики и ENCODE
![Intervene_venn1](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/Intervene_venn.pdf) | ![Intervene_venn2](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/Intervene_venn1.pdf)

### Пересечение пиков 2 реплики и ENCODE
![Intervene_venn3](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/Intervene_venn2.pdf) | ![Intervene_venn4](https://github.com/yaraksen/hse_hw2_chip/blob/main/data/images/Intervene_venn3.pdf)

**Количество пересечений получилось таким низким, так как выравнивали риды на одну хромосому, составляющую небольшую часть человеческого генома. В ENCODE пиков намного больше, потому что они составлены для всех хромосом.**