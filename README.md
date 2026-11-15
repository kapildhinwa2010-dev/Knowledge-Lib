# Knowledge-Lib

[![CI](https://github.com/kapildhinwa2010-dev/Knowledge-Lib/actions/workflows/ci.yml/badge.svg)](https://github.com/kapildhinwa2010-dev/Knowledge-Lib/actions/workflows/ci.yml)
[![CodeQL](https://github.com/kapildhinwa2010-dev/Knowledge-Lib/actions/workflows/codeql.yml/badge.svg)](https://github.com/kapildhinwa2010-dev/Knowledge-Lib/actions/workflows/codeql.yml)

Facts, alias derivation and chain reasoning.

**Part of the [Kapildhinwa2010-dev Toolkit](https://github.com/kapildhinwa2010-dev/Kapildhinwa2010-dev).**

![Python](https://img.shields.io/badge/python-3.9%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## ✨ Features

- (subject, predicate, object) fact triples with dedup
- Transitive `same_as` alias closure
- Multi-hop chain walks and interference ranking

## 📦 Install

```bash
pip install -r requirements.txt
```

## 🚀 Quick start

```python
from knowledge_lib import KnowledgeNet

net = KnowledgeNet()
net.add('a', 'next', 'b')
net.add('b', 'next', 'c')
print(net.chain('a', 'next'))  # ['b', 'c']
```

## 🧪 Tests

```bash
pytest tests/ -v
```

## 📄 License

MIT — see [LICENSE](LICENSE).
