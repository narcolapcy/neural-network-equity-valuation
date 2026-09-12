# Evidence and limitations

## Source mapping

Primary source: the author's April 2025 undergraduate thesis, *Evaluation and Application of Digital Enterprise Value based on Feedforward Neural Network — Software Development Industry*.

| Public claim | Original location |
| --- | --- |
| 388 companies, 2011–2023, CSMAR, ST exclusion, 1% winsorization and Z-score scaling | Chapter 3, data sources and preprocessing |
| 14 inputs, four hidden neurons, tanh, one output | Chapter 3, detailed model design |
| Four factors and 71.854% cumulative variance | Chapter 3, factor-analysis table and discussion |
| Test R² 0.9800 and MSE 0.0099 | Table 3-6 |
| RMB 26.84bn versus RMB 25.52bn, 5.17% | Chapter 4, company valuation results table |

Values in the public report are reported historical results, not newly recomputed estimates. The case difference is independently arithmetically consistent with `(26.84 - 25.52) / 25.52 ≈ 5.17%`.

## Boundaries

- The original narrative has inconsistent descriptions of network depth. The public summary follows the detailed 14-input, four-hidden-neuron, one-output specification, without asserting that original fitted weights are available.
- The archive does not establish the train/test allocation, random seed, training-only preprocessing, information-availability dates or a complete fitted-model artifact. Exact replication is unavailable.
- Table 3-6 is transcribed unchanged; small MSE/RMSE rounding or transcription discrepancies remain. The transformed target scale cannot be treated as a currency error scale.
- A high reported R² does not establish protection against leakage, future predictive accuracy or investable mispricing.
- Licensed input rows are excluded; anonymization would not by itself establish redistribution permission.

## Replication requirements

Recover the original training implementation and fitted model, document the final sample, and acquire appropriately licensed point-in-time inputs. Then test chronological and company-disjoint splits, train-only preprocessing, baseline models and robustness to alternative architectures.
