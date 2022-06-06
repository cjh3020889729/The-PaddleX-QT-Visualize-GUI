# Jetson平台QT可视化部署Demo方案
The-PaddleX-QT-Visualize-GUI

基于PaddleX推理部署方案构建Jetson的QT可视化界面：[jetson_deploy](./deploy/cpp/docs/jetson_deploy)

实现功能:

    - PaddleClas可视化推理
    - PaddleSeg可视化推理
    - PaddleDetection可视化推理
    - PaddleX可视化推理

界面展示:

![](./deploy/cpp/docs/jetson_deploy/images/gpu_infer.png)


- 特别感谢

    - [lijilai](https://github.com/lijilai): 项目开启Tensorrt加速功能，需要在`deploy/cpp/docs/jetson_deploy/model_infer.cpp`的InitModel函数内的合适位置添加`engine_config.use_trt = true;`——注意启动Tensorrt时，请确保模型运行在GPU运行状态。
