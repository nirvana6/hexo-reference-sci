# hexo-reference-sci

## 01. Introduction 

`hexo-reference-sci` is based on [hexo-reference-new](https://github.com/kchen0x/hexo-reference) and PR named [modified render logics to support non-number footnote marks](https://github.com/kchen0x/hexo-reference/pull/12). Thanks the original contribution from these two authors. However, when I generate the cross-reference with pached [hexo-reference-new](https://github.com/kchen0x/hexo-reference), some strange behavior appears. This is the first reason I decided to improve the original `hexo-reference-new`.

Furthermore, given that scientific writing has specific requirements regarding citation formatting and other aspects compared to general writing, this plugin will undergo significant modifications based on the existing one.

## 02. Objective

This hexo plugin will generate cross-reference when wring scitific paper or blog. On base of [AMA STYLE GUIDE](https://guides.lib.uw.edu/hsl/ama/intext), several adjustments is necessary in the context of webpage. The following is a sample:  

## 03. Text Sample

**In-text Citations Basics:**

Use superscript arabic numerals to cite material, e.g., <sup>[1]</sup>. The first reference used in a written document is listed as 1 in the reference list. If there are server citations, each number should be displayed. For example, here are several citations<sup>[2][3]</sup>.

**References**

1\. [Cancer Research Funding](http://www.cancer.gov.offcampus.lib.washington.edu/cancertopics/factsheet/NCI/research-funding). National Cancer Institute. Publication date unavailable. Updated June 6, 2011. Accessed November 3, 2012.

2\. Andre F, Zielinski CC. Optimal strategies for the treatment of metastatic triple-negative breast cancer with currently approved agents. _Ann Oncol._ 2012;23(Suppl 2):vi46-vi51.

3\. Gradishar WJ. Taxanes for the treatment of metastatic breast cancer. _Breast Cancer (Auckl.)_. 2012;6:159-171.
   
## 04. Usage

### 4.1 Markdow Syntax

```markdown

Here is the first reference[^first].

The expected style of cross-reference[^anyStringIsOk].

Here is the third reference[^another].

[^first]: basic footnote content.

[^anyStringIsOk]: [AMA STYLE GUIDE](https://guides.lib.uw.edu/hsl/ama/intext).

[^another]: [Wiki](https://www.wikiwand.com/en/Wiki).

```

### 4.2 Rendered Webpage

**Content**: 

<img width="302" alt="image" src="https://github.com/nirvana6/hexo-reference-sci/assets/2957421/8433df93-77d6-462d-ad21-88d6e52f6399">


**Reference**: 

<img width="280" alt="image" src="https://github.com/nirvana6/hexo-reference-sci/assets/2957421/1280a24b-c26c-4443-907f-5d13670653d1">
