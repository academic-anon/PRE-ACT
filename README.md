# PRE-ACT: Progressive Risk Estimation for Accident Anticipation


## Verification of Results

We believe that independent verification of reported results is essential. To support this, we provide our model predictions on the CAP, DADA, and Nexar datasets, together with the evaluation code used to compute the metrics, enabling direct verification of the results reported in the state-of-the-art comparison tables.

We share the compact annotation files derived from original MM-AU and Nexar datasets in the `annotations` folder. 
Predictions of our model for all three datasets are shared in the `predictions` folder.
We also share the scripts used to calculate the metrics on MM-AU and Nexar datasets in `src` folder.

After installing the required packages (check `src/requirements.txt`), and `cd src`:

**CAP** dataset evaluation run; 

```
python mmau_eval.py --subset cap
```

**DADA** dataset evaluation run;

```
python mmau_eval.py --subset dada
```

Finally, for **Nexar** dataset, run;

```
python nexar_eval.py
```

**After acceptance, we will publicly release the full codebase and pretrained models to support open and reproducible research.**

## Visual Comparison with Baseline and Failure Cases

We created a project page in this [LINK](https://academic-anon.github.io/pre-act/).
In this page, we present visual comparisons of PRE-ACT and a baseline method on randomly selected videos of CAP and DADA datasets.

Furthermore, we show representative failure cases of our model on both datasets.