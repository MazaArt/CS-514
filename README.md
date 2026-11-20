# CS 514 — Online Convex Optimization

## Contents

- **`Bandit-Convex-Optimization-Notes/`** — Presentation notes on Bandit Convex
  Optimization (Hazan, *Introduction to Online Convex Optimization*, Ch. 6.1–6.3):
  the BCO setting, the multi-armed bandit reduction, the simple MAB and EXP3
  algorithms with unbiased loss estimators and regret bounds, and the general
  reduction from bandit feedback to first-order OCO via randomized gradient
  estimation. (`main.tex`, compiled `main.pdf`)

- **`Robust-Option-Pricing-OCO-Paper/`** — Final research overview paper,
  *Financial Online Convex Optimization* (Artem Ivaniuk & Khyaati Sigicherla),
  reviewing DeMarzo, Kremer & Mansour (2006) and Abernethy, Frongillo & Wibisono
  (2012): deriving pathwise, no-arbitrage option-price bounds from online-trading
  regret guarantees, and showing the minimax hedging game converges to
  Black–Scholes in the high-frequency limit. (`main.tex`, `references.bib`,
  compiled `main.pdf`)

## Building

```bash
# Bandit notes
cd Bandit-Convex-Optimization-Notes && pdflatex main.tex && pdflatex main.tex

# OCO paper (has a bibliography)
cd Robust-Option-Pricing-OCO-Paper && pdflatex main.tex && bibtex main && pdflatex main.tex && pdflatex main.tex
```
