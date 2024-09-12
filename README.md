Wilhelm Vocabulary
==================

![GitHub last commit badge][GitHub last commit]
![GitHub workflow status badge][GitHub workflow status]
[![Apache License Badge]](https://www.apache.org/licenses/LICENSE-2.0)

The data that serves [wilhelmlang.com](https://wilhelmlang.com/). They are written in YAML format, because

1. it is machine-readable so that it can be consumed quickly in data pipelines
2. it is human-readable and, thus, easy to modify
3. it supports multi-lines value which is very handy for data of natural languages

YAML Schema
-----------

### Geraman

```yaml
vocabulary:
  - term: string
    definition: list
    plural: string
    declension/conjugation: string
```

where the `conjugation` is the inflection paradigm for a German verb and `declension` the inflection for nouns and
adjectives. Only one of the two is present for a term.

### Korean

```yaml
vocabulary:
  - term: string
    definition: list
```

### Ancient Greek

```yaml
vocabulary:
  - term: string
    definition: list
```

### Latin

```yaml
vocabulary:
  - term: string
    definition: list
```

License
-------

The use and distribution terms for [wilhelm-vocabulary]() are covered by the [Apache License, Version 2.0].

[Apache License Badge]: https://img.shields.io/badge/Apache%202.0-F25910.svg?style=for-the-badge&logo=Apache&logoColor=white
[Apache License, Version 2.0]: http://www.apache.org/licenses/LICENSE-2.0.html

[GitHub last commit]: https://img.shields.io/github/last-commit/QubitPi/wilhelm-vocabulary/master?logo=github&style=for-the-badge
[GitHub workflow status]: https://img.shields.io/github/actions/workflow/status/QubitPi/wilhelm-vocabulary/ci-cd.yaml?branch=master&logo=github&style=for-the-badge
