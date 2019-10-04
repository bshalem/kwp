# What is KWP?
A machine-generated dataset of Kinematic word problems to train and evaluate neural models for the task of physical language understanding.

The dataset is formatted as a collection of json objects, each defines a word problem as shown in the following sample:

```json
{
    "problem_id": [3],
    "missing": ["v"],
    "equation": ["x=x0+v0*t+0.5*a*t^2"],
    "asked": ["t"],
    "known": ["x,x0,v0,a"],
    "values": ["9348 m,2122 m,6516 m/s,1256 m/s/s"],
    "derivation": ["t=sqrt(6516^2+2*1256*(9348-2122))"],
    "solution": ["7785.24 s"],
    "question": ["a train  has  an initial displacement of 2122 m, acceleration of 1256 m/s/s, final displacement of 9348 m, initial velocity of 6516 m/s . what is the time elapsed ?"]
  },
```
The initial version of the dataset contains 50,000 word problems as the split to train/dev/test is a user choice.

# Download KWP
The single file to download the entire data is [kwp.json](kwp.json).

# Paper
Motivation for simple interpreted queries, data construction and analyses are available in our companion paper:

- Avi Bleiweiss. *Neural Sequence Modeling in Physical Language Understanding*. In NCTA, 2019. (oral)

### Citation
If you use the KWP dataset as part of your work, please cite:

    @inproceedings{bleiweiss-ncta19,
        author = {Bleiweiss, Avi},
        title = {Neural Sequence Modeling in Physical Language Understanding},
        booktitle = {NCTA},
        year = {2019},
    }
