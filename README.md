## Nanodet - Face Detecion

**Nanodet** trained models for **Face Detection**. For more details check out [Nanodet repo](https://github.com/RangiLyu/nanodet/). Models were trained with Google Colab servers (Single GPU)

### Directory structure

```
.
├── face                                 # Face related object detection - OpenImages Dataset (20k train : 4k test)
│   ├── nanodet_m_1.0x_sgd                      # Cfg, checkpoints, ... for nanodet_m_1.0x @ 320x320
│   ├── nanodet_m_0.5x_sgd_416x416              # Cfg, checkpoints, ... for nanodet_m_0.5x @ 416x416
|   ├── nd-efficientnet_lite0_more_aug_320x320  # Cfg, checkpoints, ... for efficientnet_lite0 @ 320x320
└── ...
```

*Note: Current models are trained with 20k images (Human faces) of Open Images v6. All these faces satisfy: bbox_area/image_area > 0.03*. So expect poor performance on those images which bbox occupy less than 3% of the image.

## TODO

- [x] ncnn optimized models
- [x] EfficientNet-Lite0 model
- [ ] Yolo Fastest v2
