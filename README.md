# FEGTOR
3D Facial expression generator with Transformer-based conditional VAE.

## 1. Dataset
Our dataset is generated from the  [**BU face data**](http://www.cs.binghamton.edu/~lijun/Research/3DFE/3DFE_Analysis.html) .<br>. It consists of a total of 606 sequences of 83 manually labeled landmarks extracted from 3D facial scans. 6 basic expressions (anger, disgust, fear, happy, sad, and surprise) have been recorded for each of 101 subjects.

## 2. Model
<img  src="Results/Face 3D.png"  />

                                       
## 3. Evaluation
1. FID score


| Model type  | FID |
| ------------- | -------------  |
| CondGRU| 101.5 |
| Action2motion| 33.3 |
| GRU VAE | 28.7 |
| Ours | 13.7 |
## 4. Results
Our results are based on 83 landmarks which should be reconstructed to deform 3D mesh
### Example           
| Happy  | Surprise |  Angry | 
| ------------- | ------------- | ------------- | 
| <img  src="Results/happy.gif"  /> | <img src="Results/surprise.gif"  /> |  <img src="Results/angry.gif"  /> |   
### Rendered Example           
| Model|Happy  | Surprise |  Angry | 
| ------------- | ------------- | ------------- | -------------------|
| Ours |<img  src="Results/gif/trans/trans_Happy15.gif"  /> | <img src="Results/gif/trans/transSurprise_15.gif"  /> |  <img src="Results/gif/trans/trans_angry15.gif"  /> | 
       
