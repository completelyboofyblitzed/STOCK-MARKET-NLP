<!-- inspired by https://github.com/ryanzhumich/Contrastive-Learning-NLP-Papers -->
<!-- make read me prettier:  -->
<!-- todo list https://docs.github.com/ru/get-started/writing-on-github/working-with-advanced-formatting/about-task-lists#about-task-lists -->
<!-- emojies https://github.com/chroline/well_app/blob/main/README.md -->
<!-- tables https://github.com/ArmynC/ArminC-AutoExec/#readme -->
<!-- pic https://github.com/karan/joe#readme -->
## Research on all kinds of NLP for market forecasting, experts estimation, etc.

```mermaid
%%{init: {"theme": "default","fontFamily": "cursive", "sequence": { "securityLevel":"loose" }}}%%
graph TD
    classDef containers fill:#E6E1F7
    
    %% styling the nodes and arrors https://dompl.medium.com/produce-great-looking-flowcharts-in-seconds-7f3bea64f2e2
    %% mermaid editor https://mermaid.live
    
    A(<b>NLP</b>) -->|for| F{<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#market-forecasting'>Market Forecasting</a>} 
    
    style A stroke:#333,stroke-width:4px
    subgraph MF [<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#sentiment-based' >Sentiment based</a>]
    Se{{<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#sentiment-analysis'>Sentiment<br>Analysis</a>}}
    Fc{{<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#forecasting'>Forecasting</a>}}
    %% Al{{?}}
    end

    
    Ts[(<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#text-sources'>Text Sources</a>)]
    Mo[[<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#models'>Models</a>]]
    Se<-.-Mo
    Fc<-.-Al[[<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#algorithms'>Algorithms</a>]]
    F--> Di{{Direct}}

    Sc(((<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#scrapping'>Scrapping</a>)))
    A -->|to estimate| E[<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#experts-competence-estimation'>Expert's Competence</a>]
    A -->|to identify| M((<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#market-movers-identification'>Market Movers</a>))
    F -->|"  "| MF{{?}}
    style Se stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5,text-decoration: none
    E -->|?| V[/?\]
    M -->|?| Q([?])
    %% class A,B,F,E,E,M,F,Q containers;
```

```mermaid
%%{init: {"theme": "default","fontFamily": "cursive", "sequence": { "securityLevel":"loose" }}}%%
graph TD
    classDef containers fill:#E6E1F7
    %% Nw(((Websites)))
    %% Tw(((Tweets)))
    Sc(((<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#scrapping'>Scrapping</a>)))
    Ts[(<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#text-sources'>Text Sources</a>)]
    subgraph Ws [Websites]
        subgraph Tw [Twitter]
            subgraph Fb [Facebook]
                subgraph Tg [Telegram]
                Of[(Official Media)]
                Cm[(Plain mentions/tags)]
                Ex[("''Experts'''")]
                In[(Highly influential<br> individuals)]

                end
            end
        end
    end
    Ts-->Cm
    Ts-->Ex
    Ts-->In
    Ts-->Of
    Sc-.-Fb
    Sc-.-Tw
    Sc-.-Ws
    Sc-.-Tg
```

# Market Forecasting
## Sentiment Based
- __Predicting the Stock Market with Sentiment Analysis of Newspaper Text__ <i>Juan Luis Ruiz-Tagle</i> `2020` [[thesis draft]](https://github.com/juanluisrto/stock-prediction-nlp/blob/master/memoria/Juan%20Luis%20Ruiz-Tagle%2018-Mayo_memoria_2/Master_Thesis_memoria_v2.pdf) [[repo]](https://github.com/juanluisrto/stock-prediction-nlp)

> _Text source: newspapers_ <br />
> _Sentiment model: BERT_ <br />
> _Predictions model: LSTM?_ <br />
<img src="https://github.com/juanluisrto/stock-prediction-nlp/blob/master/stock-prediction/etsfactory_article/pngs/predictions_tesla.png" width="460" title="Claimed predictions Tesla based solely on newspaper text"> <br />
_Claimed predictions for Tesla based solely on newspaper text_

<!-- https://youtu.be/G5ycs1hFSKk -->
<!-- https://github.com/pvanand07/NIFTY50-Daily-Trend-Prediction-Using-NLP-Python -->
<!-- finbert https://github.com/juanluisrto/stock-prediction-nlp/blob/master/memoria/papers/FinBERT.pdf -->
<!-- https://github.com/search?o=desc&q=nlp+for+stock&s=updated&type=Repositories -->
<!-- https://github.com/yiaktan/NLP-Stock-Prediction -->
### Sentiment Analysis
### Forecasting

# Expert's Competence Estimation
`To be added`

# Market Movers Identification
`To be added`

# Text Sources
`To be added`

# Scrapping
`To be added`



