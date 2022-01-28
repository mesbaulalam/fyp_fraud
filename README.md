![Python](https://img.shields.io/badge/Python-3.7.4-fcba03)
![SEC-API](https://img.shields.io/badge/SECAPI-1.0.8-green)
![NLTK](https://img.shields.io/badge/NLTK-3.6.7-blueviolet)


# Financial Fraud Detection using Text Mining

## Abstract

Financial statements are a representation of the economic status of a company. Besides being a
significant source of loss for potential stakeholders, fraudulent financial statements also erode
confidence in the capital market. Current auditing practices rely heavily on quantitative measures
such as financial ratios to detect possible fraud. However, there is a lack of research or analysis
of detecting financial fraud through textual analysis. Furthermore, quantitative analysis of
financial statements heavily ignores underlying information such as auditor’s comments or notes.
Hence, several text mining approaches are proposed in this project, which process the textual
information present in financial statements in the hopes of detecting fraud. The research will
leverage various text transformation techniques such as Bag of Words and Term
Frequency–Inverse Document Frequency (TF-IDF) to extract meaning out of the textual content.
The use of data mining techniques will result in a more thorough examination of financial
statements, examining qualitative variables to determine the degree of fraud. Currently, the
project is in its interim stage, where MD&A sections of financial statements are collected
successfully and data cleaning is performed for text transformation purposes. The transformed
text is tested against various machine learning algorithms. The machine learning models are
further optimized through GridSearchCV. A considerable amount of work needs to be
accomplished in the next stage such as determining advanced text transformation techniques
such as vector embeddings and generating further relevant features from the current text corpus.
These transformation techniques are vital for extracting more meaningful information regarding
the fraudulent nature of documents. Upon feedback from relevant supervisors, the model will be
optimized accordingly. Although the team faced some setbacks, such as selecting appropriate
datasets and generating features from the text corpus, the project is expected to be implemented
on schedule through an extensive literature review of external research papers.

```
Dataset Creation - Outlines the methods and the API used to extract MD&A section from financial statements using SEC-API

Predictor - Outlines the EDA and the text transformation techniques used to predict fraud through SVM, Naive Bayes and Logistic Regression

```

## Accuracy Scores

  <table>
    <thead>
      <tr>
        <th></th>
        <th>BoW</th>
        <th>TF-IDF</th>
      </tr>
    </thead>
    <tbody>
        <tr>
            <td>NB Classifier</td>
            <td><code>80.31%</code></td>
            <td><code>78.52%</code></td>
        </tr>
       <tr>
            <td>SVM</td>
            <td><code>79.32%</code></td>
            <td><code>87.07%</code></td>
        </tr>
         <tr>
            <td>LR</td>
            <td><code>86.2%</code></td>
            <td><code>89.66%</code></td>
        </tr>
    </tbody>
  </table>
