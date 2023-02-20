<!-- inspired by https://github.com/ryanzhumich/Contrastive-Learning-NLP-Papers -->
<!-- make read.me prettier:  -->
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
    A(<b>NLP</b>) -->|for| F{<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#1-market-forecasting'>Market Forecasting</a>} 
    
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
    A -->|to identify| M((<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#2-market-movers-identification'>Market Movers</a>))
    A -->|to estimate| E[<a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#3-experts-competence-estimation'>Expert's Competence</a>]
    F -->|"  "| MF{{?}}
    style Se stroke:#f66,stroke-width:2px,stroke-dasharray: 5 5,text-decoration: none
   
    
    %%I><a href='https://github.com/completelyboofyblitzed/NLP-in-STOCK-MARKET/blob/main/README.md#interpretability'>Interpretability?</a>]
    %%V<-.-I
    %%Q<-.-I
    %%Di<-.-I
    %%MF<-.-I
    %% class A,B,F,E,E,M,F,Q containers;
```

# Models
- __FinancialBERT - A Pretrained Language Model for Financial Text Mining__ `2022` <i>Ahmed Rachid Hazourli</i> [[pdf]](https://www.researchgate.net/publication/358284785_FinancialBERT_-_A_Pretrained_Language_Model_for_Financial_Text_Mining) [[demo]](https://huggingface.co/ahmedrachid/FinancialBERT)
- __FinBert - A Large Language Model for Extracting Information from Financial Text__ `2019-2022` <i> Allen H. Huanga, Hui Wang, Yi Yang</i> [[pdf]](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3910214) [[repo]](https://github.com/yya518/FinBERT) [[website]](https://finbert.ai/) [[demo]](https://huggingface.co/ProsusAI/finbert)
- __NFinBERT: A Number-Aware Language Model for Financial Disclosures__ `2021` <i>Hao-Lun Lin and Jr-Shian Wu, Yu-Shiang Huang, Ming-Feng Tsai, Chuan-Ju Wang</i> [[pdf]](https://ceur-ws.org/Vol-2957/paper5.pdf)
# 1. Market Forecasting
Projection of the market states (high/low volatility, up/down index movements).
<!-- Survey https://www.mdpi.com/2078-2489/13/10/466 -->
## Sentiment Based
- __Predicting the Stock Market with Sentiment Analysis of Newspaper Text__ <i>Juan Luis Ruiz-Tagle</i> `2020` [[master thesis (draft)]](https://github.com/juanluisrto/stock-prediction-nlp/blob/master/memoria/Juan%20Luis%20Ruiz-Tagle%2018-Mayo_memoria_2/Master_Thesis_memoria_v2.pdf) [[repo]](https://github.com/juanluisrto/stock-prediction-nlp)

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
`To be added`

## Interpretability
Essentially we want an answer to a question "what..", but can we as well know "why"?<br>
Is this problem related to long-form question-answering (LFQA)? I don't know. If so, here's something to read:<br>
- __WebGPT: Browser-assisted question-answering with human feedback__ `2021` <i>OpenAI</i> [[blog]](https://openai.com/blog/webgpt) [[pdf]](https://arxiv.org/abs/2112.09332) [[demo]](https://openaipublic.blob.core.windows.net/webgpt-answer-viewer/index.html) + the [explanation](https://habr.com/ru/company/ods/blog/709222/) on habr (by [@stalkermustang](https://github.com/stalkermustang) I presume) <br>
- __GopherCite: Teaching language models to support answers with verified quotes__ `2022` <i>DeepMind</i> [[blog]](https://www.deepmind.com/blog/gophercite-teaching-language-models-to-support-answers-with-verified-quotes) [[pdf]](https://storage.googleapis.com/deepmind-media/Teaching%20language%20models%20to%20support%20answers%20with%20verified%20quotes/Teaching%20language%20models%20to%20support%20answers%20with%20verified%20quotes.pdf)<br>
- (And obviously) __Toolformer: Language Models Can Teach Themselves to Use Tools__ `2023` <i>Meta</i> [[pdf]](https://arxiv.org/pdf/2302.04761.pdf)<br>

Can the task of prediction can be solved as collateral to the Market Movers identification?
# 2. Market Movers Identification
Market moving information is a term used in stock market investing, defined as __information that would cause any reasonable investor to make a buy or sell decision__. ([Wikipedia](https://en.wikipedia.org/wiki/Market_moving_information))<br> 

Example of a stock mover identification taken from [Benzinga](https://www.benzinga.com/apis/cloud-product/bz-why-is-it-moving/): <br>
<img src="https://www.benzinga.com/apis/wp-content/uploads/2019/10/2-1.jpg" width="600"> <br>

__How can such pipeline look:__
```mermaid
%%{init: {"theme": "default","fontFamily": "cursive", "sequence": { "securityLevel":"loose" }}}%%
stateDiagram

    classDef Important stroke:#f66,stroke-width:2px,stroke-dasharray: 5 5,text-decoration: none
    direction LR
    A: Get top N gainers/losers
    b: Get latest tweets/news
    c: Summarize as an explanation
    B: ~
    C: Show
    [*] --> A
    A --> B
    B --> C
    state B {
      direction LR
      b --> c
    }
    C --> [*]
    class c Important
```

# 3. Expert's Competence Estimation
Ranking experts, qualification of experts, based on their past predictions/performance.<br>

# Tools
__Pythonic ways to download market data from__ [Yahoo!Ⓡ finance](https://finance.yahoo.com/):<br>
[yfinance](https://pypi.org/project/yfinance/)<br>
[yahooquery](https://pypi.org/project/yahooquery/2.2.5/)<br>

# Text Sources
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

# Scrapping
`To be added`
## Websites
`To be added`
## Twitter
`To be added`
## Facebook
`To be added`
## Telegram
`To be added`

## 🤝 Contributing

Contributions, issues and feature requests are welcome.



