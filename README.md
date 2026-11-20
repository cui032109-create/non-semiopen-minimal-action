# A minimal action of two commuting maps with no semi-open nonidentity element

[English paper (PDF)](semiopen-actions.pdf) · [中文全文](paper.zh-CN.md) · [LaTeX source](semiopen-actions.tex)

在一个紧致、道路连通、可度量的空间上，两个交换的连续满射可以生成极小作用，同时每个非恒等作用映射都把某个非空开集映满同一个闭的无处稠密集。中文全文包含联合极小性的证明、各个开集的构造和文献出处。

For the constructed action of $\mathbb N_0^2$, each nonzero $(m,n)$ admits a nonempty open set $U_{m,n}$ with $s^m r^n(U_{m,n})=D$, where $D$ is one fixed closed nowhere dense slice. The system itself is a factor of a minimal action by open maps.

The result answers the existence question in §1.2, footnote 1 of Blahodatna, Detmold, Glasscock and Le. Taking one generator as a self-factor also answers the metrizable branch of Question 5.2.4 of Dai, Feng, Lv and Xie. [First question](https://arxiv.org/abs/2610.10397v1) · [Second question](https://arxiv.org/html/2601.03380v2#S5.SS2)

## Build the PDF

From the repository root, run the following commands with a standard TeX Live installation. The bibliography is included in the source.

```sh
pdflatex -interaction=nonstopmode -halt-on-error semiopen-actions.tex
pdflatex -interaction=nonstopmode -halt-on-error semiopen-actions.tex
```

## Provenance

OpenAI's ChatGPT generated the counterexample and an initial proof in response to the research question and assisted in preparing the English and Chinese manuscripts.
