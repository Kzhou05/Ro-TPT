# Enhancing Vision-Language Model Calibration via Rotation-Enhanced Orthogonality-Constrained Prompt Tuning

Our contributions are summarized as follows:
  - We introduce a Ro-TPT method, which can mitigate overfitting to single alignment directions by integrating random orthogonal rotations into the O-TPT framework.
- We present a new feedback reward to search for the optimal rotation space, further enhancing the directional alignment of the feature space.
- Evaluation on multiple benchmark datasets show that Ro-TPT reduces expected calibration error while maintaining accuracy, demonstrating superior performance.

## Installation
```bash
#Steps to set up the environment
 1. git clone https://github.com/ashshaksharifdeen/O-TPT.git
 2. cd O-TPT
 3. conda env create -f environment.yml
 4. conda activate otpt
```

## Datasets
We have conducted main experiments on fine-grained and natural distribution shift datasets:

- **Fine-grained datasets**:  
  1. ImageNet  
  2. Flower102  
  3. OxfordPets  
  4. SUN397  
  5. DTD  
  6. Food101  
  7. StanfordCars  
  8. Aircraft  
  9. UCF101  
  10. EuroSAT  
  11. Caltech101  

Follow this repository for datasets preparation: [TPT](https://github.com/azshue/TPT) 

## Run Experiments
In each .sh file, you can edit the root dataset directory location as well as configure the baseline, whether it's ‘RN50’ or ‘ViT-B/16’. Also, you can switch between different experiment modes by changing run_type, whether it is opt, tpt baselines, or calibration with temperature scaling.  

```bash
bash scripts/test_tpt_rotpt_fg.sh {dataset}
```

##  Citation
If you find our work useful for your research, please consider citing it:

