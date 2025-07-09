# TradingView Pine Script Dashboard – Unterstützung für LuxAlgo SMC

## 🎯 Ziel

Ein kompakter, dynamischer Indikator zur Unterstützung des LuxAlgo SMC-Indicators.

Das Ziel ist es, ein Live-Dashboard auf dem Chart zu haben, das:

- die wichtigsten Smart Money Concepts (SMC) überwacht
- mögliche Long- oder Short-Setups erkennt (nach klaren Regeln)
- alle Infos übersichtlich und farblich codiert darstellt
- nur Setups anzeigt, die aktuell für den gewählten Timeframe gültig sind
- die letzten 3–5 abgeschlossenen Setups zur Lernhilfe anzeigt

## 📦 Komponenten des Dashboards

1. **Trend-Zeitfenster-Anzeige (Multi-Timeframe Trend Check)**
   - 4 farbliche Boxen für die Trends der Zeitrahmen: 1m, 5m, 15m, 1h
   - Farbe: 🟩 Grün = Bullisch, 🟥 Rot = Bärisch, ⬜️ Grau = Seitwärts
   - Unabhängig vom aktuellen Timeframe

2. **Setup-Matrix für den aktuellen Chart (Live & kontextsensitiv)**
   - Zeigt nur Setups für den aktiven Timeframe
   - Dynamisches Update bei Chart-Wechsel
   - Zwei Sektionen: Long & Short Setup mit je 4 Kriterien (Liquidity Grab, CHoCH, OB, FVG)
   - Farbcode: ✅ erfüllt (grün), ❌ nicht erfüllt (rot), ⚪️ neutral (grau)
   - Zusammenfassende Gültigkeit

3. **Rückblick: Letzte Setups (Backtest-Helper)**
   - Zeigt die letzten 3–5 vollständigen Setups im Chart
   - Markiert Entry, Reaktion (TP/SL), Setup-Typ etc.
   - Optional im Dashboard: Statusübersicht

## 🛠️ Was vom LuxAlgo-SMC übernommen wird

LuxAlgo liefert:
- CHoCH & BOS
- Orderblocks
- FVGs
- Liquidity (Swing High/Low)

Diese Signale werden gelesen/genutzt, nicht neu berechnet.

## 📌 Zusätzliche Funktionen (optional)

- Umschaltfunktion: Nur Long, nur Short, beide anzeigen
- Optionaler Button: „Letzte Setups anzeigen/ausblenden“
- Kompaktes, verschiebbares UI

## ✅ Fazit

Dieses Pine Script erstellt ein visuelles Live-Dashboard, das Long- und Short-Setups gemäß Smart Money Concepts (in Zusammenarbeit mit LuxAlgo SMC) live auswertet. Es berücksichtigt den aktiven Timeframe, zeigt relevante Setups und die letzten 3–5 Setups zur Analyse an. Multi-Timeframe-Trend hilft, die Marktstruktur einzuordnen.

---

**Projektstart:** 2025-07-09  
**Autor:** minik28
