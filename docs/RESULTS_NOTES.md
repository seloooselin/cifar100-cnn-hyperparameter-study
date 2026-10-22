# Results and interpretation notes

## Evidence boundaries

The final submitted report is authoritative for what the author reports having conducted and concluded. The author confirms that computational limitations required experiments across multiple computers and Colab accounts. The included notebooks are a deliberately small accessible subset; archive gaps are not evidence that a reported experiment did not occur.

`reported_results.csv` transcribes the final report's nine rows verbatim in numeric content and uncertainty, retaining its original train/test labels. No values, uncertainties or averages were recalculated. `preserved_runs.csv` separately transcribes the selected notebooks' explicit `Test accuracy` and `Test loss` output lines and reads their settings from code. Neither table replaces the other. The ± entries retain the report's notation; this package does not independently establish their calculation convention.

The unmodified original workbook is additional historical evidence. It is not silently preferred over the final report. In particular, the workbook's low-dropout average test accuracy is 0.6098, while the final report states 0.6055 ± 0.0065. Both sources are retained.

## Original reported conclusions

- Learning rate 0.0005 performs best in the report's learning-rate comparison; 0.0001 learns more slowly and 0.001 plateaus earlier.
- The report favours batch size 128 as a balance between performance and stability. Its table nevertheless lists higher mean test accuracy for 256 (0.6038 versus 0.6017). The narrative's description of 128 as having the highest accuracy, and its claim that 256 has higher training accuracy, do not match the table. No narrative or numeric source was rewritten.
- The report favours baseline dropout, interpreting high dropout as underfitting and low dropout as more prone to overfitting despite slightly higher reported accuracy. The confidence/calibration interpretation is the author's reported interpretation; no calibration experiment is claimed.
- Longer training, CutMix, label smoothing, learning-rate schedules and other datasets are future directions only.

## Preserved implementation details

Every selected notebook retains a complete 100-epoch log, final printed evaluation and two embedded plots. The baseline contains the entire pipeline in one code cell. Two learning-rate notebooks have null execution counts despite retained outputs; their saved outputs are preserved evidence, not a fresh execution performed for this package.

The selected dropout notebooks use batch size 125; the report describes 128. This means the preserved dropout comparison is not strictly a one-parameter change relative to the included baseline. Code is unchanged and the difference is explicit in `preserved_runs.csv`.

In the broader accessible archive, three 0.0001 notebooks labelled runs 2, 4 and 5 have identical saved outputs. They were excluded from this concise selection in favour of run 1. The accessible batch-size and dropout folders contain three runs per setting, while the report describes five. These observations limit reconstruction from the accessible archive; they do not establish what was or was not run on other systems.

Some report training entries match values shown in Keras evaluation progress displays, which differ from final printed evaluations and from the training-history series. Therefore original labels are retained as reported, without certifying that every historical entry measures the quantity its heading suggests.

## Histories and figures

- `history_run1.json`: 100 epochs of accuracy, loss, validation accuracy and validation loss; final validation accuracy 0.6090999841690063. It corresponds to a separate historical baseline run, not the selected representative run 4.
- `history_run2_2_2.json`: same four series for 100 epochs; final validation accuracy 0.5246000289916992, matching the selected learning-rate 0.001 run's evaluation accuracy. The filename is preserved; association is based on matching recorded values, not a global run-ID system.
- `baseline_accuracy.png` and `baseline_loss.png`: decoded directly from the representative notebook's existing PNG outputs, without regenerating curves.
- `original_learning_rate_comparison.png`: byte-for-byte copy of the original local figure. Its title identifies validation accuracy; the report's Figure X caption describes training accuracy. No relabelling was performed, and all series are not reconstructed from the two bundled histories.

The report PDF and its Drive reference text are preserved independently. The Drive text snapshot omits image rendering; consult the PDF for the submitted layout and figures.
