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
    title[<u>Table of Contents:</u>]
    title---F
    style title fill:#FFF,stroke:#FFF
    linkStyle 0 stroke:#FFF,stroke-width:0;

    %%FirstStep-->...
    %%classDef containers fill:#E6E1F7
    
    %% styling the nodes and arrors https://dompl.medium.com/produce-great-looking-flowcharts-in-seconds-7f3bea64f2e2
    %% mermaid editor https://mermaid.live
    Mo[[<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#models'>Models</a>]]
    A(<b>NLP</b>) -->|for| F{<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#market-forecasting'>Market Forecasting</a>} 
    
    style A stroke:#333,stroke-width:4px
    subgraph MF [<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#sentiment-based' >Sentiment based</a>]
    Se{{<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#sentiment-analysis'>Sentiment<br>Analysis</a>}}
    Fc{{<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#forecasting'>Forecasting</a>}}
    %% Al{{?}}
    end

    
    Ts[(<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#text-sources'>Text Sources</a>)]
    
    %% Se<-.-Mo
    %% Fc<-.-Al[[<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#algorithms'>Algorithms</a>]]
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
    Sc(((<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#scrapping'>Scrapping</a>)))
    Ts[(<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#text-sources'>Text Sources</a>)]
    subgraph Ws [<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#websites'>Websites</a>]
        subgraph Tw [<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#websites'>Twitter</a>]
            subgraph Fb [<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#websites'>Facebook</a>]
                subgraph Tg [<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#websites'>Telegram</a>]
                Cm[(Plain mentions/tags)]
                Ex[("''Experts''")]
                In[(Highly influential<br> individuals)]
                Of[(Official Media)]
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
# Models
- __FinBert: A Large Language Model for Extracting Information from Financial Text__ `2019-2022` <i> Allen H. Huanga, Hui Wang, Yi Yang</i> [[pdf]](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3910214) [[repo]](https://github.com/yya518/FinBERT) [[website]](https://finbert.ai/)
# 1. Market Forecasting
Projection of the market states (high/low volatility, up/down index movements).
## Sentiment Based
- __Predicting the Stock Market with Sentiment Analysis of Newspaper Text__ <i>Juan Luis Ruiz-Tagle</i> `2020` [[thesis draft]](https://github.com/juanluisrto/stock-prediction-nlp/blob/master/memoria/Juan%20Luis%20Ruiz-Tagle%2018-Mayo_memoria_2/Master_Thesis_memoria_v2.pdf) [[repo]](https://github.com/juanluisrto/stock-prediction-nlp)

> __Text source:__ newspapers <br />
> __Sentiment model:__ BERT <br />
> __Predictions model:__ LSTM? <br />
<img src="https://github.com/juanluisrto/stock-prediction-nlp/blob/master/stock-prediction/etsfactory_article/pngs/predictions_tesla.png" width="460" title="Claimed predictions Tesla based solely on newspaper text"> <br />
_Claimed predictions for Tesla based solely on newspaper text_

<!-- https://youtu.be/G5ycs1hFSKk -->
<!-- https://github.com/pvanand07/NIFTY50-Daily-Trend-Prediction-Using-NLP-Python -->
<!-- finbert https://github.com/juanluisrto/stock-prediction-nlp/blob/master/memoria/papers/FinBERT.pdf -->
<!-- https://github.com/search?o=desc&q=nlp+for+stock&s=updated&type=Repositories -->
<!-- https://github.com/yiaktan/NLP-Stock-Prediction -->
### Sentiment Analysis
__Models__ <br>
[__Hugging Face Hub #financial-sentiment-analysis__](https://huggingface.co/models?other=financial-sentiment-analysis)


<!-- - __Fine-tuned LM__ -->
### Forecasting

#### Algorithms
# 2. Expert's Competence Estimation
Ranking experts, qualification of experts, based on their past predictions/performance.<br>

# 3. Market Movers Identification
Market moving information is a term used in stock market investing, defined as __information that would cause any reasonable investor to make a buy or sell decision__. ([Wikipedia](https://en.wikipedia.org/wiki/Market_moving_information))<br> 

# Text Sources
`To be added`

# Scrapping

## Websites
`To be added`
## Twitter
`To be added`
## Facebook
`To be added`
## Telegram
`To be added`



