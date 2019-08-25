---
title: Li-Li - teresa alias
category: CLI
layout: 2017/sheet
ads: false
updated: 2019-08-25
keywords:
  - Luilza Labs
  - Heroku
  - Teresa
  - Shell
  - Alias
intro: |
  [Teresa](https://github.com/luizalabs/teresa) is a Open source tool to deploy apps to Kubernetes clusters.

  [Li-Li](https://github.com/TiagoTi/LiLi) is my personal support in oh my zsh plugin
---
---

## Alias

### App
{: .-prime}

```bash
#teresa app logs -f <app-name>
trsl <app-name>
```

```bash
#teresa app info <app-info>
trsli <app-name>
```

### Cluster

```bash
#teresa config use cluster
trscuc <cluster-name>
```

```bash
#teresa config use cluster transaction production
trscuctp <cluster-name>

#teresa config use cluster transaction stage
trscucts <cluster-name>
```
