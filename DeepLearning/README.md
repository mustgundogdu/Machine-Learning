
## Create Neural Network with Python

![](https://github.com/mustgundogdu/Machine-Learning/blob/main/DeepLearning/media/nn%20.jpg)

### ----> Feed Forward
  - First of All calculate to Hidden Neurons with input values like below; (Using Activation Func.) [Φ -> Activation Func]
  
    - [x] Φ(X1.W1 + X2.W3) = H1  
                           
    - [x] Φ(X1.W2 + X2.W4) = H2  
    
    - [x] Φ(H1.W5 + H2.W6) = Output(Prediction)
    

### <--- Backward Propagation 
   - After calculating Error Value (Delta) with the formula;
     Delta = 1/2(Prediction - Actual)^2 | ---> Delta = (Prediction - Actual)
     
   - Output weights Update step with the formula (New Weight = Old Weight - αλ(Hn))[λ -> Delta][*W -> New Weight]
   
      - [x] *W5 = W5 - αλ(H1)
   
      - [x] *W6 = W6 - αλ(H2)
      
   - Input Weights Update Step with the formula like below;
   
   [W1 W3] - αλ[H1*W5 H1*W6] = [(W1-αλ[H1*W5]) (W3 - H1*W6)]
               
   [W2 W4] - αλ[H2*W5 H2*W6] = [(W2-αλ[H2*W5]) (W4-αλ[H2*W6])]
             
  
  
