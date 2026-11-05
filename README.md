# UCBShift-X models for the browser port

Random-forest models of **UCBShift-X** (the machine-learning module of UCBShift 2.0), converted losslessly from the
published scikit-learn models for use by the fully client-side web app (UCBShift-X Web).

* `manifest.json`: list of models (one R0 ExtraTrees and one R1 RandomForest model per atom type, 47 atom types)
  and their chunks.
* `*.bin.gz`: 100-tree chunks in a compact binary format (u16 feature index, float32 threshold, float32 leaf value;
  byte-shuffled and gzip-compressed). Predictions are identical to scikit-learn's (max. difference 1.2·10⁻⁷ ppm).

Source models: Zenodo record 15375968 (https://doi.org/10.5281/zenodo.15375968), from
https://github.com/THGLab/CSpred. Please check the licence of the original record before reusing these files.

If you use them, please cite:
* Li, Bennett, Liu, Martin & Head-Gordon, *Chem. Sci.* 2020, 11, 3180.
* Ptaszek, Li, Konrat, Platzer & Head-Gordon, *J. Am. Chem. Soc.* 2024, 146, 31733.