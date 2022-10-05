# Convolutional-Neural-Network
Coded Convolutional Neural Network using Keras as part of the ITCS-6156-001-Machine Learning

In this program I have creatyed CNN 

![image](https://user-images.githubusercontent.com/13596624/193973175-ff526c29-64f6-4200-818e-5021274459d1.png)

<br/>

Tested the code with different Optimizers


Available Optimizers<br/>
&nbsp;&nbsp;&nbsp;&nbsp; **- SGD:** In stochastic gradient descent, instead of taking the whole dataset for each iteration, it randomly selects the batches of data.<br/><br/>
&nbsp;&nbsp;&nbsp;&nbsp;**- RMSprop:** RMS prop can also be considered an advancement in AdaGrad optimizer as it reduces the monotonically decreasing learning rate<br/><br/>
&nbsp;&nbsp;&nbsp;&nbsp;**- Adam:**   Adaptive moment estimation which is extension of stochastic gradient descent to update network weights during training<br/><br/>
&nbsp;&nbsp;&nbsp;&nbsp;**- Adadelta:** It is more robust version of AdaGrad optimizer. AdaDelta uses two state variables to store the leaky average of the second moment gradient and a leaky average of the second moment of change of parameters in the model. <br/><br/>
&nbsp;&nbsp;&nbsp;&nbsp;**- Adagrad:** The adaptive gradient descent algorithm is different from other gradient descent algorithms as it uses different learning rates for each iteration. The change in learning rate depends upon the difference in the parameters during training.<br/><br/>
&nbsp;&nbsp;&nbsp;&nbsp;**- Adamax:** AdaMax is an extension to the Adam version of gradient descent that generalizes the approach to the infinite norm (max) and may result in a more effective optimization on some problems.<br/><br/>
&nbsp;&nbsp;&nbsp;&nbsp;**- Nadam**<br/><br/>
&nbsp;&nbsp;&nbsp;&nbsp;**- Ftrl**<br/><br/>
 Except from SGD, others are Adaptive optimizers<br/><br/>

On testing the code with the following optimizers for 100 epochs, below are the observation after 50 Epochs and the Final IOU

**ADAM**<br/>
Epoch 50, Loss: 3.52e+03, IOU - Train: 0.978 Valid: 0.762 Test: 0.793<br/>
IOU: 0.793213448518527<br/><br/>

**SGD: Updates the weights after seeing each data points**<br/>
Epoch 50, Loss: 5.56e+04, IOU - Train: 0.66 Valid: 0.583 Test: 0.675<br/>
IOU: 0.7186441827007882<br/><br/>

**Adagrad: Adaptive Leap**<br/>
Epoch 50, Loss: 4.46e+04, IOU - Train: 0.704 Valid: 0.63 Test: 0.687<br/>
IOU: 0.7200430199134298<br/><br/>

**Adadelta**<br/>
Epoch 50, Loss: 1.14e+05, IOU - Train: 0.502 Valid: 0.459 Test: 0.506<br/>
IOU: 0.5237069707087039<br/><br/>

**Adamax**<br/>
Epoch 50, Loss: 1.06e+04, IOU - Train: 0.933 Valid: 0.733 Test: 0.773<br/>
IOU: 0.7728205776406226<br/><br/>

**RMSprop**<br/>
Epoch 50, Loss: 7.09e+03, IOU - Train: 0.928 Valid: 0.751 Test: 0.814<br/>
IOU: 0.8139378503341943 <br/><br/>

Adam, RMSprop and Adamax converged quicker than other optimizer
