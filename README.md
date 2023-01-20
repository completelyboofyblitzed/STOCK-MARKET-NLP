<!-- make read me prettier: todo list https://docs.github.com/ru/get-started/writing-on-github/working-with-advanced-formatting/about-task-lists#about-task-lists -->
## Paper List on all kinds of NLP for market forecasting, experts estimation, etc.

```mermaid
%%{init: { "sequence": { "securityLevel":"loose" }}}%%
graph TD
    %% styling the nodes and arrors https://dompl.medium.com/produce-great-looking-flowcharts-in-seconds-7f3bea64f2e2
    %% mermaid editor https://mermaid.live
    A(<b>NLP</b>) -->|for| C{<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#market-forecasting'>Market Forecasting</a>} 
    style A stroke:#333,stroke-width:4px
    J[(<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#text-sources'>Text Sources</a>)]
    H(((<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#scrapping'>Scrapping</a>)))
    A -->|to| E[<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#experts-competence-estimation'>Estimate Expert's Competence</a>]
    A -->|in| M((<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#market-movers-identification'>Market Movers Identification</a>))
    C -->|based on| D{{<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#sentiment-based'>Sentiment</a>}}
    C -->|?| B{{?}}
    style D fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
    click B href "https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#sentiment-based" "This is a tooltip for a link"
    E -->|?| F[/?\]
    M -->|?| Q([?])
```

# Market Forecasting
## Sentiment Based
- __Predicting the Stock Market with Sentiment Analysis of Newspaper Text__ <i>Juan Luis Ruiz-Tagle</i> `2020` [[thesis draft]](https://github.com/juanluisrto/stock-prediction-nlp/blob/master/memoria/Juan%20Luis%20Ruiz-Tagle%2018-Mayo_memoria_2/Master_Thesis_memoria_v2.pdf) [[repo]](https://github.com/juanluisrto/stock-prediction-nlp)

> _Text source: newspapers_ <br />
> _Sentiment model: BERT_ <br />
> _Predictions model: LSTM?_ <br />
<img src="https://github.com/juanluisrto/stock-prediction-nlp/blob/master/stock-prediction/etsfactory_article/pngs/predictions_tesla.png" width="460" title="Claimed predictions Tesla based solely on newspaper text"> <br />
_Claimed predictions for Tesla based solely on newspaper text_

# Expert's Competence Estimation
`To be added`

# Market Movers Identification
`To be added`

# Text Sources
`To be added`

# Scrapping
`To be added`



