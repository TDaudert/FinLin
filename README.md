# A Multi-Source Entity-Level Sentiment Corpus for the Financial Domain: The FinLin Corpus

FinLin is multi-source multi-entity corpus for fine-grained financial sentiment analysis. It covers a period of 3 months and a set of automobile companies as sentiment targets. In addition to  fine-grained sentiment, it comes with a relevance measure aimed at supporting the capture of a market sentiment by giving each item an individual weight. FinLin covers microblogs from StockTwit, news articles, company reports, and analyst reports.
If you want, then you can add figure 4 from the paper here but I dont think its needed. 

A full description of the corpus can be found in the [original paper](https://doi.org/10.1007/s10579-021-09555-3). 

The data distribution is as follows:

<img src="https://github.com/TDaudert/FinLin/blob/main/FinLin_observations.png"  width="450">

## FinLin Structure

The FinLin files come in the following structure: 

<img src="https://github.com/TDaudert/FinLin/blob/main/FinLin_structure.png"  width="450">

- "type" : The data type [SW,NA,AR,CR].
- "text" : The body of text.
- "title" : The title/headline.
- "created_at" : The timestamp.
- "entity" : The sentiment target (abbreviations are defined in the original paper).
- "id" : The unique identifier. 
- "sentiment" : The fine-grained sentiment score in the range [-1,1].
- "relevance" : The fine-grained relevance score in the range [0,1].
- "annotations" : The list of each individual annotation per annotator. 
- "spans" : The list of "text_spans" and "title_spans".
- "text_spans" : The substring of "text" as highlighted by the corresponding annotator. 
- "title_spans" : The substring of "title" as highlighted by the corresponding annotator. 

## Reference 
If you use FinLin in your research, please cite [this paper](https://doi.org/10.1007/s10579-021-09555-3):

~~~
@article{daudert2021multi,
  title={A multi-source entity-level sentiment corpus for the financial domain: the FinLin corpus},
  author={Daudert, Tobias},
  journal={Language Resources and Evaluation},
  pages={1--24},
  year={2021},
  publisher={Springer},
  doi = {10.1007/s10579-021-09555-3},
  url = {https://doi.org/10.1007/s10579-021-09555-3}
}
~~~
## License 
This corpus is openly available for non-commercial use under the [Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/).

## Contact & Obtaining this Corpus
If you have any questions, suggestions, or want to obtain a copy of this corpus, you can contact Tobias Daudert (finlin.corpus@gmail.com).

## Disclaimer 
FinLin is created for research purposes only. The author is not responsible for any damages related to or inflicted by its use.
