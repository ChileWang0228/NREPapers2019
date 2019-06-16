# Relation Extraction in 2019

This repo covers almost all the papers (35) related to **Neural Relation Extraction** in ACL, EMNLP, COLING, NAACL, AAAI, IJCAI in 2019.

Use tags to search papers you like.

**tags: | DSRE | PGM | Combining Direct Supervision | GNN | new perspective | new dataset | joint extraction of relations and entities | few shot | BERT |... |**

## NAACL 2019

1. **Structured Minimally Supervised Learning for Neural Relation Extraction**
   _Fan Bai and Alan Ritter_
   NAACL 2019
   [paper](https://arxiv.org/pdf/1904.00118.pdf)
   [code](https://github.com/bflashcp3f/PCNN-NMAR)

   PGM | DSRE

   > This paper adds a PGM inference into training stage.

2. **Combining Distant and Direct Supervision for Neural Relation Extraction**
   _Iz Beltagy, Kyle Lo and Waleed Ammar_
   NAACL 2019
   [paper](https://arxiv.org/pdf/1810.12956.pdf)
   [code](https://github.com/allenai/comb_dist_direct_relex)

   Combining Direct Supervision | DSRE

   > This paper combines direct supervision and distant supervision. It innovatively uses direct supervision for training sigmoid attention in a multi-task way. Further, when applying to the CNN backbone with different filter sizes, adding entity embedding as additional inputs is a useful trick, which performs comparable to RESIDE and better than PCNN-ATT. After combining the supervised sigmoid attention, this paper become a new sota.   

## ACL 2019

1. **Graph Neural Networks with Generated Parameters for Relation**
    _Hao Zhu and Yankai Lin and Zhiyuan Liu, Jie Fu, Tat-seng Chua, Maosong Sun_
    ACL 2019
    [paper](https://arxiv.org/pdf/1902.00756.pdf)

    GNN | new task | new perspective 

    > This paper considers multi-hop relation extraction, which constructs a fully-connected graph for all entities in a sentence. Experiments show that modeling entity-relation as a graph signifcantly improves the performance. 
2. **Entity-Relation Extraction as Multi-turn Question Answering**
   _Xiaoya Li, Fan Yin, Zijun Sun, Xiayu Li
    Arianna Yuan, Duo Chai, Mingxin Zhou and Jiwei Li_
    ACL2019
    [paper](https://arxiv.org/abs/1905.05529)

    | new dataset | new perspective| joint extraction of relations and entities

    > In this paper, we propose a new paradigm for
the task of entity-relation extraction. We cast
the task as a multi-turn question answering
problem, i.e., the extraction of entities and relations
is transformed to the task of identifying
answer spans fromthe context. Thismulti-turn
QA formalization comes with several key advantages:
firstly, the question query encodes
important information for the entity/relation
class we want to identify; secondly, QA provides
a natural way of jointly modeling entity
and relation; and thirdly, it allows us to exploit
the well developed machine reading comprehension
(MRC) models.
    > Additionally, we construct a newly developed
    dataset RESUME in Chinese, which requires
    multi-step reasoning to construct entity dependencies,
    as opposed to the single-step dependency
    extraction in the triplet exaction in previous
    datasets.

3. **Matching the Blanks: Distributional Similarity for Relation Learning**
   _Livio Baldini Soares, Nicholas FitzGerald, Jeffrey Ling, Tom Kwiatkowski_
   ACL2019
   [paper](https://arxiv.org/pdf/1906.03158.pdf)

   | few shot | sota | BERT |

   > In this paper we study the problem of producing
useful relation representations directly from text.
We describe a novel training setup, which we call
matching the blanks, which relies solely on entity
resolution annotations. When coupled with
a new architecture for fine-tuning relation representations
in BERT, our models achieves state-ofthe-
art results on three relation extraction tasks,
and outperforms human accuracy on few-shot relation
matching. In addition, we show how the
new model is particularly effective in low-resource
regimes, and we argue that it could significantly
reduce the amount of human effort required to create
relation extractors.