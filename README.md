# ResNet20v1-On-CIFAR-10
In this repository I have applied ResNet20v1 On CIFAR-10 dataset and received accuracy of 88.4 % at 30th epoch.
My Model Structure is 

Layer (type)                    Output Shape         Param #     Connected to                     
==================================================================================================
input_2 (InputLayer)            (None, 32, 32, 3)    0                                            
__________________________________________________________________________________________________
conv2d_22 (Conv2D)              (None, 32, 32, 16)   448         input_2[0][0]                    
__________________________________________________________________________________________________
batch_normalization_20 (BatchNo (None, 32, 32, 16)   64          conv2d_22[0][0]                  
__________________________________________________________________________________________________
activation_20 (Activation)      (None, 32, 32, 16)   0           batch_normalization_20[0][0]     
__________________________________________________________________________________________________
conv2d_23 (Conv2D)              (None, 32, 32, 16)   2320        activation_20[0][0]              
__________________________________________________________________________________________________
batch_normalization_21 (BatchNo (None, 32, 32, 16)   64          conv2d_23[0][0]                  
__________________________________________________________________________________________________
activation_21 (Activation)      (None, 32, 32, 16)   0           batch_normalization_21[0][0]     
__________________________________________________________________________________________________
conv2d_24 (Conv2D)              (None, 32, 32, 16)   2320        activation_21[0][0]              
__________________________________________________________________________________________________
batch_normalization_22 (BatchNo (None, 32, 32, 16)   64          conv2d_24[0][0]                  
__________________________________________________________________________________________________
add_10 (Add)                    (None, 32, 32, 16)   0           activation_20[0][0]              
                                                                 batch_normalization_22[0][0]     
__________________________________________________________________________________________________
activation_22 (Activation)      (None, 32, 32, 16)   0           add_10[0][0]                     
__________________________________________________________________________________________________
conv2d_25 (Conv2D)              (None, 32, 32, 16)   2320        activation_22[0][0]              
__________________________________________________________________________________________________
batch_normalization_23 (BatchNo (None, 32, 32, 16)   64          conv2d_25[0][0]                  
__________________________________________________________________________________________________
activation_23 (Activation)      (None, 32, 32, 16)   0           batch_normalization_23[0][0]     
__________________________________________________________________________________________________
conv2d_26 (Conv2D)              (None, 32, 32, 16)   2320        activation_23[0][0]              
__________________________________________________________________________________________________
batch_normalization_24 (BatchNo (None, 32, 32, 16)   64          conv2d_26[0][0]                  
__________________________________________________________________________________________________
add_11 (Add)                    (None, 32, 32, 16)   0           activation_22[0][0]              
                                                                 batch_normalization_24[0][0]     
__________________________________________________________________________________________________
activation_24 (Activation)      (None, 32, 32, 16)   0           add_11[0][0]                     
__________________________________________________________________________________________________
conv2d_27 (Conv2D)              (None, 32, 32, 16)   2320        activation_24[0][0]              
__________________________________________________________________________________________________
batch_normalization_25 (BatchNo (None, 32, 32, 16)   64          conv2d_27[0][0]                  
__________________________________________________________________________________________________
activation_25 (Activation)      (None, 32, 32, 16)   0           batch_normalization_25[0][0]     
__________________________________________________________________________________________________
conv2d_28 (Conv2D)              (None, 32, 32, 16)   2320        activation_25[0][0]              
__________________________________________________________________________________________________
batch_normalization_26 (BatchNo (None, 32, 32, 16)   64          conv2d_28[0][0]                  
__________________________________________________________________________________________________
add_12 (Add)                    (None, 32, 32, 16)   0           activation_24[0][0]              
                                                                 batch_normalization_26[0][0]     
__________________________________________________________________________________________________
activation_26 (Activation)      (None, 32, 32, 16)   0           add_12[0][0]                     
__________________________________________________________________________________________________
conv2d_29 (Conv2D)              (None, 16, 16, 32)   4640        activation_26[0][0]              
__________________________________________________________________________________________________
batch_normalization_27 (BatchNo (None, 16, 16, 32)   128         conv2d_29[0][0]                  
__________________________________________________________________________________________________
activation_27 (Activation)      (None, 16, 16, 32)   0           batch_normalization_27[0][0]     
__________________________________________________________________________________________________
conv2d_30 (Conv2D)              (None, 16, 16, 32)   9248        activation_27[0][0]              
__________________________________________________________________________________________________
conv2d_31 (Conv2D)              (None, 16, 16, 32)   544         activation_26[0][0]              
__________________________________________________________________________________________________
batch_normalization_28 (BatchNo (None, 16, 16, 32)   128         conv2d_30[0][0]                  
__________________________________________________________________________________________________
add_13 (Add)                    (None, 16, 16, 32)   0           conv2d_31[0][0]                  
                                                                 batch_normalization_28[0][0]     
__________________________________________________________________________________________________
activation_28 (Activation)      (None, 16, 16, 32)   0           add_13[0][0]                     
__________________________________________________________________________________________________
conv2d_32 (Conv2D)              (None, 16, 16, 32)   9248        activation_28[0][0]              
__________________________________________________________________________________________________
batch_normalization_29 (BatchNo (None, 16, 16, 32)   128         conv2d_32[0][0]                  
__________________________________________________________________________________________________
activation_29 (Activation)      (None, 16, 16, 32)   0           batch_normalization_29[0][0]     
__________________________________________________________________________________________________
conv2d_33 (Conv2D)              (None, 16, 16, 32)   9248        activation_29[0][0]              
__________________________________________________________________________________________________
batch_normalization_30 (BatchNo (None, 16, 16, 32)   128         conv2d_33[0][0]                  
__________________________________________________________________________________________________
add_14 (Add)                    (None, 16, 16, 32)   0           activation_28[0][0]              
                                                                 batch_normalization_30[0][0]     
__________________________________________________________________________________________________
activation_30 (Activation)      (None, 16, 16, 32)   0           add_14[0][0]                     
__________________________________________________________________________________________________
conv2d_34 (Conv2D)              (None, 16, 16, 32)   9248        activation_30[0][0]              
__________________________________________________________________________________________________
batch_normalization_31 (BatchNo (None, 16, 16, 32)   128         conv2d_34[0][0]                  
__________________________________________________________________________________________________
activation_31 (Activation)      (None, 16, 16, 32)   0           batch_normalization_31[0][0]     
__________________________________________________________________________________________________
conv2d_35 (Conv2D)              (None, 16, 16, 32)   9248        activation_31[0][0]              
__________________________________________________________________________________________________
batch_normalization_32 (BatchNo (None, 16, 16, 32)   128         conv2d_35[0][0]                  
__________________________________________________________________________________________________
add_15 (Add)                    (None, 16, 16, 32)   0           activation_30[0][0]              
                                                                 batch_normalization_32[0][0]     
__________________________________________________________________________________________________
activation_32 (Activation)      (None, 16, 16, 32)   0           add_15[0][0]                     
__________________________________________________________________________________________________
conv2d_36 (Conv2D)              (None, 8, 8, 64)     18496       activation_32[0][0]              
__________________________________________________________________________________________________
batch_normalization_33 (BatchNo (None, 8, 8, 64)     256         conv2d_36[0][0]                  
__________________________________________________________________________________________________
activation_33 (Activation)      (None, 8, 8, 64)     0           batch_normalization_33[0][0]     
__________________________________________________________________________________________________
conv2d_37 (Conv2D)              (None, 8, 8, 64)     36928       activation_33[0][0]              
__________________________________________________________________________________________________
conv2d_38 (Conv2D)              (None, 8, 8, 64)     2112        activation_32[0][0]              
__________________________________________________________________________________________________
batch_normalization_34 (BatchNo (None, 8, 8, 64)     256         conv2d_37[0][0]                  
__________________________________________________________________________________________________
add_16 (Add)                    (None, 8, 8, 64)     0           conv2d_38[0][0]                  
                                                                 batch_normalization_34[0][0]     
__________________________________________________________________________________________________
activation_34 (Activation)      (None, 8, 8, 64)     0           add_16[0][0]                     
__________________________________________________________________________________________________
conv2d_39 (Conv2D)              (None, 8, 8, 64)     36928       activation_34[0][0]              
__________________________________________________________________________________________________
batch_normalization_35 (BatchNo (None, 8, 8, 64)     256         conv2d_39[0][0]                  
__________________________________________________________________________________________________
activation_35 (Activation)      (None, 8, 8, 64)     0           batch_normalization_35[0][0]     
__________________________________________________________________________________________________
conv2d_40 (Conv2D)              (None, 8, 8, 64)     36928       activation_35[0][0]              
__________________________________________________________________________________________________
batch_normalization_36 (BatchNo (None, 8, 8, 64)     256         conv2d_40[0][0]                  
__________________________________________________________________________________________________
add_17 (Add)                    (None, 8, 8, 64)     0           activation_34[0][0]              
                                                                 batch_normalization_36[0][0]     
__________________________________________________________________________________________________
activation_36 (Activation)      (None, 8, 8, 64)     0           add_17[0][0]                     
__________________________________________________________________________________________________
conv2d_41 (Conv2D)              (None, 8, 8, 64)     36928       activation_36[0][0]              
__________________________________________________________________________________________________
batch_normalization_37 (BatchNo (None, 8, 8, 64)     256         conv2d_41[0][0]                  
__________________________________________________________________________________________________
activation_37 (Activation)      (None, 8, 8, 64)     0           batch_normalization_37[0][0]     
__________________________________________________________________________________________________
conv2d_42 (Conv2D)              (None, 8, 8, 64)     36928       activation_37[0][0]              
__________________________________________________________________________________________________
batch_normalization_38 (BatchNo (None, 8, 8, 64)     256         conv2d_42[0][0]                  
__________________________________________________________________________________________________
add_18 (Add)                    (None, 8, 8, 64)     0           activation_36[0][0]              
                                                                 batch_normalization_38[0][0]     
__________________________________________________________________________________________________
activation_38 (Activation)      (None, 8, 8, 64)     0           add_18[0][0]                     
__________________________________________________________________________________________________
average_pooling2d_2 (AveragePoo (None, 1, 1, 64)     0           activation_38[0][0]              
__________________________________________________________________________________________________
flatten_2 (Flatten)             (None, 64)           0           average_pooling2d_2[0][0]        
__________________________________________________________________________________________________
dense_2 (Dense)                 (None, 10)           650         flatten_2[0][0]                  
==================================================================================================
Total params: 274,442
Trainable params: 273,066
Non-trainable params: 1,376
__________________________________________________________________________________________________
ResNet20v1


Accuracy Logs for 50 epochs is 

Epoch 1/50
Learning rate:  0.001
1563/1563 [==============================] - 39s 25ms/step - loss: 1.6801 - acc: 0.4472 - val_loss: 1.7122 - val_acc: 0.4850

Epoch 00001: val_acc improved from -inf to 0.48500, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.001.h5
Epoch 2/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 1.3323 - acc: 0.5808 - val_loss: 1.2364 - val_acc: 0.6239

Epoch 00002: val_acc improved from 0.48500 to 0.62390, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.002.h5
Epoch 3/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 1.1610 - acc: 0.6483 - val_loss: 1.0790 - val_acc: 0.6773

Epoch 00003: val_acc improved from 0.62390 to 0.67730, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.003.h5
Epoch 4/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 1.0660 - acc: 0.6844 - val_loss: 1.1193 - val_acc: 0.6902

Epoch 00004: val_acc improved from 0.67730 to 0.69020, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.004.h5
Epoch 5/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 1.0001 - acc: 0.7076 - val_loss: 1.0037 - val_acc: 0.7184

Epoch 00005: val_acc improved from 0.69020 to 0.71840, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.005.h5
Epoch 6/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 0.9493 - acc: 0.7297 - val_loss: 1.0671 - val_acc: 0.7037

Epoch 00006: val_acc did not improve from 0.71840
Epoch 7/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 0.9108 - acc: 0.7437 - val_loss: 0.9611 - val_acc: 0.7335

Epoch 00007: val_acc improved from 0.71840 to 0.73350, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.007.h5
Epoch 8/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 0.8845 - acc: 0.7555 - val_loss: 0.8782 - val_acc: 0.7671

Epoch 00008: val_acc improved from 0.73350 to 0.76710, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.008.h5
Epoch 9/50
Learning rate:  0.001
1563/1563 [==============================] - 34s 22ms/step - loss: 0.8565 - acc: 0.7657 - val_loss: 1.1798 - val_acc: 0.6918

Epoch 00009: val_acc did not improve from 0.76710
Epoch 10/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 0.8391 - acc: 0.7717 - val_loss: 0.8151 - val_acc: 0.7864

Epoch 00010: val_acc improved from 0.76710 to 0.78640, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.010.h5
Epoch 11/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 0.8219 - acc: 0.7791 - val_loss: 0.8762 - val_acc: 0.7706

Epoch 00011: val_acc did not improve from 0.78640
Epoch 12/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 0.8054 - acc: 0.7852 - val_loss: 0.7952 - val_acc: 0.7961

Epoch 00012: val_acc improved from 0.78640 to 0.79610, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.012.h5
Epoch 13/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 0.7878 - acc: 0.7941 - val_loss: 0.9032 - val_acc: 0.7635

Epoch 00013: val_acc did not improve from 0.79610
Epoch 14/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 0.7783 - acc: 0.7968 - val_loss: 0.9768 - val_acc: 0.7376

Epoch 00014: val_acc did not improve from 0.79610
Epoch 15/50
Learning rate:  0.001
1563/1563 [==============================] - 33s 21ms/step - loss: 0.7732 - acc: 0.7995 - val_loss: 0.7909 - val_acc: 0.8001

Epoch 00015: val_acc improved from 0.79610 to 0.80010, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.015.h5
Epoch 16/50
Learning rate:  0.001
1563/1563 [==============================] - 90s 57ms/step - loss: 0.7619 - acc: 0.8042 - val_loss: 0.7666 - val_acc: 0.8023

Epoch 00016: val_acc improved from 0.80010 to 0.80230, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.016.h5
Epoch 17/50
Learning rate:  0.001
1563/1563 [==============================] - 145s 93ms/step - loss: 0.7465 - acc: 0.8095 - val_loss: 0.7746 - val_acc: 0.8069

Epoch 00017: val_acc improved from 0.80230 to 0.80690, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.017.h5
Epoch 18/50
Learning rate:  0.001
1563/1563 [==============================] - 129s 83ms/step - loss: 0.7417 - acc: 0.8120 - val_loss: 0.8159 - val_acc: 0.7982

Epoch 00018: val_acc did not improve from 0.80690
Epoch 19/50
Learning rate:  0.001
1563/1563 [==============================] - 127s 81ms/step - loss: 0.7336 - acc: 0.8156 - val_loss: 0.8160 - val_acc: 0.7998

Epoch 00019: val_acc did not improve from 0.80690
Epoch 20/50
Learning rate:  0.001
1563/1563 [==============================] - 140s 90ms/step - loss: 0.7283 - acc: 0.8154 - val_loss: 1.0570 - val_acc: 0.7433

Epoch 00020: val_acc did not improve from 0.80690
Epoch 21/50
Learning rate:  0.001
1563/1563 [==============================] - 140s 90ms/step - loss: 0.7220 - acc: 0.8190 - val_loss: 0.7387 - val_acc: 0.8165

Epoch 00021: val_acc improved from 0.80690 to 0.81650, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.021.h5
Epoch 22/50
Learning rate:  0.0001
1563/1563 [==============================] - 141s 90ms/step - loss: 0.6256 - acc: 0.8549 - val_loss: 0.6008 - val_acc: 0.8609

Epoch 00022: val_acc improved from 0.81650 to 0.86090, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.022.h5
Epoch 23/50
Learning rate:  0.0001
1563/1563 [==============================] - 140s 90ms/step - loss: 0.5811 - acc: 0.8673 - val_loss: 0.5694 - val_acc: 0.8710

Epoch 00023: val_acc improved from 0.86090 to 0.87100, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.023.h5
Epoch 24/50
Learning rate:  0.0001
1563/1563 [==============================] - 139s 89ms/step - loss: 0.5608 - acc: 0.8717 - val_loss: 0.5700 - val_acc: 0.8732

Epoch 00024: val_acc improved from 0.87100 to 0.87320, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.024.h5
Epoch 25/50
Learning rate:  0.0001
1563/1563 [==============================] - 139s 89ms/step - loss: 0.5555 - acc: 0.8724 - val_loss: 0.5543 - val_acc: 0.8743

Epoch 00025: val_acc improved from 0.87320 to 0.87430, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.025.h5
Epoch 26/50
Learning rate:  0.0001
1563/1563 [==============================] - 141s 90ms/step - loss: 0.5425 - acc: 0.8778 - val_loss: 0.5551 - val_acc: 0.8729

Epoch 00026: val_acc did not improve from 0.87430
Epoch 27/50
Learning rate:  1e-05
1563/1563 [==============================] - 141s 90ms/step - loss: 0.5253 - acc: 0.8830 - val_loss: 0.5404 - val_acc: 0.8775

Epoch 00027: val_acc improved from 0.87430 to 0.87750, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.027.h5
Epoch 28/50
Learning rate:  1e-05
1563/1563 [==============================] - 135s 86ms/step - loss: 0.5283 - acc: 0.8800 - val_loss: 0.5374 - val_acc: 0.8792

Epoch 00028: val_acc improved from 0.87750 to 0.87920, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.028.h5
Epoch 29/50
Learning rate:  1e-05
1563/1563 [==============================] - 137s 88ms/step - loss: 0.5235 - acc: 0.8834 - val_loss: 0.5389 - val_acc: 0.8794

Epoch 00029: val_acc improved from 0.87920 to 0.87940, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.029.h5
Epoch 30/50
Learning rate:  1e-05
1563/1563 [==============================] - 137s 88ms/step - loss: 0.5225 - acc: 0.8841 - val_loss: 0.5372 - val_acc: 0.8797

Epoch 00030: val_acc improved from 0.87940 to 0.87970, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.030.h5
Epoch 31/50
Learning rate:  1e-05
1563/1563 [==============================] - 137s 88ms/step - loss: 0.5189 - acc: 0.8843 - val_loss: 0.5354 - val_acc: 0.8805

Epoch 00031: val_acc improved from 0.87970 to 0.88050, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.031.h5
Epoch 32/50
Learning rate:  1e-06
1563/1563 [==============================] - 137s 88ms/step - loss: 0.5191 - acc: 0.8834 - val_loss: 0.5334 - val_acc: 0.8813

Epoch 00032: val_acc improved from 0.88050 to 0.88130, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.032.h5
Epoch 33/50
Learning rate:  1e-06
1563/1563 [==============================] - 137s 88ms/step - loss: 0.5160 - acc: 0.8846 - val_loss: 0.5377 - val_acc: 0.8806

Epoch 00033: val_acc did not improve from 0.88130
Epoch 34/50
Learning rate:  1e-06
1563/1563 [==============================] - 137s 88ms/step - loss: 0.5177 - acc: 0.8831 - val_loss: 0.5325 - val_acc: 0.8817

Epoch 00034: val_acc improved from 0.88130 to 0.88170, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.034.h5
Epoch 35/50
Learning rate:  1e-06
1563/1563 [==============================] - 136s 87ms/step - loss: 0.5176 - acc: 0.8847 - val_loss: 0.5340 - val_acc: 0.8816

Epoch 00035: val_acc did not improve from 0.88170
Epoch 36/50
Learning rate:  1e-06
1563/1563 [==============================] - 137s 88ms/step - loss: 0.5181 - acc: 0.8831 - val_loss: 0.5332 - val_acc: 0.8817

Epoch 00036: val_acc did not improve from 0.88170
Epoch 37/50
Learning rate:  1e-06
1563/1563 [==============================] - 137s 88ms/step - loss: 0.5150 - acc: 0.8844 - val_loss: 0.5358 - val_acc: 0.8816

Epoch 00037: val_acc did not improve from 0.88170
Epoch 38/50
Learning rate:  1e-06
1563/1563 [==============================] - 139s 89ms/step - loss: 0.5149 - acc: 0.8858 - val_loss: 0.5348 - val_acc: 0.8805

Epoch 00038: val_acc did not improve from 0.88170
Epoch 39/50
Learning rate:  1e-06
1563/1563 [==============================] - 139s 89ms/step - loss: 0.5174 - acc: 0.8837 - val_loss: 0.5328 - val_acc: 0.8815

Epoch 00039: val_acc did not improve from 0.88170
Epoch 40/50
Learning rate:  1e-06
1563/1563 [==============================] - 138s 88ms/step - loss: 0.5156 - acc: 0.8835 - val_loss: 0.5314 - val_acc: 0.8829

Epoch 00040: val_acc improved from 0.88170 to 0.88290, saving model to C:\Users\RASHU TYAGI\EIP 4 Phase 1\Session 4\saved_models\cifar10_ResNet20v1_model.040.h5
Epoch 41/50
Learning rate:  1e-06
1563/1563 [==============================] - 138s 88ms/step - loss: 0.5186 - acc: 0.8833 - val_loss: 0.5321 - val_acc: 0.8818

Epoch 00041: val_acc did not improve from 0.88290
Epoch 42/50
Learning rate:  5e-07
1563/1563 [==============================] - 138s 88ms/step - loss: 0.5186 - acc: 0.8841 - val_loss: 0.5315 - val_acc: 0.8817

Epoch 00042: val_acc did not improve from 0.88290
Epoch 43/50
Learning rate:  5e-07
1563/1563 [==============================] - 138s 88ms/step - loss: 0.5142 - acc: 0.8841 - val_loss: 0.5328 - val_acc: 0.8819

Epoch 00043: val_acc did not improve from 0.88290
Epoch 44/50
Learning rate:  5e-07
1563/1563 [==============================] - 134s 86ms/step - loss: 0.5174 - acc: 0.8834 - val_loss: 0.5324 - val_acc: 0.8815

Epoch 00044: val_acc did not improve from 0.88290
Epoch 45/50
Learning rate:  5e-07
1563/1563 [==============================] - 127s 81ms/step - loss: 0.5137 - acc: 0.8833 - val_loss: 0.5327 - val_acc: 0.8810

Epoch 00045: val_acc did not improve from 0.88290
Epoch 46/50
Learning rate:  5e-07
1563/1563 [==============================] - 132s 85ms/step - loss: 0.5150 - acc: 0.8852 - val_loss: 0.5335 - val_acc: 0.8811

Epoch 00046: val_acc did not improve from 0.88290
Epoch 47/50
Learning rate:  5e-07
1563/1563 [==============================] - 137s 87ms/step - loss: 0.5159 - acc: 0.8835 - val_loss: 0.5321 - val_acc: 0.8818

Epoch 00047: val_acc did not improve from 0.88290
Epoch 48/50
Learning rate:  5e-07
1563/1563 [==============================] - 138s 88ms/step - loss: 0.5190 - acc: 0.8838 - val_loss: 0.5354 - val_acc: 0.8810

Epoch 00048: val_acc did not improve from 0.88290
Epoch 49/50
Learning rate:  5e-07
1563/1563 [==============================] - 139s 89ms/step - loss: 0.5164 - acc: 0.8849 - val_loss: 0.5323 - val_acc: 0.8814

Epoch 00049: val_acc did not improve from 0.88290
Epoch 50/50
Learning rate:  5e-07
1563/1563 [==============================] - 138s 88ms/step - loss: 0.5129 - acc: 0.8853 - val_loss: 0.5324 - val_acc: 0.8811

Epoch 00050: val_acc did not improve from 0.88290
<keras.callbacks.History at 0x20e983b9780>


Validation Accuracy Received = 88.3% Under 50 epochs.
