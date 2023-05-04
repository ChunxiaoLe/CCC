实验室内部颜色恒常性课题组入门学习材料
===============================
前言：为了帮助同学，更快的了解和融入颜色恒常性课题组，找到属于自己的研究方向，特拟该资料。

## 该课题成立时间
2020年11月~至今

## 项目组成员（一些最新的研究因保密原因，不便展示）

| 方向       | 描述     | 可能技术 | 目前人员     |
| :-----------: | :--------: | :--------: | :--------: |
| 白平衡    |   sRGB图像白平衡技术    |   元学习、对比学习      |      李春晓（博四，带队）    |
| 颜色恒常性    |    RAW图像白平衡技术   |   迁移学习、对抗学习、多域学习    |   朱家贤(研一) 、张志峰(研三)、 唐宇翔(毕业)    |
| HDR    |    高动态范围图像重建   |   待补充   |   商帅康(研二)    |
| 图像分割    |    夜间图像分割   |   待补充   |   董成豪(研二)    |
| 图像抠图    |    高分辨率下的图像抠图   |  多任务学习、模型轻量化   |   刘飞(研二)    |

## 颜色恒常性背景
+ 定义：相机拍摄的原始RAW图像会受到外界非中性光影响，导致拍摄图像发生色偏，颜色恒常性就是消除色偏现象保持物体本来颜色的过程。
+ 步骤：光照估计：估计出物体表面的光照颜色；颜色矫正，去除光照色偏影响。
+ 示意图如下所示：<img src="https://github.com/ChunxiaoLe/CCC/blob/main/%E9%A2%9C%E8%89%B2%E6%81%92%E5%B8%B8%E6%80%A7%E8%83%8C%E6%99%AF.png" width = "500" height = "300" alt="" align=center />

## 入门文章
组内已投中顶会顶刊：
+ Yuxiang Tang, Xuejing Kang, Chunxiao Li, Zhaowen Lin, Anlong Ming*, Transfer Learning for Color Constancy via Statistic Perspective, AAAI 2022, 人工智能领域顶会.
+ Zhifeng Zhang, Xuejing Kang, Anlong Ming*, Domain Adversarial Learning for Color Constancy,IJCAI 2022，人工智能领域顶会.
+ Chunxiao Li, Xuejing Kang, Zhifeng Zhang, Anlong Ming*, SWBNet: A Stable White Balance Network for sRGB images, AAAI 2023, 人工智能领域顶会.
+ Chunxiao Li, Xuejing Kang, Anlong Ming*, WBFlow: Few-shot White Balance for sRGB Images via Reversible Neural Flows，IJCAI 2023, 人工智能领域顶会.
+ Chenghao Dong, Xuejing Kang, Anlong Ming, ICDA: Illumination-Coupled Domain Adaptation Framework for Unsupervised Nighttime Semantic Segmentation,IJCAI 2023, 人工智能领域顶会.
+ 在投3篇

其它资料：
+ *博客：RAW图像到sRGB图像的全过程*  [[link]](https://ridiqulous.com/process-raw-data-using-matlab-and-dcraw/comment-page-3/#comments)
+ *公开课：RAW图像处理全流程代码* [[link]](https://nbviewer.jupyter.org/github/yourwanghao/CMUComputationalPhotography/blob/master/class2/notebook2.ipynb)
+ 经典论文：Hu, Yuanming and Wang, Baoyuan and Lin, Stephen: "*Fc4: Fully convolutional color constancy with confidence-weighted pooling*" CVPR (2017) [[pdf]](https://openaccess.thecvf.com/content_cvpr_2017/papers/Hu_FC4_Fully_Convolutional_CVPR_2017_paper.pdf) [[code]](https://github.com/yuanming-hu/fc4)
+ 经典论文：Lo Y C, Chang C C, Chiu H C, et al. : "*Clcc: Contrastive learning for color constancy*" CVPR (2021) [[pdf]](https://openaccess.thecvf.com/content/CVPR2021/papers/Lo_CLCC_Contrastive_Learning_for_Color_Constancy_CVPR_2021_paper.pdf) [[code]](https://openaccess.thecvf.com/content/CVPR2021/papers/Lo_CLCC_Contrastive_Learning_for_Color_Constancy_CVPR_2021_paper.pdf)



可用数据集
--------------
各类颜色恒常性数据集大全，[点击链接](http://colorconstancy.com/evaluation/datasets/index.html)，数据集处理可参考[点击链接](https://github.com/ChunxiaoLe/CCC/blob/main/color_constancy_data_process_all.py)

| 数据集名称  | 数据集描述  | 数据集规模    |   作用   | 链接|
| :-----------: | :--------: | :--------: | :--------: | :--------: |
| CCC | 经典单光照数据集 | 568张照片 | 评价单光照颜色恒常性性能 | [链接](https://www2.cs.sfu.ca/~colour/data/shi_gehler/) |
| NUS8 | 单光照+8相机数据集| 1700+图像 | 评价单光照颜色恒常性性能、跨相机性能| [链接](https://cvil.eecs.yorku.ca/projects/public_html/illuminant/illuminant.html) |
| Cube+ | 单光照+双光照数据集、立方蜘蛛 | 1700+张图像 | 评价单光照和双光照颜色恒常性性能 | [链接](https://ipg.fer.hr/ipg/resources/color_constancy) |
| LSMI | 大规模多光照数据集 |7,486张图像 | 评价多光照颜色恒常性性能 | [链接](https://github.com/DY112/LSMI-dataset) |

## 理论知识
+ "*李宏毅机器学习课程.*" 哔哩哔哩 [[link]](https://www.bilibili.com/video/BV1JE411g7XF?from=search&seid=16114573361443816126)

## 动手实践
+ "*动手学深度学习(PyTorch版).*" GitHub [[link]](https://tangshusen.me/Dive-into-DL-PyTorch/#/)
+ "*深度学习框架PyTorch：入门与实践.*" GitHub [[link]](https://github.com/chenyuntc/pytorch-book)


## 实验室自研颜色恒常性代码库平台Anole[[link]](https://github.com/YuxiangTang/Anole)
+ 目的：提供规范化的图像处理框架；提供稳定、公平、可比较的平台；补充RAW图像处理缺口
+ 主要模块：
  + RAW图像处理：RAW图像在相机前后端的处理功能。
  + 颜色恒常性模型：在同一套框架下提供流行和常用颜色恒常性模型。
  + 模型训练和验证：规范化颜色恒常性训练、测试、评价流程。
  + 实验环境配置：Hydra 和可视化技术生成报告来管理实验。

## 其它工具
+ "*Zotero.*" 论文整理工具 [[link]](https://www.zotero.org/)
+ "*connectedpapers.*" 论文追溯工具 [[link]](https://www.connectedpapers.com/)
+ "*Paperswithcode.*" 论文代码查找工具 [[link]](https://paperswithcode.com/)
+ "*Google colab.*" 免费线上GPU平台，如额外需要线下服务器资源，请联系我本人 [[link]](https://colab.research.google.com/notebooks/intro.ipynb)

## 组会和学习时间安排
+ 每周组会安排：一次大组会。组会一般有老师参加，否则有博士师姐组织，主要分享上一周科研进度和论文阅读情况，准备PPT。组会一般在周一。
+ 组内同学学习时间要求：一般：周一至周五白天，9:30-11:30，2:30-5:30，8:00-10:00，无硬性时间要求，根据个人情况出勤
