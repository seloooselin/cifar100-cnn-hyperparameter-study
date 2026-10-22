# Provenance, selection and publication review

Prepared on 22 October 2026 as a local portfolio package for Selin Deniz İşken. No training, repository creation or publication was performed. Original Mac and Google Drive files were read only.

## Primary sources

- [Experiment collection](https://drive.google.com/drive/folders/1CL_dEEAy3wxXM8SWNWYlbQ65sBgPC9K9)
- [Final report reference](https://docs.google.com/document/d/1iQrgMYbj6doJDgOfrefy5Y4fYpFcr1OAYJLvwrvqZ58/edit)
- [Earlier Colab development notebook](https://colab.research.google.com/drive/1y2zaSX0emBdGOWj1xwBkVcKPUpqy99E-), retained as a source link only. It mixes experimental code with teaching material and is not the primary portfolio implementation.

The final report text was retrieved in the preceding audit in this conversation. `submitted_report_text.txt` preserves that retrieved reference. Local report, workbook, figure and history files are unmodified copies; neutral source filenames and SHA-256 hashes appear in `source_manifest.json`. Personal filesystem paths have been omitted from this public package.

## Notebook selection

- `notebooks/01_cifar100_cnn_baseline.ipynb` — [learningrate0005-4.ipynb](https://colab.research.google.com/drive/1Is_xA5TMM5_bwUbziQGBW27-ceOJPAa4)
- `notebooks/experiments/learning_rate_0001.ipynb` — [learningrate0001-1.ipynb](https://drive.google.com/file/d/1Xop85JRgqnAtOWjrqOiCxC8JmqWgOOUB/view?usp=drivesdk)
- `notebooks/experiments/learning_rate_001.ipynb` — [learningrate001-1.ipynb](https://colab.research.google.com/drive/1w_spQwAqJBqLSZfAVBY8suhCOJ0oO9u5)
- `notebooks/experiments/batch_size_64.ipynb` — [batchsize64-1.ipynb](https://colab.research.google.com/drive/15COORnwat7rKUqe5aLGYIzx4YpOvHaAQ)
- `notebooks/experiments/batch_size_256.ipynb` — [batchsize256-2.ipynb](https://colab.research.google.com/drive/1S_qqSMPkzAlLLqMMYBOWQTZd_mWkesIL)
- `notebooks/experiments/dropout_low.ipynb` — [dropoutlow-1.ipynb](https://colab.research.google.com/drive/1sfi-_mkiCg9EqmpPLhk0_rnIBy95Kv4W)
- `notebooks/experiments/dropout_high.ipynb` — [dropouthigh-1.ipynb](https://colab.research.google.com/drive/1K66N08ocehheR2EAuYv4i_BWJSaBbxgu)

The baseline was selected for completeness and representative settings, not as the highest-accuracy run. The six alternatives cover both sides of each report comparison. Source notebooks keep their code, execution counts and recorded outputs. Only package filenames, JSON formatting and transient Colab execution metadata were changed in copies. The manifest records source-byte and packaged-byte hashes.

Relevant local notebooks were compared with these Drive versions during the audit. Examples include `learningrate0005_3.ipynb` in the local notebook-export collection, `batchsize64_1.ipynb`, `batchsize256_2.ipynb`, `dropoutlow_1.ipynb`, and `dropouthigh_1.ipynb`. Drive versions were chosen consistently for the seven-notebook selection; identical or overlapping local exports are not duplicated in the package. The earlier CIFAR-10 draft and mixed exploratory notebooks are omitted for focus.

## Attribution

The University of Manchester COMP34212 CIFAR CNN teaching notebook contains this attribution:

> Copyright (c) 2022 Angelo Cangelosi, MIT License. Code and examples adapted from Gulli & Pal (2017) Deep Learning with Kera. Punkt Publishing. With support from Wenjie Huang.

The quotation retains the spelling in the original notice. Bibliographic spelling is commonly “Deep Learning with Keras.” The instructor-supplied source lab is `COMP34212_Lab2b_Keras_CNN_CIFAR_2025(1).ipynb`, inspected in the local university-coursework archive. The full teaching notebook is excluded from this package.

The portfolio describes the author's coursework extensions and experimental work, not authorship of the underlying CNN methods, dataset or teaching foundation. The report's references are preserved in the report. No claim of a novel CNN architecture or deployed robotics system is made.

## Public-publication review

Reviewed on 22 October 2026 for the proposed `seloooselin/cifar100-cnn-hyperparameter-study` repository. No GitHub repository has been created or published.

### Coursework content and permissions

The University's [published guidance on lecture/course material and assessment content](https://www.staffnet.manchester.ac.uk/adviceandresponse/resources/types-of-potential-misbehaviour/) distinguishes student-owned assessment content from university-owned questions, instructions and feedback. It permits students to use their assessment content after the examination period has concluded. Its [student copyright guidance](https://subjects.library.manchester.ac.uk/copyright/students) also confirms student ownership of original coursework, subject to any separate IP assignment.

The author has identified this as completed individual coursework after the examination period. The available 2025 COMP34212 assignment brief was inspected in full: no explicit restriction on subsequent public publication of the student's solution was found. Its prohibition on AI-generated reports concerns assessment preparation, not post-assessment publication. No additional COMP34212-specific publication ban was found in the available documentation or the targeted public search. This is a finding about the sources inspected, not a claim that an individual course approval letter exists.

The university assignment brief, questions, marking criteria, lecture slides, assessment feedback and complete teaching notebooks are excluded. The included report and reference text contain the author's review and experimental analysis, not a reproduced assignment brief. No source papers or book pages are redistributed. Existing plots, report, workbook, metric histories, notebook code and recorded results are preserved unchanged.

### Upstream code rights

The supplied instructor notebook explicitly marks the teaching code MIT-licensed. [Third-party notices](../THIRD_PARTY_NOTICES.md) preserve its Cangelosi copyright, Gulli/Pal and Huang credits, and complete MIT terms. The official Packt repository was checked directly, including its corresponding CIFAR CNN example and complete [publisher MIT licence](https://github.com/PacktPublishing/Deep-Learning-with-Keras/blob/master/LICENSE). The publisher notice is retained verbatim in [licenses/Packt-MIT.txt](../licenses/Packt-MIT.txt). No separate lab-specific full licence document was available; the lab's explicit MIT identification is the source for its declared licence, with standard MIT terms reproduced transparently.

No material unresolved rights issue was identified for this selected package on the inspected evidence. No new repository-wide licence is assigned to the author's original work or report. Upstream code retains its MIT terms.

### Privacy and integrity

Personal local paths have been replaced by source filenames and neutral archive descriptions. The package retains author attribution and source Drive/Colab URLs, which do not contain access credentials. Those historical source links may require permission to open; all essential review material is included locally, so public repository readers do not depend on Drive access.

The source manifest continues to record original and packaged hashes. Notebooks, report, CSV results, workbook, histories and figures were not altered during publication cleanup. Missing preserved runs reflect distributed execution and incomplete accessible archives; this package makes no allegation about experiments outside the retained files.
