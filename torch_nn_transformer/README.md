# Sequence-to-Sequence Modeling with nn.Transformer and TorchText

This example is based on a [PyTorch tutorial](https://pytorch.org/tutorials/beginner/transformer_tutorial.html).

* `pt_model.py` contains the pytorch model used by both PyTorch and ONNX Runtime
* `pt_train.py` is used for PyTorch training
* `ort_train.py` is used for ONNX Runtime training 

## Gettings started

* Install Pytorch Nightly
* Install latest ORT
* `python pt_train.py`   # Python training
* `python ort_train.py`  # ORT training

## Limitations

For this example to work with ORT, the following restrictions apply:

* Static batch size and sequences length (bptt)
* No LR scheduler
* Batch size for training and evaluation must match
