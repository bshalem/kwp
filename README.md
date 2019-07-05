# kwp_dataset
A machine-generated dataset of Kinematic word problems to train and evaluate neural models for the task of physical language understanding.

The dataset is a collection of word problem objects, each formatted with the following set of fields:

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
