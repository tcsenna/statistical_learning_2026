# Chapter 1 — Introduction to Machine Learning


## What is Machine Learning?

Machine Learning (ML) enables computers to learn patterns from data without being explicitly programmed.

Instead of writing rules manually, we provide data and let the system infer patterns and relationships.

## Basic Concepts


* **Training Set**: The dataset used to train the model.
* **Instance (Sample)**: Each individual example in the training set.
* **Accuracy**: The proportion of correctly classified instances.

Machine Learning is especially useful for:

* Problems too complex for rule-based solutions
* Problems with no known algorithm

  * Example: speech recognition

---

##  Why Machine Learning Matters (Beyond Automation)

ML is not only a tool for automation — it can also help **humans understand problems better**.

By analyzing what a model learns, we can:

* Discover unexpected correlations
* Identify hidden patterns
* Gain deeper insights into the data

This process is often referred to as **data mining**.

---

## Types of Machine Learning

### 1. Supervised Learning

The training data includes **input features and target labels**.

#### Main Tasks:

* **Classification**: Predict discrete labels
* **Regression**: Predict continuous numeric values

#### Common Algorithms:

* Linear Regression
* Logistic Regression
* Support Vector Machines (SVM)
* Decision Trees & Random Forests
* Neural Networks

> Note: Some algorithms can be used for both classification and regression.

---

### 2. Unsupervised Learning

The training data is **unlabeled**.
The system tries to find structure without guidance.

#### 🔹 Clustering

Groups similar instances together.

Example:

* Segmenting website visitors into groups with similar behavior
* Hierarchical clustering builds nested clusters step by step

#### 🔹 Visualization

Reduces high-dimensional data into 2D/3D representations to:

* Understand structure
* Identify unexpected patterns

These methods try to preserve as much of the original data structure as possible.

#### 🔹 Dimensionality Reduction

Reduces the number of features while preserving information.

Example:

* Mileage and age of a car → combined into a single “wear” feature

This is called **feature extraction**.

💡 Common workflow:

* Apply dimensionality reduction
* Feed the output into a supervised model

Benefits:

* Faster training
* Less storage
* Sometimes better performance

---

#### 🔹 Anomaly Detection

Identifies unusual or rare instances.

Examples:

* Fraud detection in credit card transactions
* Detecting manufacturing defects
* Removing outliers before training another model

---

#### 🔹 Novelty Detection

Detects **new, previously unseen patterns**.

⚠️ Requires a **clean training dataset** (no noise or anomalies).

Example:

* If only 1% of images are a rare dog breed:

  * Anomaly detection → flags them as unusual
  * Novelty detection → does NOT flag them (they are already part of training distribution)

---

#### 🔹 Association Rule Learning

Finds relationships between variables.

Example:

* Customers who buy meat also buy toothpaste
  → Useful for product placement in retail

---

### 3. Semi-Supervised Learning

Uses a **small amount of labeled data** and a large amount of unlabeled data.

Example:

* Google Photos:

  * You label a person once
  * The system learns to identify them across all photos

Many semi-supervised models combine supervised and unsupervised techniques.

Example:

* Deep Belief Networks (DBNs):

  * Built from stacked **Restricted Boltzmann Machines (RBMs)**
  * Pretrained in an unsupervised way
  * Fine-tuned with supervised learning

---

### 4. Reinforcement Learning

A completely different paradigm.

* The system is called an **agent**
* It interacts with an **environment**
* It takes actions and receives:

  * Rewards (positive)
  * Penalties (negative)

The goal is to learn a **policy**:

* A strategy that defines the best action in each situation
* Maximizes cumulative reward over time

---

## Some Thoughts

Machine Learning is not just about prediction — it's about:

* Discovering structure
* Learning from data
* Improving decision-making

As datasets grow in size and complexity, ML becomes an essential tool for extracting meaningful insights.

---



## Typographic replacements

Enable typographer option to see result.

(c) (C) (r) (R) (tm) (TM) (p) (P) +-

test.. test... test..... test?..... test!....

!!!!!! ???? ,,  -- ---

"Smartypants, double quotes" and 'single quotes'


## Emphasis

**This is bold text**

__This is bold text__

*This is italic text*

_This is italic text_

~~Strikethrough~~


## Blockquotes


> Blockquotes can also be nested...
>> ...by using additional greater-than signs right next to each other...
> > > ...or with spaces between arrows.


## Lists

Unordered

+ Create a list by starting a line with `+`, `-`, or `*`
+ Sub-lists are made by indenting 2 spaces:
  - Marker character change forces new list start:
    * Ac tristique libero volutpat at
    + Facilisis in pretium nisl aliquet
    - Nulla volutpat aliquam velit
+ Very easy!

Ordered

1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa


1. You can use sequential numbers...
1. ...or keep all the numbers as `1.`

Start numbering with offset:

57. foo
1. bar


## Code

Inline `code`

Indented code

    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code


Block code "fences"

```
Sample text here...
```

Syntax highlighting

``` js
var foo = function (bar) {
  return bar++;
};

console.log(foo(5));
```

## Tables

| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

Right aligned columns

| Option | Description |
| ------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |


## Links

[link text](http://dev.nodeca.com)

[link with title](http://nodeca.github.io/pica/demo/ "title text!")

Autoconverted link https://github.com/nodeca/pica (enable linkify to see)


## Images

![Minion](https://octodex.github.com/images/minion.png)
![Stormtroopocat](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")

Like links, Images also have a footnote style syntax

![Alt text][id]

With a reference later in the document defining the URL location:

[id]: https://octodex.github.com/images/dojocat.jpg  "The Dojocat"


## Plugins

The killer feature of `markdown-it` is very effective support of
[syntax plugins](https://www.npmjs.org/browse/keyword/markdown-it-plugin).


### [Emojies](https://github.com/markdown-it/markdown-it-emoji)

> Classic markup: :wink: :cry: :laughing: :yum:
>
> Shortcuts (emoticons): :-) :-( 8-) ;)

see [how to change output](https://github.com/markdown-it/markdown-it-emoji#change-output) with twemoji.


### [Subscript](https://github.com/markdown-it/markdown-it-sub) / [Superscript](https://github.com/markdown-it/markdown-it-sup)

- 19^th^
- H~2~O


### [\<ins>](https://github.com/markdown-it/markdown-it-ins)

++Inserted text++


### [\<mark>](https://github.com/markdown-it/markdown-it-mark)

==Marked text==


### [Footnotes](https://github.com/markdown-it/markdown-it-footnote)

Footnote 1 link[^first].

Footnote 2 link[^second].

Inline footnote^[Text of inline footnote] definition.

Duplicated footnote reference[^second].

[^first]: Footnote **can have markup**

    and multiple paragraphs.

[^second]: Footnote text.


### [Definition lists](https://github.com/markdown-it/markdown-it-deflist)

Term 1

:   Definition 1
with lazy continuation.

Term 2 with *inline markup*

:   Definition 2

        { some code, part of Definition 2 }

    Third paragraph of definition 2.

_Compact style:_

Term 1
  ~ Definition 1

Term 2
  ~ Definition 2a
  ~ Definition 2b


### [Abbreviations](https://github.com/markdown-it/markdown-it-abbr)

This is HTML abbreviation example.

It converts "HTML", but keep intact partial entries like "xxxHTMLyyy" and so on.

*[HTML]: Hyper Text Markup Language

### [Custom containers](https://github.com/markdown-it/markdown-it-container)

::: warning
*here be dragons*
:::
