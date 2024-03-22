# HARSystem
Vite+Vue+Antd+Echarts

系统介绍
在构建活动识别系统中，传感器数据的收集是基础环节，然而传感器所采集的数据通常复杂且不易解读。为此，本系统设计了一套综合解决方案，涵盖了传感器管理以及数据采集过程的可视化展示。此外，为了实现模型的训练与维护，系统还具备了数据集管理、训练参数设置以及训练后模型管理的功能。该系统基于Vue.js框架[65]和Flask框架[66]进行开发，其中Vue.js负责前端页面的构建，而Flask则承担后端服务的处理。整个系统由传感器管理模块、数据处理模块和模型管理模块构成，详细的框架设计如图5.1所示。
 ![image](https://github.com/zmc-0207/HARSystem/assets/62058570/4a38ce17-9ca6-4cd6-aec8-234f6aa11093)

系统首页模块主要展示系统操作日志，以便追踪和监控系统中的各项操作。在传感器管理模块，系统实现了传感器的控制功能，包括断开和连接，同时将传感器收集的数据进行可视化展示。数据处理模块主要负责管理收集到的传感器数据集。而模型管理模块用于设定训练相关参数实现模型的训练及管理训练完成的模型。
5.3 系统实现
5.3.1 系统主界面
系统的登录界面如图5.2所示，用户在此输入账号和密码完成验证后，即可进入系统主界面进行相关操作。
 
图5.2 系统登陆页面
登录后，系统主界面主要展示了功能菜单和系统操作日志，用户可点击查看详细的日志信息，如图5.3所示。
 
图5.3 系统首页
5.3.2 传感器管理
传感器管理模块包含了连接状态信息和传感器实时数据显示功能。其中，连接状态信息主要用于显示人体活动数据采集传感器的地理位置信息，并允许用户控制传感器的连接与断开，如图5.4所示。
 
图5.4 传感器连接控制
传感器实时数据显示功能则致力于数据采集的可视化，包含了惯性传感器的加速度计、陀螺仪和磁力计数据，并以x、y、z三轴的形式进行数据展示，如图5.5所示。
 
图5.5 实时传感器数据可视化
5.3.3 数据集管理
为了对采集后的数据进行进一步处理，数据集管理模块提供了上传、删除、查看和下载等操作，用于管理采集的人体活动数据集，如图5.6所示。
 
图5.6 数据集管理
5.3.4 模型管理
模型管理模块则负责模型的训练及管理。模型训练过程包括数据集处理、参数设置等多个步骤，其训练流程设计如图5.7所示。
 图5.7 模型训练
 
图5.8 模型列表展示
训练完成的模型以列表形式展示，模型信息包括模型文件名称、骨干网络等，如图5.8所示。此外，该模块还支持对第3章和第4章训练的模型进行便捷查。
