# hexo-reference-sci

## Introduction 

`hexo-reference-sci` is based on [hexo-reference-new](https://github.com/kchen0x/hexo-reference) and PR named [modified render logics to support non-number footnote marks](https://github.com/kchen0x/hexo-reference/pull/12). Thanks the original contribution from these two authors. However, when I generate the cross-reference with pached [hexo-reference-new](https://github.com/kchen0x/hexo-reference), some strange behavior appears. This is the first reason I decided to improve the original `hexo-reference-new`.

Furthermore, given that scientific writing has specific requirements regarding citation formatting and other aspects compared to general writing, this plugin will undergo significant modifications based on the existing one.

**Aims**: Generate cross-reference when wring scitific paper or blog.

## Features


## Usage

### Markdow Syntax

```markdown

Here is the first reference[^first].

The expected style of cross-reference[^anyStringIsOk].

Here is the third reference[^another].

[^first]: basic footnote content.

[^anyStringIsOk]: [AMA STYLE GUIDE](https://guides.lib.uw.edu/hsl/ama/intext).

[^another]: [Wiki](https://www.wikiwand.com/en/Wiki).

```

### Rendered Webpage

**Content**: 

<img width="302" alt="image" src="https://github.com/nirvana6/hexo-reference-sci/assets/2957421/8433df93-77d6-462d-ad21-88d6e52f6399">


**Reference**: 

<img width="280" alt="image" src="https://github.com/nirvana6/hexo-reference-sci/assets/2957421/1280a24b-c26c-4443-907f-5d13670653d1">



