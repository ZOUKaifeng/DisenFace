# 3D Facial Expression Generator Based on Transformer VAE.

## 1. Dataset

We test our method on [**CoMA dataset**](https://coma.is.tue.mpg.de/) and [**BU-4DFE data**](http://www.cs.binghamton.edu/~lijun/Research/3DFE/3DFE_Analysis.html).
## 2. Model
Our approach is divided into two steps. Firstly, a Transformer VAE is trained to perform the conditional generation of landmarks sequences. Then a landmark-guided mesh deformation (LGMD) model estimates vertex-wise displacements, which is used to deform a neutral face to the expected expression frame by frame.

<img  src="Results/model1.png"  />
                                       


## 3. Results

#### Diversity of mouth open
 <img  src="Results/diversity_mouth_open.jpg"  />  
 
#### Diversity of baretheeth
 <img  src="Results/diversity_bareteeth.jpg"  />  



#### Exaggeration
Since we add the displacements to the neutral face to deform it, an exaggerated expression can easily be obtained by multiplying the displacement with a constant value.
 <img  src="Results/exaggeration.jpg"  />

### Landmark videos for the visual comparison
The outputs of transformer VAE, a set of landmark sequences conditioned by the expression label, have been compared to those from other models for the qualitative jugements. <br> 


#### "Happy expression"

 <img  src="Results/gif/happy.gif"  />  
 
 
 #### "Surprise expression"

 <img  src="Results/gif/surprise.gif"  />  
 
### Videos of meshes 
The full mesh animation can be obtained by our landmark-driven 3D mesh deformation, based on a Radial Basis Function. Some of the results thus obtained are shown below: <br>
 
#### Diversity 
 <img  src="Results/gif/div_bareteeth.gif"  /> 
 
 
  
#### Random sampling from Gaussian distribution

 <img  src="Results/gif/random_generation.gif"  /> 
 
 
 #### Exaggeration
  <img  src="Results/gif/exaggeration.gif"  /> 
  
  
    
  #### Mesh comparison
  
  #### Noise removal
