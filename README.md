# Adversarial Training with pytorch

`python main.py -a`

## Accuracy (WIP)
| Model             | Acc.        |
| ----------------- | ----------- |
| [VGG16](https://arxiv.org/abs/1409.1556)              | --.--%      |
| [ResNet18](https://arxiv.org/abs/1512.03385)          | --.--%      |
| [ResNet50](https://arxiv.org/abs/1512.03385)          | --.--%      |
| [ResNet101](https://arxiv.org/abs/1512.03385)         | --.--%      |
| [MobileNetV2](https://arxiv.org/abs/1801.04381)       | --.--%      |
| [ResNeXt29(32x4d)](https://arxiv.org/abs/1611.05431)  | --.--%      |
| [ResNeXt29(2x64d)](https://arxiv.org/abs/1611.05431)  | --.--%      |
| [DenseNet121](https://arxiv.org/abs/1608.06993)       | --.--%      |
| [PreActResNet18](https://arxiv.org/abs/1603.05027)    | --.--%      |
| [DPN92](https://arxiv.org/abs/1707.01629)             | --.--%      |

## Learning rate adjustment
I manually change the `lr` during training:
- `0.1` for epoch `[0,150)`
- `0.01` for epoch `[150,250)`
- `0.001` for epoch `[250,350)`

Resume the training with `python main.py -r --lr=0.01 -a`

## References

1. Authors' code: [Towards Deep Learning Models Resistant to Adversarial Attacks, Madry et al.](https://github.com/MadryLab/cifar10_challenge)

2. Baseline code: [kuangliu/pytorch-cifar](https://github.com/kuangliu/pytorch-cifar)