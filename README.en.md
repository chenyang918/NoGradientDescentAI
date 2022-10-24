# Super solution method

#### Introduction
From the above method, it can be further deduced that any vector @ a unit vector = [1] can be used to solve the solution of any vector multiplication.

Any vector @unit vector = [1] can be used to solve for any vector multiplication, as long as it has its own sum.

Therefore, there are data constraints to determine which vectors are used to solve

    # Suppose this vector is B = [b1,b2,b3,b4,..... .bn] sum(B)=[1]
    # k*B = k*[b1,b2,b3,b4,..... .bn] k*B@I(T)=k*[1]
    # A@x(T)=[k]=k*[1]=k*B@I(T) =[b1,b2,b3,b4,..... .bn] * k
    # [1*x1,2*x2,3*x3,.... .n*xn] = [b1,b2,b3,b4,..... .bn] * k  
    # [1*x1=b1*k,2*x2=b2*k,... .n*xn=bn*k] 
    # Multiple inputs and outputs produce multiple solutions Finally, choose a common solution for the dataset in order to generalize the model
    # Directly use no input and output weight rows to solve the equation through column vectors See code yan_zheng.py
    # The equiproportional method can only solve for one input and one output, so it is not a generic solution.
    # The number of rows of a weight determines the complexity of the data that the weight can express
This generic solution method only requires partitioning the data in series to achieve a generative network

The focus is on how to select the data for the solution
The general method is to calculate the distance of all the data relative to the zero point and then select the data equally.
To do so

By dividing the data in series, you can achieve multiple superposition 

How to create nonlinearity (using activation function) You can directly perform activation function on the output data and then input to another layer The output is still the output

This allows for nonlinearity. The data fit itself is for the uninvolved data, so the output data is equivalent to the input data.

Since the dimensionality of the input data determines the number of rows of weights, which determines the amount of reference data needed, sometimes more data is needed for the simulation.

Therefore, an equivalence matrix is used to expand the dimensionality of the input data. This means expanding the number of rows of weights and the amount of data used.

The amount of posterior data used should be consistent with the dimensionality used 
*** Translated with www.DeepL.com/Translator (free version) ***

