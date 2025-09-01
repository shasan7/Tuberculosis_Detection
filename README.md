# Tuberculosis Detection

## Dataset Link: https://www.kaggle.com/datasets/tawsifurrahman/tuberculosis-tb-chest-xray-dataset/

## Kaggle Notebook: https://www.kaggle.com/code/shasan7/tuberculosis-detection/

The images were transformed and normalized using torch, then we fed them to the **pretrained InceptionResNetV2 model for fine-Tuning**

**The best validation accuracy achieved by our model is 99.88%**.

Training Summary:

    Epoch [1/20]  Train Loss: 0.0497 | Train Acc: 98.51%  || Val Loss: 0.4828 | Val Acc: 95.24%
    Saved new best model with val_acc: 95.24%
    Epoch [2/20]  Train Loss: 0.0124 | Train Acc: 99.73%  || Val Loss: 0.4534 | Val Acc: 98.81%
    Saved new best model with val_acc: 98.81%
    Epoch [3/20]  Train Loss: 0.0058 | Train Acc: 99.82%  || Val Loss: 3.6025 | Val Acc: 98.21%
    Epoch [4/20]  Train Loss: 0.0212 | Train Acc: 99.46%  || Val Loss: 0.0331 | Val Acc: 99.64%
    Saved new best model with val_acc: 99.64%
    Epoch [5/20]  Train Loss: 0.0023 | Train Acc: 99.94%  || Val Loss: 0.0057 | Val Acc: 99.88%
    Saved new best model with val_acc: 99.88%
    Epoch [6/20]  Train Loss: 0.0017 | Train Acc: 99.94%  || Val Loss: 0.0104 | Val Acc: 99.64%
    Epoch [7/20]  Train Loss: 0.0015 | Train Acc: 99.94%  || Val Loss: 0.0066 | Val Acc: 99.52%
    Epoch [8/20]  Train Loss: 0.0127 | Train Acc: 99.61%  || Val Loss: 0.1349 | Val Acc: 99.17%
    Epoch [9/20]  Train Loss: 0.0073 | Train Acc: 99.76%  || Val Loss: 0.0545 | Val Acc: 99.52%
    Epoch [10/20]  Train Loss: 0.0039 | Train Acc: 99.91%  || Val Loss: 0.6638 | Val Acc: 99.17%
    Epoch [11/20]  Train Loss: 0.0002 | Train Acc: 100.00%  || Val Loss: 0.0825 | Val Acc: 99.88%
    Epoch [12/20]  Train Loss: 0.0012 | Train Acc: 99.94%  || Val Loss: 0.0090 | Val Acc: 99.52%
    Epoch [13/20]  Train Loss: 0.0061 | Train Acc: 99.79%  || Val Loss: 0.0064 | Val Acc: 99.64%
    Epoch [14/20]  Train Loss: 0.0004 | Train Acc: 100.00%  || Val Loss: 0.0125 | Val Acc: 99.64%
    Epoch [15/20]  Train Loss: 0.0000 | Train Acc: 100.00%  || Val Loss: 0.0064 | Val Acc: 99.76%
    Epoch [16/20]  Train Loss: 0.0000 | Train Acc: 100.00%  || Val Loss: 0.0074 | Val Acc: 99.76%
    Epoch [17/20]  Train Loss: 0.0000 | Train Acc: 100.00%  || Val Loss: 0.0086 | Val Acc: 99.52%
    Epoch [18/20]  Train Loss: 0.0000 | Train Acc: 100.00%  || Val Loss: 0.0041 | Val Acc: 99.88%
    Epoch [19/20]  Train Loss: 0.0006 | Train Acc: 100.00%  || Val Loss: 0.0192 | Val Acc: 99.29%
    Epoch [20/20]  Train Loss: 0.0233 | Train Acc: 99.08%  || Val Loss: 0.1057 | Val Acc: 99.40%


Obtained Results:

    Classification Report:

                  precision    recall  f1-score   support
    
          Normal       1.00      1.00      1.00       700
    Tuberculosis       1.00      0.99      1.00       140
    
        accuracy                           1.00       840
       macro avg       1.00      1.00      1.00       840
    weighted avg       1.00      1.00      1.00       840


    Confusion Matrix:

    [[700   0]
     [  1 139]]


![Confusion Matrix: ](Conf_Mat.png)

![Accuracy Curve: ](Acc.png)

![Loss_Curve): ](Loss.png)
