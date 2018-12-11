# dialog-data
This repository contains a few Dialog Datasets that I retrieved from various sources.
Please cite/acknowledge the original authors or creators:

## Friends 
FRIENDS TV show dataset cleaned and partitioned. 
I obtained this data from https://github.com/fangj/friends/ and cleaned it to a nicer TSV format. No information on whom to cite (guessing this is in public domain now!)

## Cornell movie dialog corpus
I obtained this from [this link](https://www.cs.cornell.edu/~cristian/Cornell_Movie-Dialogs_Corpus.html) and formatted to nicer TSV format
```
@InProceedings{Danescu-Niculescu-Mizil+Lee:11a,
  author={Cristian Danescu-Niculescu-Mizil and Lillian Lee},
  title={Chameleons in imagined conversations: 
  A new approach to understanding coordination of linguistic style in dialogs.},
  booktitle={Proceedings of the Workshop on Cognitive Modeling and Computational Linguistics, ACL 2011},
  year={2011}
}
```


# Format of the data

TSVs are nicer to work with, so lets make this as a standard :)

## Data format
- A corpus file can have many dialogs
- An empty line (new line `\n`) separates dialogs.
- Each dialog can have many utterances ( an utterance is a turn)
- Each turn can have three fields, separated by tab character `\t`
  - first column is unique identifier for turn.
  - second column is character or agent name.
  - third column is a text utterance (a sequence of words).

Here is an example of two dialogs:
```tsv
0101_002	monica	there 's nothing to tell he 's just some guy i work with
0101_003	joey	c 'mon , you 're going out with the guy there 's gotta be something wrong with him
0101_004	chandler	all right joey , be nice . so does he have a hump ? a hump and a hairpiece ?
0101_005	phoebe	wait , does he eat chalk ?

0101_007	phoebe	just , cause , i don 't want her to go through what i went through with carl- oh
0101_008	monica	okay , everybody relax . this is not even a date . it 's just two people going out to dinner and- not having sex .
0101_009	chandler	sounds like a date to me .

```



P.S.
If you have a new dataset, please send me a link by creating an issue or send it via pull request. Goal is to collect lots of data, so we can train interesting neural models 
