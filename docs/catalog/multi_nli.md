<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>
  <meta itemprop="name" content="multi_nli" />
  <meta itemprop="description" content="The Multi-Genre Natural Language Inference (MultiNLI) corpus is a&#10;crowd-sourced collection of 433k sentence pairs annotated with textual&#10;entailment information. The corpus is modeled on the SNLI corpus, but differs in&#10;that covers a range of genres of spoken and written text, and supports a&#10;distinctive cross-genre generalization evaluation. The corpus served as the&#10;basis for the shared task of the RepEval 2017 Workshop at EMNLP in Copenhagen.&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/multi_nli" />
  <meta itemprop="sameAs" content="https://www.nyu.edu/projects/bowman/multinli/" />
</div>

# `multi_nli`

The Multi-Genre Natural Language Inference (MultiNLI) corpus is a crowd-sourced
collection of 433k sentence pairs annotated with textual entailment information.
The corpus is modeled on the SNLI corpus, but differs in that covers a range of
genres of spoken and written text, and supports a distinctive cross-genre
generalization evaluation. The corpus served as the basis for the shared task of
the RepEval 2017 Workshop at EMNLP in Copenhagen.

*   URL:
    [https://www.nyu.edu/projects/bowman/multinli/](https://www.nyu.edu/projects/bowman/multinli/)
*   `DatasetBuilder`:
    [`tfds.text.multi_nli.MultiNLI`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/text/multi_nli.py)

`multi_nli` is configured with `tfds.text.multi_nli.MultiNLIConfig` and has the
following configurations predefined (defaults to the first one):

*   `plain_text` (`v0.0.2`) (`Size: 216.34 MiB`): Plain text

## `multi_nli/plain_text`

Plain text

Versions:

*   **`0.0.2`** (default):
*   `1.0.0`: New split API (https://tensorflow.org/datasets/splits)

### Statistics

Split                 | Examples
:-------------------- | -------:
ALL                   | 412,349
TRAIN                 | 392,702
VALIDATION_MISMATCHED | 9,832
VALIDATION_MATCHED    | 9,815

### Features

```python
FeaturesDict({
    'hypothesis': Text(shape=(), dtype=tf.string),
    'label': ClassLabel(shape=(), dtype=tf.int64, num_classes=3),
    'premise': Text(shape=(), dtype=tf.string),
})
```

### Urls

*   [https://www.nyu.edu/projects/bowman/multinli/](https://www.nyu.edu/projects/bowman/multinli/)

## Citation
```
@InProceedings{N18-1101,
  author = "Williams, Adina
            and Nangia, Nikita
            and Bowman, Samuel",
  title = "A Broad-Coverage Challenge Corpus for
           Sentence Understanding through Inference",
  booktitle = "Proceedings of the 2018 Conference of
               the North American Chapter of the
               Association for Computational Linguistics:
               Human Language Technologies, Volume 1 (Long
               Papers)",
  year = "2018",
  publisher = "Association for Computational Linguistics",
  pages = "1112--1122",
  location = "New Orleans, Louisiana",
  url = "http://aclweb.org/anthology/N18-1101"
}
```

--------------------------------------------------------------------------------
