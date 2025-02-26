## [ 仅 paddle 参数更多 ]torch.nn.functional.upsample_bilinear

### [torch.nn.functional.upsample_bilinear](https://pytorch.org/docs/stable/generated/torch.nn.functional.upsample_bilinear.html#torch.nn.functional.upsample_bilinear)

```python
torch.nn.functional.upsample_bilinear(input, size=None, scale_factor=None)
```

### [paddle.nn.functional.upsample](https://www.paddlepaddle.org.cn/documentation/docs/zh/develop/api/paddle/nn/functional/upsample_cn.html#upsample)

```python
paddle.nn.functional.upsample(x, size=None, scale_factor=None, mode='nearest', align_corners=False, align_mode=0, data_format='NCHW', name=None)
```

Paddle 参数更多，具体如下：
### 参数映射
| PyTorch       | PaddlePaddle | 备注                                                   |
| ------------- | ------------ | ------------------------------------------------------ |
| <font color='red'> input </font> | <font color='red'> x </font> | 表示输入的 Tensor ，仅参数名不一致。  |
| <font color='red'> size </font>             | <font color='red'> size </font>  | 输出 Tensor 的大小。               |
| <font color='red'> scale_factor </font>   | <font color='red'> scale_factor </font>   | 输入的高度或宽度的乘数因子。              |
| -  | <font color='red'> mode </font>   | 插值方法。 Pytorch 无此参数，Paddle 默认为 `’nearest‘`，需要设置为 `‘bilinear'` 。             |
| -  |    <font color='red'> align_corners  </font>  | 是否将输入和输出张量的 4 个角落像素的中心对齐，并保留角点像素的值。Pytorch 无此参数，Paddle 默认为 `False`，需要设置为 `True`。            |
| -  |    <font color='red'> align_mode  </font>         | 双线性插值的可选项。Pytorch 无此参数。Paddle 保持默认即可。            |
| -  |    <font color='red'> data_format  </font>         | 指定输入的数据格式。Pytorch 无此参数。Paddle 保持默认即可。            |
