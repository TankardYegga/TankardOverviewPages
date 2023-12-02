- # 实验结果修正
  collapsed:: true
	- 对[[ResultsForPaper]]中auc和检查点文件代码进行修改后的正确结果
	- 提出的论文模型
	  collapsed:: true
		- 损失比 1：1： 1  d=8 （最终论文使用的结果）
			- ![image.png](../assets/image_1659093953503_0.png)
			- ![image.png](../assets/image_1659096207392_0.png)
			- ![image.png](../assets/image_1659097041048_0.png)
	- 消融实验
	  collapsed:: true
		- densenet121 学习率为0.0008
		  collapsed:: true
			- ![image.png](../assets/image_1659153671297_0.png)
			- ![image.png](../assets/image_1659176607671_0.png)
			- ![image.png](../assets/image_1659176650388_0.png)
		- densenet121 学习率为0.0005
		  collapsed:: true
			- ![image.png](../assets/image_1659832210584_0.png)
			- ![image.png](../assets/image_1659832238077_0.png)
		- resnet18
		  collapsed:: true
			- ![image.png](../assets/image_1659153902889_0.png)
			- ![image.png](../assets/image_1659177358837_0.png)
			- ![image.png](../assets/image_1659177527347_0.png)
		- proposed without multi-output
		  collapsed:: true
			- ![image.png](../assets/image_1659160482008_0.png)
			- ![image.png](../assets/image_1659179060199_0.png)
			- ![image.png](../assets/image_1659179084285_0.png)
	- 对比实验
	  collapsed:: true
		- SVC
		  collapsed:: true
			- ![image.png](../assets/image_1656777023945_0.png)
			- ![image.png](../assets/image_1659972927753_0.png){:height 909, :width 1011}
		- 随机森林
		  collapsed:: true
			- ![image.png](../assets/image_1656776889151_0.png)
			- ![image.png](../assets/image_1659973221878_0.png)
			-
		- K-近距离
		  collapsed:: true
			- ![image.png](../assets/image_1656777091059_0.png)
			- ![image.png](../assets/image_1659972945448_0.png)
			-
		- FDFFE
		  collapsed:: true
			- 中间维度设置为500
				- ![image.png](../assets/image_1659161688071_0.png)
				- ![image.png](../assets/image_1659177972240_0.png)
				- ![image.png](../assets/image_1659178020642_0.png)
				-
				-
				-
				-
			-
				-
				-
				-
		- propopsed with 拼接融合方式
		  collapsed:: true
			- ![image.png](../assets/image_1659163363866_0.png)
			- ![image.png](../assets/image_1659177045183_0.png)
			- ![image.png](../assets/image_1659177105954_0.png)
		- inception 输入图片的大小为 299 * 299， 且使用第三个版本的训练和测试函数（因为inception_v3有辅助输出）
		  collapsed:: true
			- ![image.png](../assets/image_1659166775549_0.png)
			- ![image.png](../assets/image_1659179303762_0.png)
			-
			-
		- vgg11（一层fc）
		  collapsed:: true
			- ![image.png](../assets/image_1659179473383_0.png)
			- ![image.png](../assets/image_1659192219396_0.png)
			- ![image.png](../assets/image_1659192251367_0.png)
			-
		- vgg16（一层fc）
		  collapsed:: true
			- ![image.png](../assets/image_1659191403755_0.png)
			- ![image.png](../assets/image_1659193985746_0.png)
			- ![image.png](../assets/image_1659194036853_0.png)
			-
			-
		- efficientnet(一层fc)
		  collapsed:: true
			- ![image.png](../assets/image_1657119278780_0.png)
			- ![image.png](../assets/image_1659195264313_0.png)
			- ![image.png](../assets/image_1659195307659_0.png)
			-
		- alexnet
		  collapsed:: true
			- ![image.png](../assets/image_1657120385448_0.png)
			- ![image.png](../assets/image_1659197207592_0.png)
			- ![image.png](../assets/image_1659197300429_0.png)
				-
				-
				-
	- 拓展实验
		- resnet_change_pool3  不使用任何池化，直接SDWFM（设置的d为32） 学习率设置为0.0005
		  collapsed:: true
			- ![image.png](../assets/image_1657241483063_0.png)
			- ![image.png](../assets/image_1659197964059_0.png)
			- ![image.png](../assets/image_1659197989026_0.png)
			-
		- DenseNet2_W_WeightPool  先平均池化，再直接SDEFM（d设置为119） 学习率设置为0.0005  只使用一层全连接层
			- ![image.png](../assets/image_1660199728483_0.png)
			- ![image.png](../assets/image_1659832870432_0.png)
			- ![image.png](../assets/image_1659832876580_0.png)
			-
			-
		- DenseNet2_W_WeightPool  先平均池化，再直接SDEFM（d设置为120） 学习率设置为0.0005  只使用一层全连接层
		  collapsed:: true
			- ![image.png](../assets/image_1659832916433_0.png)
			-
	- gram-cam所使用的图片
		- B18RMLO.jpg、B54RMLO.jpg、B90RMLO.jpg
		- M35LMLO.jpg、M77RMLO.jpg、M74LCC.jpg
	- auc图
		- ![roc_curve_paper_final1 [9].jpg](../assets/roc_curve_paper_final1_[9]_1659964362413_0.jpg)
		- ![roc_curve_paper_final4 [2].jpg](../assets/roc_curve_paper_final4_[2]_1659974511963_0.jpg)
		- ![roc_curve_paper_final5 [3].jpg](../assets/roc_curve_paper_final5_[3]_1659974536172_0.jpg)
		- ![roc_curve_paper_final6 [2].jpg](../assets/roc_curve_paper_final6_[2]_1659974564956_0.jpg)
		- ![roc_curve_paper_final_merged_2.jpg](../assets/roc_curve_paper_final_merged_2_1659974585693_0.jpg)
		-
		-
		-
-
- # 研究问题的调研分析
  collapsed:: true
	- 相关论文
	  collapsed:: true
		- Hybrid Biogeography-Based Optimization and Genetic Algorithm for Feature Selection in Mammographic Breast Density Classification. Int. J. Image Graph. 22(3): 2140007:1-2140007:38 (2022)
			- 从文献中可以看出，乳腺组织的高密度是女性乳腺癌发病率上升的根本原因，在女性癌症死亡中发挥着主要作用。此外，在这个计算机辅助诊断系统已成为放射科医师得力助手的时代，研究人员在特征选择技术上仍有改进的空间。本研究旨在提出基于生物地理学的优化和遗传算法的混合版本，用于乳房密度分类中的特征选择，以消除数据集中冗余和不相关的特征；与它一起以实现出色的分类精度或以较少的特征保持相同的精度。为了进行实验，从 mini-MIAS 数据库中选择了 322 张乳房 X 线照片，然后提取了 7 种不同大小的感兴趣区域 (ROI)，以提取对应于每个 ROI 的一组 45 个纹理特征。随后，所提出的算法用于从与每个 ROI 对应的大量特征集中提取最佳特征子集。结果表明，将结果与使用各种参数的其他一些受自然启发的元启发式算法进行比较时，所提出算法的性能优于其他算法。
		- DenseNet for Breast Tumor Classification in Mammographic Images. BIOMESIP 2021: 166-176
		- Mammographic breast density classification using a deep neural network: assessment on the basis of inter-observer variability. Medical Imaging: Image Perception, Observer Performance, and Technology Assessment 2019: 109520O
		-
	- 调研结论
	  collapsed:: true
		- 本论文研究  基于钙化点特征来 对 评级为BI-RADS 4的乳腺数字钼靶图像 进行良恶性分类。
			- 原因在于：BI-RADS 4 的数字钼靶图像 是 非常可疑的恶性，但是活检样本中只有35%是恶性，所以尽可能避开活检来进行诊断。
		- 相关的研究有，但与本论文的研究差别较大：
			- 多分类：分类为BI-RADS 1，BI-RADS 2，BI-RADS 3，BI-RADS 4，BI-RADS 5, BI-RADS 6
			  collapsed:: true
				- ![image.png](../assets/image_1659803402270_0.png)
			- 乳腺肿块的分类：
				- 对于超声图像来说是进行三分类（良性；正常；恶性）
				- 对于数字钼靶乳腺来说也是二分类（良性恶性）
				  collapsed:: true
					- ![image.png](../assets/image_1659803179662_0.png)
					-
			- 乳腺肿瘤密度的类别：
				- ACR BI-RADS 指南（第五版）定义了四个乳房密度类别，可以通过两个超级类别进行区分 “密集”和“不密集”。
		-
	- 李敏学姐论文发表期刊
	  collapsed:: true
		- Li, M., Zhu, L., Zhou, G., He, J., Jiang, Y., & Chen, Y. (2021). Predicting the pathological status of mammographic microcalcifications through a radiomics approach. Intelligent Medicine, 1(03), 95-103.
		- ![image.png](../assets/image_1659949736146_0.png)
		- https://www.sciencedirect.com/journal/intelligent-medicine
		  collapsed:: true
			- ![image.png](../assets/image_1659949964995_0.png)
			  id:: 62f0d37a-3895-4443-901c-0c98a177aaf6
			-
	- 关于为什么只选择4级进行分类诊断
	  collapsed:: true
		- ![image.png](../assets/image_1659950962001_0.png)
		- ![image.png](../assets/image_1659950975609_0.png)
		- ![image.png](../assets/image_1659950986315_0.png)
		- According to the Breast Imaging Reporting and Data System (BI-RADS),  a mammographic abnormality can be radiologically summarized into 7 levels ranging from BI-RADS 0 to BI-RADS 6.  The BI-RADS 3 refers to suspicious benignity, and patients can choose to have regular checkups; the BI-RADS 5 refers to confirmed malignancy, there is no need for a further suspect but direct operation; the BI-RADS 4 is considered highly suspicious for malignancy, and usually a puncture biopsy is required to confirm the ultimate diagnosis.  Obviously, accurate identification of benignity and malignancy on BI-RADS 4 mammographic images plays a key guiding role in the formulation of clinical treatment plans.
		- In the real medical scenario, there are two points to be optimized: first, statistics reveal only about 35% of all biopsies of cancerous MC require a mastectomy, which means that most biopsies are unnecessary; second, only a clinically experienced physician can give a reliable diagnosis. Therefore, the need for assistance with AI technology in this field has become imminent.
		- 这个类别的识别说的是对这个类别进行良恶性分类  而不是说识别出这个类别
		- 通过数据来说明减少活检不会降低诊断过程的有效性   因为大部分活检都是没有必要的
		- 只有经验丰富的医生才能给出比较可靠的诊断
		-
		-
	-
	-
-
- # 分类结果分析
  collapsed:: true
	- 原因： 模型关注的图片区域不准确
		- 根本原因：乳腺钼靶图片本身质量导致的（钙化点的数量、位置、原始大小；截取的ROI区域的尺寸以及位置）。
		  collapsed:: true
			- 换句话说，图片本身就没有那么强的规律
		- 正常情况：
			- 一般来说钙化点大且分散的乳腺钼靶图片是良性的
			- 一般来说钙化点小且密集的乳腺钼靶图片是恶性的
	- 错误分类的具体原因包括：
		- collapsed:: true
		  1. 如果模型将比较分散的良性钙化点区域只识别出了一部分，也就是有可能把分散的钙化点识别成密集的，进而误分类成恶性
			- ![image.png](../assets/image_1659799322932_0.png)
		- collapsed:: true
		  2. 原始ROI的长度和宽度差距较大，将其resize到正方形时回产生横向或者纵向形变
			- ![image.png](../assets/image_1659799811912_0.png)
			- ![image.png](../assets/image_1659799976591_0.png)
		- 3. 原始ROI的尺寸太小，resize到一个较大尺寸时模糊程度严重、钙化点放大程度过大
			- ![image.png](../assets/image_1659800295421_0.png)
		- 4. 钙化点的数目太小了
			- ![image.png](../assets/image_1659800866240_0.png)
			- ![image.png](../assets/image_1659801079777_0.png)
			- ![image.png](../assets/image_1659801191475_0.png)
			-
-
- # 实验的问题
	- 关于论文严谨性的问题：
		- 问题1: 数据集是一个病人对应多张图片（数目不确定），每个图片是从不同的侧面进行拍摄的。我在进行实验的时候：
		  collapsed:: true
			- 一是并没有把每个病人的多张图片进行打包
			  collapsed:: true
				- 我感觉这事实上也做不到 原因是：
					- 模型一般是输入单张图片的，输入多张图片的模型一般是三维图像的二维切片
					- 我觉得病人不同视角图片的重要性不同，并不存在空间上的连续性
			- 二是训练集和测试集中的数据应该是属于不同病人
				- 原因：
					- 同一个病人的不同图片相似性比较高 =》同一病人的不同图片分散出现在训练集和测试集，也就是类似“训练集中的图片再次出现在测试集了”
				- 反驳：
					- 同一个病人的不同图片未必相似：
						- 不同侧面的图片主观认为相似性高，但实际拍摄结果细节上可能差别较大（比如说形状、整体上的分布）
						- 即使是同一个病人的不同图像被分散到训练集、验证集和测试集中去了，这些图像也是不同的图像，并不是说它是一个病人的就是完全一模一样的性质了，如果是这样的话那么同一个病人只取一张图像不就行了
					- 模型本身及其应用：
						- 模型关注的是单张钼靶图像的图像特性
						- 如果一个病人的不同图像测出不同的结果，应该按照预测结果数目多的那个类别作为最终预测类别
			- 思考的结果：
			  collapsed:: true
				- 这篇文章最主要的贡献是在于提高图片准确率，至于其他属于别人后续工程的工作
				- 确定下你投的期刊或者会议比较偏向于哪个
		- 问题2：数据集数量过小，不够有说服力
		  collapsed:: true
			- 按照相同比例重新划分数据集，查看一下效果？
				- 原有的图片本身就是不均匀的：
					- train_loss and train_acc
					  collapsed:: true
						- ![resnet13_change_pool3_2_paper_train_loss.png](../assets/resnet13_change_pool3_2_paper_train_loss_1661044747357_0.png)
						- ![resnet13_change_pool3_2_paper_train_acc [2].png](../assets/resnet13_change_pool3_2_paper_train_acc_[2]_1661044784303_0.png)
					- val_loss and val_acc
					  collapsed:: true
						- ![resnet13_change_pool3_2_paper_val_acc.png](../assets/resnet13_change_pool3_2_paper_val_acc_1661044939073_0.png)
						- ![resnet13_change_pool3_2_paper_val_loss.png](../assets/resnet13_change_pool3_2_paper_val_loss_1661044952401_0.png)
						-
		- 问题3：创新点侧重于模型，而非背景本身
		  collapsed:: true
			- 没有找到数字钼靶类型的通用数据集，有超声的通用数据集且是三分类问题
			- 如果找到另外一个数据集效果好，也仍然不够充分，如果另外那个数据集也是恰好呢？
		- 问题4：原文使用resize，而非image filling
		  collapsed:: true
			- ![image.png](../assets/image_1661043367636_0.png)
			- 因为这种方法会导致图像的一部分出现重复，如果应用到这里，可能会导致钙化点的分布发生变化。
			- 这时候没法使用师姐的机器学习方法作为对比
			  collapsed:: true
				- 因为师姐的方法需要使用钙化点分割结果，而钙化点的分割结果是直接提供的512 * 512的图片
					- ![image.png](../assets/image_1661044577111_0.png)
						- 这个用开闭运算 + 医生去除假阳性点 分割的
		-
	- 第九届医学图像计算青年研讨会 (MICS 2022)上的相关工作： [[Self-adverisal learning for Detection of Clustered Microcalcifications in Mammograms]]
		- ![image.png](../assets/image_1660986676182_0.png)
		- ![image.png](../assets/image_1660986692471_0.png)
			- 任务：先进行分割从而定位到钙化点；划分点簇，对每个点簇计算凸包分析，画出每个点簇的边界（注意目的是为了判断是否存在聚集）
			- 问题：是一个两阶段的过程，而不是端对端的，且需要人手工的参与；假阳率高
			- 难点：
			  collapsed:: true
				- 钙化点不像猫狗等自然图像具有很明显的boundary，其边界的形态非常多样化
				- 钙化点的尺寸不一，一般是0.1-1.0mm，但是也有小于0.1mmm的
				- 钙化点的亮度各异
				- 分割的准确率不够，导致后续的聚类结果也有误差
			- Insights：
				- 多任务且端到端：用钙化点的分割来辅助分类（良恶性）和聚类（钙化点簇的检测）
				- 分类和聚类任务相互促进：
					- 从分类任务推导出聚类结果：
						- 使用online CAM的定位图来划分点簇，并勾画点簇的边界，从而使得聚类任务变得可训练
					- 提高点簇边界勾画的准确率来提升分类效果：
						- 提出了自对抗的学习方式，即将网络本身也作为鉴别器
							- 使得CAM不仅是关注到最具区分性的区域，而是关注到更全面的钙化点簇，
							- 提升对于困难案例的提升效果
		- ![image.png](../assets/image_1660999312377_0.png)
			- id:: 6300d573-03f9-4064-bd63-2ad271d92324
			  collapsed:: true
				- ![image.png](../assets/image_1660999019463_0.png)
			- 整体思路：
				- 模型以Unet为主干网络进行分割；
				- 第一次上采样后的特征图 up_feature_maps_1   先经过log-sum-exp池化和一层fc就产生良恶性分类预测结果；
				  collapsed:: true
					- Log-sum-exp pooling
						- ![image.png](../assets/image_1661010811188_0.png)
						-
				- 将FC的权重作为1*1卷积的参数，然后对 up_feature_maps_1 进行卷积 得到  良性CAM图 和 恶性CAM图：
					- 【1】对两张CAM图与人工标注的检测框计算dice损失，以便CAM图的注意力区域能始终在有效范围内；
					- 【2】对良性CAM和恶性CAM都进行"擦除”处理：
						- 良性CAM中会定位到与乳腺点簇相似的密集腺体，CAM * Image 能够排除掉不感兴趣的区域，那么剩下的区域就是 已经关注到的乳腺钙化点簇 +  密集腺体
						- 恶性CAM中进行反向擦除，通过 （1 - CAM）* image的方式来擦除掉目前具有鉴别性的重点区域，那么剩下的区域其实就是无关区域和部分被遗漏掉的稀疏钙化点簇
					- 【3】Unet的encoder + bottleneck + one layer decoder + pooling + fc层  被复用为 鉴别器，这里的复用即共享参数的意思：
						- 对 良性擦除结果 进行 分类，GT也为良性，从而让网络注重如何区别  密集腺体  和  钙化点
						- 对 恶性擦除结果  进行 分类，GT也为良性，从而让网络学习到 剩余的稀疏钙化点簇中 小部分是与良性有关，而更多的一部分是与恶性相关的，从而使得最终的恶性CAM能定位到被遗漏的稀疏钙化点簇，定位结构更加完整 （待确定，待质疑）
				- 使用的损失函数：
					- ![image.png](../assets/image_1661013089783_0.png)
					- ![image.png](../assets/image_1661013195401_0.png)
						- 分割损失的分母不再使用图像的总像素个数，而是使用  预测分割 和 掩膜 中的 分割部分 的 像素数之和
							- 原因是 钙化点的尺寸过小，BCE 计算的结果可能很小，如果分母过大，最后的损失值也就很小
		- 实验结果
		  collapsed:: true
			- ![image.png](../assets/image_1660987331696_0.png)
			- ![image.png](../assets/image_1660987384615_0.png)
			- ![image.png](../assets/image_1660987411879_0.png){:height 459, :width 807}
			- ![image.png](../assets/image_1660987442581_0.png)
		- 总结
		  collapsed:: true
			- ![image.png](../assets/image_1660987471114_0.png)
		-
		-
	- 关于可解释性深度学习网络
	  collapsed:: true
		- ![image.png](../assets/image_1661013535699_0.png)
		-
- # 写作问题
  collapsed:: true
	- 摘要
	  collapsed:: true
		- DONE 摘要里面没有说明清楚是对4个级别的乳腺钼靶图片进行二分类研究  这个研究目的不够清楚
		  :LOGBOOK:
		  CLOCK: [2022-08-09 Tue 16:37:50]--[2022-09-16 Fri 14:05:47] =>  909:27:57
		  :END:
		- DONE 摘要中两个向量这个词语的表述太模糊了
		  :LOGBOOK:
		  CLOCK: [2022-08-09 Tue 16:37:57]--[2022-09-16 Fri 14:05:46] =>  909:27:49
		  :END:
		- DONE 对于grad-cam的分析写的模棱两可
		  :LOGBOOK:
		  CLOCK: [2022-08-09 Tue 16:38:01]--[2022-09-16 Fri 14:05:45] =>  909:27:44
		  :END:
		- DONE 做了哪些实验也不知道，特别是对于拓展实验的作用完全没有提
		  :LOGBOOK:
		  CLOCK: [2022-08-09 Tue 16:38:07]--[2022-09-16 Fri 14:05:48] =>  909:27:41
		  :END:
		- DONE 实验和模型的意义写的都非常的浅
		  :LOGBOOK:
		  CLOCK: [2022-08-09 Tue 16:38:11]--[2022-09-16 Fri 14:05:48] =>  909:27:37
		  :END:
	- Introduction
	  collapsed:: true
		- DONE 插图有两张，是否合适
		  :LOGBOOK:
		  CLOCK: [2022-08-09 Tue 16:38:20]
		  CLOCK: [2022-08-09 Tue 16:39:35]
		  CLOCK: [2022-08-09 Tue 16:41:37]
		  CLOCK: [2022-08-09 Tue 16:41:41]--[2022-09-16 Fri 14:05:25] =>  909:23:44
		  :END:
		- DONE 需要着重引用学姐那篇论文
		  :LOGBOOK:
		  CLOCK: [2022-08-11 Thu 00:21:33]
		  CLOCK: [2022-08-11 Thu 00:21:35]--[2022-09-16 Fri 14:05:26] =>  877:43:51
		  :END:
		- DONE 贡献是否确实达到了、贡献之间的优先级排序
		  collapsed:: true
		  :LOGBOOK:
		  CLOCK: [2022-08-09 Tue 16:41:48]
		  CLOCK: [2022-08-09 Tue 16:44:12]--[2022-08-10 Wed 20:06:03] =>  27:21:51
		  :END:
			- 我们利用一个共享潜在嵌入为resnet18和densenet121的两个输出向量按位置计算权重并加权求和，这种融合方式被称作基于相似性解码的加权融合方式。提出的模型比单独使用resnet18或者densenet121 以及 拼接融合方式 都要好，这证明了融合机制的有效性和高效性；同时与基于放射组学的机器学习和经典深度学习模型进行对比，我们的模型在定性和定量结果都要出色，其中grad-cam可视化表明提出的模型能更准确地定位到乳腺钙化点所在的区域。
				- We use a shared latent embedding to calculate weights and make the summation for the two vectors that emerged from resnet18 and densenet121 in a position-to-position manner, which is claimed by the paper as the similarity-decoding-based weighted fusion mechanism (SDWFM). The proposed outperforms resnet18 or densenet121 alone and the concatenation fusion strategy,  demonstrating the effectiveness and efficiency of the SDWFM. Also, compared with radiomics-based machine learning and classical deep learning models, our model excels in both qualitative and quantitative performance, where the grad-cam visualisation reveals that the proposed can locate calcifications more precisely.
			- 我们将加权融合机制的应用范围进行拓展，让其替换全局平均池化层，替换后的结果被我们称作加权池化层。我们在resnet18和densenet121上都分别使用了加权池化，结果都要比原模型效果好，这在一定程度上说明了该机制的通用性。（唯一的不足之处在于参数不好调）
				- We replace the global average pooling with the SDWF to form the concept of weighted pooling. The new concept is then applied to resnet18 and densenet121 respectively, and both perform better than the original model. Therefore, the SDWF has generality to a certain extent.
			- 我们增加了两个额外的分类输出，并使用多输出的加权损失函数进行训练。这解决了必须对resnet18和densenet121进行事先预训练的限制，使得模型能一次性进行训练。同时这能缓解多个模型集成时参数累加带来的麻烦，进而提高了在小样本数据上获取丰富特征的能力。
				- We add two additional outputs and design a multi-output weighted loss function to train the model in one pass, which solves the limitation that resnet18 and densenet121 must be pre-trained beforehand. Simultaneously,  this can alleviate the contradiction between the sharp increase in the number of parameters and the trainability of the model when multiple models are integrated, thereby improving the capacity to obtain rich features on small sample data.
		- Trash
			- Another philosophy focuses on the direct merging of model outputs. Hard or soft voting [35] follows the principle of majority rule and reduces variance through the integration of multiple models, increasing the robustness and generalizability; the weighted average takes into account differences in the capabilities of different models.
			- resnet18和densenet121的两个输出向量上每个相同位置的值都转化成对应的两个向量，然后使用一个共享的潜在嵌入与两个向量做内积再求softmax，得到每个位置上的两个权重
			- 我们利用一个共享潜在嵌入为两个向量上的每个对应位置计算一组权重，在每个位置上进行加权后得到融合向量
			-
	- 方法
	  collapsed:: true
		- DONE 是否易于理解
		  :LOGBOOK:
		  CLOCK: [2022-08-09 Tue 16:46:09]
		  CLOCK: [2022-08-09 Tue 16:46:14]
		  CLOCK: [2022-08-09 Tue 16:46:19]--[2022-09-16 Fri 14:05:29] =>  909:19:10
		  :END:
	- 实验
	  collapsed:: true
		- 直接把结果写在实验这一部分了，不知道是否应该分开呢？
		- DONE 检查是否有对d进行说明
		  :LOGBOOK:
		  CLOCK: [2022-08-11 Thu 11:44:26]
		  CLOCK: [2022-08-11 Thu 11:44:31]
		  CLOCK: [2022-08-11 Thu 11:44:41]--[2022-09-16 Fri 14:05:32] =>  866:20:51
		  :END:
		- Trash
			- Additionally, for the number of parameters, the concatenation fusion is 2c1c2 and SDWF is c1c2 plus 2d. Therefore the difference in the number of parameters between the two in our experimental configuration is (c1c2 - d) = 48, which matches the results in the table.
			- 提出的模型其注意力强度从图像的中央区域开始向外递减式扩散，能更为准确地定位到钙化点，而单独的resnet18或densenet121则关注到图像的边缘或者角落，覆盖的钙化点不够全面，这说明了SDWFM能够结合resnet和densenet模型各自的优势，提取到更为有效的特征。
				- The attention intensity of the proposed decreases from the central area of the image, locating the calcifications more accurately, while the individual resnet18 or densenet121 focuses on the edges or corners of the image and cannot cover comprehensive calcifications. Therefore, SDWFM can combine the advantages of resnet and densenet to extract more effective features.
			- X 要么会定位到左上角的一小片区域，要么会定位到左下角的一大片区域，这说明连接融合的可解释性不如提出的融合方式。
				- Resnet18 or densenet121 will either locate a small area in the upper left corner or a large area in the lower left corner, which means that the interpretability of the concatenation fusion is not as good as the proposed SDWFM.
				  id:: 62f4f453-eb49-49b0-bd62-7e3dd3a24724
			- 带有加权池化的resnet18和densenet121、vgg关注到的区域都要比提出的模型范围更大，但是很明显对不包含钙化点的区域过分关注了。
				- Resnet18 with weighted pooling, densenet121 with weighted pooling, and vgg all focus on a larger area than the proposed, but obviously over-focus on areas that do not contain calcifications.
				-
		-
	- 讨论
	  collapsed:: true
		- 对于错误分类的图片分析是在这里写吗？
		- 第一点 定位
			- 每张数字钼靶图像上的ROI必须由专业医生手动进行标注，一方面这非常耗时，另一方面标注的效果十分依赖医生的个人经验。对ROI的自动化检测will be explored in future work.
				- The ROI on each digital mammography image must be manually labeled by a professional physician, which is very time-consuming, and relies heavily on personal experience. Automatic detection of ROI will be explored in future work.
		- 第二点  尺寸
			- 每张钼靶图像上ROI的长宽比和大小都有所差异，这会造成提出的模型产生错误分类。图所示，原始长宽比较大的图片变化成正方形之后会产生横向或者纵向形变；图所示，原始尺寸较小的图片缩放到统一尺寸后会变得模糊。输入的图片可以是任意长宽比和任意尺寸，将被整合进未来的工作。
				- The aspect ratio and size of the ROI on each mammographic image differ, which can lead to a misclassification. As shown in the Fig. , a picture with a larger aspect ratio will be deformed horizontally or vertically after it is transformed into a square; as shown in the figure, a picture with a smaller size will become blurred after being scaled to a uniform size. The input can be of any aspect ratio and any size which will be incorporated into future work.
		- 第三点 模型本身  d参数不好训练（解释一下原因，因为跟向量每个位置的值都有关系，太大就不好训练，太小蕴含的信息不足，不能充分建模向量不同位置的值）  融合机制拓展性还不够强
			- 在模型的实际训练中参数d难以确定，因为当d太大时，模型变得难以训练而欠拟合，当d太小时，向量包含的信息量不足，容易导致过拟合。我们会探索更多有效且方便的融合方式，试图使得模型融合的范围能是任意多个随机挑选的模型。
				- The parameter d in SDWF is difficult to determine. When d is too large, the model tends to underfit for the growing parameters, and when d is too small,  the information contained will be insufficient, which easily leads to overfitting. We will explore more efficient and more convenient fusion strategies so that the range of model fusion can be any number of randomly selected models.
		- 第四点  钙化点本身的大小问题  图片本身的灰度分布问题   这个可能得数字钼靶成像技术的一些进步才能解决
			- 如图所示，部分钼靶图片中的钙化点尺寸过小而难以被模型识别；如图所示，部分钼靶图片中钙化点的灰度与周围乳腺组织过于接近而难以区分。这是由于图像本身的质量问题导致的，也是为什么医生针对同一个病人需要拍摄多张钼靶图片的原因。这个可能得数字钼靶成像技术或者预处理技术的一些进步才能解决。
			- There are other reasons for misclassification. In mammography images,  if the calcifications are too small, it will be difficult to identify them; If the grayscale of calcifications is too close to the surrounding breast tissue, it will be hard to distinguish. Essentially, it's a quality issue with the images themselves, which is why doctors need to take multiple mammography images of the same patient. It can be addressed with some advancement in preprocessing technology or digital mammography imaging.
	- 结论
	  collapsed:: true
		- 对于缺陷和不足到底是写在讨论里面还是结论里面
		-
- # 论文第一遍修改
	- DONE 修改论文问题
	  collapsed:: true
	  :LOGBOOK:
	  CLOCK: [2022-09-13 Tue 11:40:04]
	  CLOCK: [2022-09-13 Tue 11:40:06]--[2022-09-20 Tue 17:24:59] =>  173:44:53
	  :END:
		- 长句太多 需要进行拆解
		- 部分语句别人读不懂
		- 关于为什么使用resnet和densenet121并没有引用任何相关的论文？到底是在方法里面写还是在introduction里面写？
		- 给的模型图不够清楚、相似性加权的这个过程示意图也不清楚
		- 直接跳到相似性解码的加权机制，关于为什么这样设计并没有做出任何解释？这里相似性的含义是什么？shared deep latent是怎么出来的？model fusion block最好有箭头指向其具体的设计结构？
		- 关于两点不足解释得非常不恰当，第一个原因应该是图片的方差比较大，第二个是影像组学的推广
		- 不应该说数字钼靶图片是所有技术中更好的，而是应该指出其相对的优点，我记得MICCAI那篇钼靶的论文里面写的很好，可以借鉴一下
		- 背景、问题或者任务介绍、问题本身的困难
		  :LOGBOOK:
		  CLOCK: [2022-09-16 Fri 15:05:12]
		  CLOCK: [2022-09-16 Fri 15:05:15]
		  :END:
		- 没有提及钙化点的作用、研究背景好像与钙化点没有任何关系、后面研究数据的表明显得非常突兀、用到了太多难懂的专业词汇、没有说清楚任务到底是分类还是检测，也没有说明这个分类预钙化点到底有什么关系
		- 问题的难点需要分段写还是必须写在第一段呢？
		- 这个评判标准写的非常僵硬，在描述一些例子的时候应该拿准确的图片进行举例（描述和例子的关系在这里写的很模糊），而且由此导致的分类困难没有说明白，对于AI诊断的这个痛点并不能让读者感受到。不要用第一个困难、第二个困难这种描述方式了。灰度接近这个描述也不太对，灰度相近也就是视觉效果相似，然后就是难以区分或者是容易造成干扰。应该描述临床医生即便有丰富经验，也不能准确诊断。没有在本段引出AI的必要性。
		- 学姐的方法只是基于放射组学的一种，所以不需要把对应的步骤描述得这么清楚，同时其他的组学方法也要拿出来讲。缺点的描述非常不生动。后面一种方法的关注点是否描述得过于简单了？只关注模型的结构，不关注模型的背景？对于这个乳腺问题，到底关注的是模型的什么呢？是钙化点的检测？是钙化点簇的聚类？没有调研关于乳腺钼靶图像的相关论文啊？这个few-shot问题需不需要使用这样的专业术语？后面介绍的模型融合方法也没有讲在乳腺或者类似医学问题上的实例？综述中使用多个例子时，要怎么进行连接？怎么安排不同例子的先后顺序？如何避免描述一个例子太长？例子描述得是否清晰呢？没有大量降低参数量，这个缺陷非常不清晰，这么多模型难道都没有试图降低大小的？优点描述得也不明确，比如增加鲁棒性和泛化性，分别是针对什么的鲁棒性和泛化性？软硬投票和后面的三种策略是否有重合呢？融合方法里可以增加简单相加这个，简单相加其实不是这个原始加权相加的一个特例，需要特别说明一下吧？没有说明是怎么解决这两个问题的？多任务的点也没有提，事实上这本身就不是一个创新点？到底需不需要在摘要中适当描述方法呢？如果需要，又需要描述到什么样的详细程度？
		- 对比学习里面的移除特征冗余、特征相似性、KL散度
			- 移除特征冗余性的过程和影像组学的筛选特征的过程很相似
			- 自动编码器部分要怎么描述呢？
			- 基于相似性来计算权重的，很像对比学习里面筛选特征的过程，正负样本通过两个分支得到两个特征向量，然后这两个特征向量计算KL散度之类的，太相似就移除某些特征？
			- 两个模型学习出的共有特征是应该需要关注的
		- check一下集成学习那篇综述的论文的影像因子，和老师PAMI给的多分支论文进行对比
		- 重点要阐述为什么要这样计算权重
	- 论文垃圾箱
	  collapsed:: true
		- but a serious bias of classification will be induced if there are discrimination conflicts between different feature vectors.
		- We use the similarity-decoding-based weighted fusion mechanism (SDWFM) to fuse the feature vectors of resnet18 and densenet121. The proposed model outperforms resnet18 or densenet121 alone and the concatenation fusion strategy, demonstrating the effectiveness of the SDWFM. Furthermore, when compared to radiomics-based machine learning and classical deep learning models, our model outperforms both in qualitative and quantitative performance. For reason analysis, the grad-cam visualizations reveal that the proposed can locate calcifications more precisely.
		- We apply SDWF in fusing the feature vectors corresponding to all pixels of the feature map. The procedure can replace the global average pooling and form the concept of weighted pooling. We carry out the concept on resnet18 and densenet121 respectively, and both obtain better performance than original ones. The generality of SDWF is thus validated to some extent.
		- To address the limitation that resnet18 and densenet121 must be pre-trained beforehand, we allow them both to have their outputs for classification and design a multi-output weighted loss function to guide them to learn useful features. This enables the model to be trained in a single pass. Importantly, this strategy alleviates the training difficulties caused by the proliferation of parameters and the limited number of samples during model integration.
		-
		- 这种策略缓解了模型集成时因为参数量激增和样本数量有限所造成的训练困难.
	- 论文问题-2
		- DONE 对集成深度学习的引用过多
		  :LOGBOOK:
		  CLOCK: [2022-09-22 Thu 08:54:20]
		  CLOCK: [2022-09-22 Thu 08:55:16]--[2022-09-22 Thu 19:30:50] =>  10:35:34
		  :END:
			- 查找具体的单项知识点在哪里？
		- DONE 连接词衔接不恰当
		  :LOGBOOK:
		  CLOCK: [2022-09-22 Thu 09:04:53]--[2022-09-22 Thu 19:30:51] =>  10:25:58
		  :END:
		- DONE 在解释方法的核心思想时并没有引用什么论文
		  :LOGBOOK:
		  CLOCK: [2022-09-22 Thu 09:04:57]
		  CLOCK: [2022-09-22 Thu 09:06:25]--[2022-09-22 Thu 19:30:53] =>  10:24:28
		  :END:
		- DOING resnet和densenet互补的论文文献
		  :LOGBOOK:
		  CLOCK: [2022-09-22 Thu 09:22:39]
		  CLOCK: [2022-09-22 Thu 09:22:46]--[2022-09-22 Thu 09:22:59] =>  00:00:13
		  CLOCK: [2022-09-22 Thu 19:31:00]
		  :END:
			- DPN 28
		- DOING 改完方法后再修改摘要中的方法描述
		  :LOGBOOK:
		  CLOCK: [2022-09-22 Thu 09:23:37]--[2022-09-22 Thu 19:30:54] =>  10:07:17
		  CLOCK: [2022-09-22 Thu 19:31:00]
		  :END:
		-
	-
- # 中文草稿
	- 显然，这意味着一个模型提取的所有单个特征都具有一样的权重，这实际上是不合理的。一个深度学习模型提取到的所有特征虽然从语义上不像影像组学有充足的数学可解释性，但单个特征值之间应该具有不同的重要性。只有这样模型的决策融合才有意义，即能够合并不同模型各自的有用特征，移除各自的无用特征。于是，我们提出multi-group feature fusion的概念，其将不同特征向量同一位置上的所有特征作为一组，即Gi = {vi_0,vi_1,...,vi_n-1}(i=0,1,...,l-1， l是特征向量的长度，n是模型的个数)，然后对组内的特征通过加权平均融合成一个特征值。可以发现，这种方式将多个模型中相关的多个特征按照重要程度压缩成了一个特征，降低了信息尺度的同时却增加了信息的有效密度，同时各个组别之间的特征相对隔离，不会因为融合而使得每个特征趋于相似。第二个方面是组内权重的计算。两类现象使其必须是data-adaptive：钼靶图片中钙化点在分布、位置、形状、大小都有差异，因而图片本身的方差比较大；用于进行融合的模型选择有很多种组合。于是，为了解决此问题，我们提出了一种创新的基于相似性解码的加权融合机制。首先，我们使用同一个线性矩阵将所有特征向量上的所有特征拓展为一维特征向量，这能增加特征的信息量，但并不会改变特征的相对关系。接着，我们引入了一个待学习的潜在向量L，用以表征一组完全有效且纯净的分类特征。最后，所有的特征向量与L分别进行内积，同一组内的特征向量之间利用内积值的归一化得到权重。内积反应了特征向量与L的相似性，相似性越大，代表特征越有效，其权重也设置得更大。
	-
	- 原生的加权平均中，一个权重对应于一个模型的特征向量的整体，所有权重之和为1.
	- 引出加权聚合的方式，然后解释存在的问题
	- 多任务融合的论文可以引用，原论文里面是多个任务之间的信息是相互补充的，然后由这个得出多个模型之间的信息可能是相互补充的，也有促进分类性能提高的潜力，这里就可以开始解释resnet18和densenet121被选中的原因了。但是这里的多个损失函数应该是为了引导resnet18和densenet学习到对于分类有用的信息，这样才能为后面的信息融合提供前提或者基础。我们使用这个机制去模仿多任务学习里的训练策略？
	- 就说本论文设计的机制在resnet和densenet构成的双模型上进行了应用，具体的设计细节和训练策略见方法部分。
	- 两模型融合到底在哪里提及才比较合适呢？因为我这里的示意图画的全部是两个特征向量的。我前面的描述需不需要进行形式化的描述？我觉得肯定是加上数学描述符的，但是需不需要用公式呢？感觉在摘要中使用公式会特别奇怪。两模型融合的选项到底在方法里面描述还是摘要里面描述呢？可是这样的话感觉方法里面的内容是不是太少了。
	- 我们旨在对加权平均这一融合机制进行改进，改进围绕权重的两个方面。第一面是加权融合的作用对象，vallina加权平均中的权重针对的是一个模型对应的特征向量这个整体，但是受传统影像组学的启发，每个特征的重要性都不尽相同，不同模型提取到的分类特征有共性也有差异，每个模型提取到的特征都是不完善的，也就是说都会提取到一部分有用的特征一部分无用的特征，决策融合如果要发挥作用就得合并不同模型提取到的有用特征，移除各自的无用特征，所以权重融合可以被重新定义为对特征向量的每个位置处的值，或者说特征值进行加权融合，权重之和同样必须为1，某个模型的特征向量的某个位置只要权重不为0，就说明其对分类有贡献，权重为0，则说明对分类没有贡献，这种方式可以避免连接方式学习到的冗余，单个模型提取的特征向量本身就已经有冗余了，如果再拼接，就会造成更多的冗余；这种方式可以保留将多个有用的特征合并到一个单元里去，相当于是对信息压缩，或者说影像组学里面的特征过滤。第二个方面就是权重的计算方式，依据分类问题特点的不同，特征向量的长度也应该进行相应的调整，所以需要计算特征权重的组数也不相同，因为不同分类问题的图片有不同的特点，部分数据集的图片本身就具有较大的差异，本研究问题中的钙化点分布位置、形状、大小造成了数据本身较大的方差，不同图片对应的权重应该不同，鉴于以上两点，自适应地进行方差计算是迫切需要的。还有如何针对每个位置上对应的若干个单个特征值计算一组和为1的权重呢？很明显单个值的维度过小，不包含丰富的信息量，难以计算出一个合理的让人信服的权重，所以需要对每个单个特征值进行拓展，使用同一个矩阵对所有特征向量的所有位置的单个特征值进行转化，一方面这能够保持原始所有特征的相对大小关系，同时极大地降低了参数量。经过此类转换之后，单个特征值都转变成了一个较短的特征向量，权重的计算利用这两个特征向量就可以。我们可以假想一个能够代表分类特征的全部有效的特征向量，然后每个位置上的特征向量与该位置计算内积，内积在一点过程度上反映相似性，相似性越大代表与分类特征越相关，这在具体实现的时候是通过共享的潜在嵌入实现的。值得注意的是，本文针对的是两模型融合。
	- 虽然深度学习提取到的特征是不可解释的，但不同位置的特征值对于分类任务的贡献就像手工特征一样也具有不同的重要性。
	- 为了避免原始每个模型对应特征向量中的冗余特征过多，原始特征向量的长度就不宜过长，所以设置为20.
	-
- # paper_content_draft
	- # introduction
		- Breast cancer is commonly recognized as one of the leading causes of death for females worldwide [1]. Early diagnosis of breast cancer is crucial to reduce the pain of patients and increase the survival rate [2]. Among the available screening tools, digital mammography is the primary choice because of its low cost, high sensitivity [3], and special ability to scrutinize possible invasive ductal carcinoma in situ (DCIS)[4][5][6][7]. According to the Reporting and Data System (BI-RADS) Atlas [8], a mammographic abnormality can be radiologically separated into seven levels, ranging from BI-RADS 0 to BI-RADS 6. The BI-RADS 4 means the cancer is highly suspicious for malignancy and requires pathological examination for final confirmation of being cancerous(malignant) or noncancerous(benign). However, real clinical statistics reveal only about 35% of cancerous MCs in biopsy samples necessarily require a mastectomy[9]. As a result, we aim to reduce unnecessary biopsies by improving the classification accuracy of BI-RADS 4 cases.
			- \bibitem{b1} F. Bray et al., ``GLOBOCAN estimates of incidence and mortality worldwide for 36 cancers in 185 countries,'' \emph{CA: a Cancer Journal for Clinicians}, vol. 71, no. 2021, pp. 209--249, 2020.
			- \bibitem{b2} L. Tabar et al., ``Mammography service screening and mortality in breast cancer patients: 20-year follow-up before and after introduction of screening,'' \emph{The Lancet}, vol. 361, no. 9367, pp. 1405--1410, 2003.
			- \bibitem{b3} American Cancer Society, ``Breast Cancer Early Detection and Diagnosis,'' emph{The Society}, 2008.
			-
		- In clinical practice, radiologists make judgments based on the characteristics of clustered microcalcifications presented in the mammograms. Calcifications associated with malignant cancers are empirically smaller in size and more densely distributed [10]. In addition, as the samples shown in Fig. 1, the benign calcifications tend to be coarsely shaped (round, oval, or popcorn-shaped) while the malignant ones tend to be finely shaped (worm-like, cast-like, branched). However, calcifications vary greatly between patients in terms of size and shape. Specifically, scattered points within calcifications have a radius size that ranges mostly from 0.1 to 1.0mm, even sometimes <0.1mm [11]. Another challenge comes from the low contrast between microcalcifications and surrounding tissues. The similar grayscale makes it hard to distinguish the key indicators of cancer. Therefore, there is a strong demand of employing artificial intelligence technology to assist the diagnosis process.
			- bibitem{b10} D. Sankar, and T. Thomas, ``A new fast fractal modeling approach for the detection of microcalcifications in mammograms,'' Journal of Digital Imaging, vol. 23, no. 5, pp. 538--546, 2010.
			- bibitem{b11} Y. Ma et al., ``A novel shape feature to classify microcalcifications,'' in \emph{2010 IEEE International Conference on Image Processing}, pp. 2265--2268, 2010.
			- Low contrast between microcalcifications and surrounding tissue results in many false positive points in the diagnosis.
			- \bibitem{b12}  \textcolor{black}{Q. Huang, Y. Luo, and Q. Zhang, ``Breast ultrasound image segmentation: a survey,” International Journal of Computer Assisted Radiology and Surgery'' \emph{International Journal of Computer Assisted Radiology and Surgery}}, vol. 12, no. 3, pp. 493-507, 2017.}
			- Q. Huang, Y. Luo, and Q. Zhang, “Breast ultrasound image segmentation: a survey,” International Journal of Computer Assisted Radiology and Surgery, vol. 12, no. 3, pp. 493-507, 2017.
		- In the literature, clustered Mc classification approaches can be categorized into two groups: traditional machine learning based on radiomics and deep learning.
		- The former emphasizes manually extracting and filtering out more informative and more discriminative features and adopts combinations or variants of traditional machine learning models to classify the features. For example，837 textures and 9 shape features were extracted and filtered by an XGBoost-embedded recursive feature elimination technique in [13]. [14] generates a series of multi-scale MC cluster graphs to investigate the scale-specific graph topological changes. [15] performs a multi-scale image decomposition based on the Haar wavelet transform and extracts features on each decomposition and the corresponding gray-level co-occurrence matrix (GLCM)[16]. [17] employs a correlation-based feature selection technique and discusses the clinical relevance of the selected features. [18] reduces irrelevant features using principal component analysis (PCA) [19]. The machine learning models chosen typically include KNN [20], AdaBoost [21], Random Forest [22], and Gaussian Naive Bayes [23]. Although this radionics-based feature signature provides some degree of interpretability, it is difficult and expensive in terms of time and expertise[24]. Subsequently, deep learning methods, especially convolutional neural networks (CNNs), have been successfully applied to the issue, and show the advantage of simple preprocessing and faster reasoning []. [] uses VGG16 to detect breast MC clusters, uses Mask RCNN to find MCs, and uses Inception V3 to identify benignity and malignancy. [] combines the two view-level decisions implemented by two neural networks into a global decision that mimics the biopsy results. Clearly, this approach focuses on the module design and module combination on the basis of standard structures such as ordinary convolution [15], dilated convolution [], autoencoder [], etc. However, the applicable models are confined to those with few parameters and simple structures, such as resnet [], densenet [], alexnet [],  vgg [], mobilenet [] and etc. More complex structures like swin-transformer [], vision-transformer [], CaiT [] and Deep ViT [] are highly likely to be undertrained due to the lack of efficient large-scale medical datasets.
			- Alam, Nashid, and Reyer Zwiggelaar. "Evaluation of Graph Topological Features in Digitized Mammogram for Microcalcification Cluster Classification." 2018 Digital Image Computing: Techniques and Applications (DICTA). IEEE, 2018.
			- \bibitem{14}  \textcolor{black}{N. Alam, and R. Zwiggelaar, ``Evaluation of Graph Topological Features in Digitized Mammogram for Microcalcification Cluster Classification," in \emph{2018 Digital Image Computing: Techniques and Applications (DICTA)}. IEEE, 2018, pp. 1--7.}
			- \bibitem{15} \textcolor{black}{A. Fanizzi et al., ``Ensemble discrete wavelet transform and gray-level co-occurrence matrix for microcalcification cluster classification in digital mammography," \emph{Applied Sciences}, vol. 9, no. 24, pp. 5388, 2019.}
			- \bibitem{17}  \textcolor{black}{N. Alam, E. RE. Denton, and R. Zwiggelaar, ``Classification of microcalcification clusters in digital mammograms using a stack generalization based classifier,'' \emph{Journal of Imaging}, vol. 5, no. 9, pp. 76, 2019.}
			- \bibitem{18}  \textcolor{black}{E. Avşar, and K. Buluş, ``A Novelty Detection Approach to Classification of Breast Tissue Containing Microcalcifications,'' in \emph{Proceedings of the International Conference on Research in Adaptive and Convergent Systems}, pp. 100--103, 2017.}
			- \bibitem{19}  \textcolor{black}{I. T. Jolliffe, and J. Cadima, ``Principal component analysis: a review and recent developments," \emph{Philosophical Transactions of the Royal Society A: Mathematical, Physical and Engineering Sciences}, vol. 374, no. 2065, pp. 20150202, 2016.}
			- \bibitem{24}  \textcolor{black}{Z. Yu et al., ``Melanoma recognition in dermoscopy images via aggregated deep convolutional features,'' \emph{IEEE Transactions on Biomedical Engineering}, vol. 66, no. 4, pp. 1006--1016, 2018.}
			- \bibitem{25}  \textcolor{black}{Z. Yu et al., ``A deep convolutional neural network-based framework for automatic fetal facial standard plane recognition,'' \emph{IEEE journal of biomedical and health informatics}, vol. 22, no. 3, pp. 874--885, 2017.}
			- \bibitem{26}  \textcolor{black}{Y. C. Hsieh et al., ``Combining VGG16, Mask R-CNN and Inception V3 to identify the benign and malignant of breast microcalcification clusters,'' in \emph{2020 International Conference on Fuzzy Theory and Its Applications (iFUZZY)}, pp. 1--4, 2020.}
			- \bibitem{27} \textcolor{black}{A. J. Bekker, ``A multi-view deep learning architecture for classification of breast microcalcifications,'' in \emph{2016 IEEE 13th International Symposium on Biomedical Imaging (ISBI)}, pp. 726--730, 2016.}
			-
			- \bibitem{40} \textcolor{black}{M. A. Ganaie et al., ``Ensemble deep learning: A review,'' \emph{arXiv preprint arXiv}, 2021.}
			-
			- \bibitem{44} \textcolor{black}{T. Xiao et al., ``Comparison of transferred deep neural networks in ultrasonic breast masses discrimination,'' \emph{BioMed research international}, vol. 2018, 2018.}
			- \bibitem{45} \textcolor{black}{W. X. Liao et al., ``Automatic identification of breast ultrasound image based on supervised block-based region segmentation algorithm and features combination migration deep learning model,'' \emph{IEEE journal of biomedical and health informatics}, vol. 24, no. 4, pp.984--993, 2019.}
			-
			- \bibitem{46} \textcolor{black}{A. Shakya, M. Biswas, and M. Pal, ``CNN-based fusion and classification of SAR and Optical data,'' \emph{International Journal of Remote Sensing}, vol. 41, no. 22, pp. 8839--8861, 2020.}
			- \bibitem{47} \textcolor{black}{H. Dong et al., ``PGA-Net: Pyramid feature fusion and global context attention network for automated surface defect detection,'' \emph{IEEE Transactions on Industrial Informatics}, vol. 16, no. 12, pp. 7448--7458, 2019.}
			- \bibitem{48} \textcolor{black}{C. Ju, A. Bibaut, and M. van der Laan, ``The relative performance of ensemble methods with deep convolutional neural networks for image classification,'' \emph{Journal of Applied Statistics}, vol. 45, no. 15, pp. 2800--2818, 2018.}
			-
			-
			-
			-
			-
			-
			-
			-
			-
			-
			-
			-
			-
			-
			-
			-
			-
			-
			-
			-
			-
		- Recently, ensemble deep learning has gradually developed, combining several individual models to obtain better generalization performance []. This methodology has seldom been explored in the current issue of research, and [] just takes the maximum of the predictions of various models as the final classification of microcalcifications. The ensemble strategy has three common types []. The first type refers to the classic methods[] including bagging[], boosting[], and stacking[]. The second type refers to general methods[], including negative correlation learning, implicit or explicit ensembles, and homogeneous or heterogeneous ensembles. The third type refers to decision fusion[], which is a special subset of the so-called feature fusion which has been extensively utilized in image classification[], data fusion[], and other fields[].It means training several base learners and then using some rules to aggregate their outputs. Notably, the outputs are the prediction vectors of the same length from the fully connected layers.  The rule used to combine the outputs determines the actual performance, and the two most straightforward ways are concatenation(see Fig. 2(a)) and averaging (see Fig. 2(b)). Concatenation can directly increase information density, but when the feature vector is too lengthy, the computation overhead will be high and redundant info will be added. Averaging actually consists of the two sub-steps of summation and division, and therefore can improve the generalization performance due to the reduction of the variance among the models. On the other side, it is not data adaptive and will lead to less optimal performance [] as it is sensitive to biased learners. One adaption of averaging is weighted averaging assigning specific weights with a sum of one to the feature vectors of different models separately. This method has a severe drawback in that the weights are not set in an interpretable manner and are consequently incomprehensible. Advanced strategies of decision fusion[] include majority voting, Bayes optimal classifier, stacked generalization, and super learner, which are based on complex mathematical theories.
		- In this work, we aim to enhance the fusion mechanism of weighted averaging by looking at two aspects of the weights. The first aspect is about the object that the fusion mechanism operates on. In the vanilla weighted averaging, a weight corresponds to the entire feature vector of a model, and all weights sum to 1. Obviously, this means that all individual features extracted by a model have the same weight, which is actually unreasonable. Although the features extracted by a deep learning model are not as mathematically interpretable as radiomics, individual feature values should have different importance. Only in this manner does the decision fusion of the models have the potential to improve performance, that is, it can combine the useful features of different models and remove their useless features. Therefore, we propose multi-group feature fusion. In its definition, all the features in the same position of different feature vectors are treated as in the same group and are then fused into one by weighted averaging. The formulation is as follows (i=0,1,...,l-1, l is the length of the feature vector, n is the number of models):
			- Gi = {vi_0,vi_1,... ,vi_n-1}
			- vi_fused = weight_averaging(Gi)
		- Hence, this approach compresses multiple features related to multiple models into one feature based on their importance, reducing the scale of info while increasing the effective density. Meanwhile, the features of each group are relatively isolated, so each fused feature will tend to remain discriminative rather than become similar due to fusion. The second aspect is the calculation of within-group weights. The process must be data-adaptive for two reasons: the calcification points in the mammography image are different in distribution, location, shape, and size, resulting in a relatively large variance of the images; there are many model combinations to choose from. To address this problem, we design a novel similarity-decoding-based weighted fusion mechanism, abbreviated as SDWFM. First, we use the same linear matrix to scale all of the features on all of the feature vectors into one-dimensional vectors, which increases the information but does not change the features' relative relationship. Following that, we introduce a deep latent vector L that can be learned to represent a set of hypothesized perfect i.e., fully valid and purely clean classification features. Finally, the inner products of all the one-dimensional vectors and L are calculated respectively, and the results in the same group are normalized to obtain the corresponding weights. Thus, we can claim that by decoding the similarity between one-dimensional vectors transformed from single feature values and the perfect features L, we acquire features' relative importance in the form of weights. The greater the similarity is, the more effective the feature is, and the larger the weight is set.
		- We use the similarity-decoding-based weighted fusion mechanism (SDWFM) to fuse the feature vectors of resnet18 and densenet121. Experiments are conducted on datasets collected by ourselves. The proposed model outperforms resnet18 or densenet121 alone and the concatenation fusion strategy, demonstrating the effectiveness of the SDWFM. Furthermore, when compared to radiomics-based machine learning and classical deep learning models, our model outperforms both in qualitative and quantitative performance. For reason analysis, the grad-cam visualizations reveal that the proposed can locate calcifications more precisely.
		- We apply SDWF in fusing the feature vectors corresponding to all pixels of the feature map. The procedure can replace the global average pooling and form the concept of weighted pooling. We carry out the concept on resnet18 and densenet121 respectively, and both obtain better performance than original ones. The generality of SDWF is thus validated to some extent.
		- To address the limitation that resnet18 and densenet121 must be pre-trained beforehand, we allow them both to have their outputs for classification and design a multi-output weighted loss function to guide them to learn useful features. This enables the model to be trained in a single pass. Importantly, this strategy alleviates the training difficulties caused by the proliferation of parameters and the limited number of samples during model integration.
	-