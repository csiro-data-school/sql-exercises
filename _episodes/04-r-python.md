---
title: "Exercise 3 - R or Python interaction"
teaching: 0
exercises: 120
objectives:
- "Write an R or Python function, interacting with database"
---

Write an R or Python function that queries your database.  
The function should:

#### 1. Accept a search term as an input argument.
#### 2. Search the 'annotation' column of the AlignAnnot table for any records that include the search term.
#### 3. For each match, print:
####    - The corresponding sequence's name
####    - The corresponding sequence's sample name
####    - The corresponding sequence's group name
####    - The corresponding sequence's type name
####    - The matched annotation's name
####    - The matched annotation
  
Test out your function. For example, you might call it with “hypothetical” as the search
term, as per question 12 of the previous exercise.
  
E.g.:

~~~
result <- searchAnnotations('hypothetical')
head(result, n=10)
~~~
{: .language-r}

~~~
            SeqName   Sample      SeqGroup SeqType  MatchName                               Annotation
1   D18-gDNA-s8.g11 D18-gDNA augustus-D18g protein KZN00833.1         hypothetical protein DCAR_009587
2   D18-gDNA-s9.g12 D18-gDNA augustus-D18g protein CAN66637.1       hypothetical protein VITISV_011340
3   D18-gDNA-s9.g12 D18-gDNA augustus-D18g protein CAN73567.1       hypothetical protein VITISV_003451
4   D18-gDNA-s9.g12 D18-gDNA augustus-D18g protein KZV51625.1          hypothetical protein F511_24998
5   D18-gDNA-s9.g12 D18-gDNA augustus-D18g protein KZV39555.1 hypothetical protein F511_13790, partial
6   D18-gDNA-s9.g12 D18-gDNA augustus-D18g protein PHT39301.1         hypothetical protein CQW23_22874
7  D18-gDNA-s20.g35 D18-gDNA augustus-D18g protein AGM34082.1                     hypothetical protein
8  D18-gDNA-s38.g65 D18-gDNA augustus-D18g protein CAN75041.1       hypothetical protein VITISV_027174
9  D18-gDNA-s42.g73 D18-gDNA augustus-D18g protein KZN00833.1         hypothetical protein DCAR_009587
10 D18-gDNA-s42.g73 D18-gDNA augustus-D18g protein KZV46985.1          hypothetical protein F511_15782
~~~
{: .output}
  
{% include links.md %}

