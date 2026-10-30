---
title: "3D 模型技术要求"
doc_id: G7RGSNQFZ2BAG7K3
source: https://sellercentral.amazon.com/help/hub/reference/external/G7RGSNQFZ2BAG7K3
language: zh-CN
fetched_at: 2026-10-30T13:22:42
---

# 3D 模型技术要求

## 3D 通用指南

现在，大多数商品分类都支持 3D 内容，帮助买家评估商品。以下是创建符合亚马逊买家体验要求的 3D 模型的通用指南。

**注意： **有关更多特定商品分类的标准，请参阅相应分类的 3D 指南。

**重要术语**

- glTF/GLB： GL 传输格式是 Khronos Group 为传输 3D 内容而开发的开源文件格式。

- GLB 是 glTF 文件格式的二进制版本，它将所有纹理和网格数据合并到一个文件中。这是我们推荐的格式。

- 有关 glTF 规范的信息，请前往 [Khronos Group](https://registry.khronos.org/glTF/specs/2.0/glTF-2.0.html) 网站。

- PBR： 基于物理的渲染是一种渲染方法，能够更真实地呈现光源与 3D 模型交互的方式。亚马逊建议使用金属度/粗糙度工作流程来创建材质。

**所有 3D 模型的通用指南**

**注意： **3D 资产不得包含任何人物图像。

- 我们接受 .GLB 和 .glTF 文件格式的资产及其相应的支持纹理。

- 3D 模型应该能在详情页面上对实物商品进行详细而准确的虚拟展示。

- 模型中每个部件的尺寸和形状都与其他部件成比例缩放。

- 模型参照实物按比例缩放，这意味着模型的尺寸与组装后的商品尺寸相符。尺寸不准确可能会导致资产发布延迟。

- 我们接受 .PNG 和 .JPG 格式的纹理文件。

## 3D 资产质量和买家期望

我们的买家依靠准确的 3D 模型来评估商品，这是一种“所见即所得”体验。逼真的模型可以建立信任，帮助买家做出更明智的购买决定。

为此，与参照的实物对比，3D 模型应显示恰当的细节水平，并以真实可信的方式呈现商品材质。如果模型未能准确呈现详情页面图片中所示商品，则可能无法通过我们的质量保证评估流程。

## 3D 资产一般技术要求 - 几何体

- 模型参照实物比例构建，这意味着模型的尺寸与组装后的商品尺寸相符。

- 模型不可拥有超过 20 万个三角形。

- 验证模型完整性，以避免出现与网格相关的缺陷，如无效的三角形、边、顶点、面或反转法线。

- 模型不可包含修改器、动画关键帧、摄像机或灯光。

- **对于眼镜模型** - glTF 资产必须包含以下节点名称：

- Frame、TempleR、TempleL、LensR、LensL。（请参阅用于定义 glTF 节点的[针对眼镜 3D 模型的虚拟试戴要求](https://sellercentral.amazon.com/gp/help/external/GPJDL6HF5QL69W4B)）

## 3D 资产一般技术要求 - 纹理和材质

- 我们接受 .PNG 和 .JPG 格式的纹理文件。我们不接受直接在 JSON 中嵌入图像资源的 glTF 文件。

- 纹理分辨率不应低于 2K（2048 像素 x 2048 像素），也不应高于 4K（4096 像素 x 4096 像素）。不支持双面纹理。

- 支持的纹理（.PNG 或 .JPG）必须是每个通道一个纹理。纹理必须是正方形，分辨率必须是 2 的幂次方，所有边的最终分辨率不大于 4K（4,096 x 4,096 像素），不小于 2K（2,048 x 2,048 像素）。

- 所有材质均为 PBR 金属度-粗糙度或 PBR 标准。

- UV 必须全部位于一个纹理图集内，即置于主坐标空间 (0,1) 中，同时最大化 UV 空间的使用。

**必选贴图**：

- 必须使用 **RGB 的基色贴图**。

- 漫反射贴图必须包含一个 α 通道，以防出现部分透明对象或表面。透明度应映射到上述 α 通道中。

**注意： **透明度不应用于代表折射指数材质（例如玻璃、厚塑料或丙烯酸等）。请使用 glTF 扩展“KHR_materials_transmission”。

- 线性（灰度）格式的**金属度**为必选项。

- 线性（灰度）格式的**粗糙度**为必选项。

**可选纹理贴图：**

- 线性-RGB 格式的**法线**为必选项。

- 线性（灰度）格式的**不透明度**。导出的贴图将在不透明度通道添加透明度值。

- 线性（灰度）格式的**高度**。如果向高度通道添加了任何高度值，则导出一个贴图；

- 线性（灰度）格式的**厚度**是必选项，用来指定物体的厚度。

- 线性（灰度）格式的**遮挡度**包含照明信息。

**支持的 glTF 扩展：**

**注意： **目前不支持此处未列出的 glTF 扩展。

- **KHR_materials_sheen**

- 丝绒材质需要 sRGB 格式的**光泽颜色**。

- 丝绒材料的光泽需要线性（灰度）格式的**光泽粗糙度**。

- **KHR_materials_reports**：玻璃和透明材质必须使用线性（灰度）格式的 KHR_materials_reports。

- **KHR_materials_clearcoat**

- 光亮表面的附加偏移量（颜色值）需要使用 sRGB 格式的**清漆颜色**。

- 光亮表面的附加偏移量（光亮值）需要使用线性（灰度）格式的**清漆粗糙度**。

- **KHR_materials_ior**：需要使用线性（灰度）格式的 KHR_materials_ior 来指定反射或折射数据。

- **KHR_materials_volume**

- **KHR_draco_mesh_compression**

- **KHR_interactivity**

## 3D 资产对齐和方向规范

上传前正确对齐模型网格，这一点非常重要。对齐不准或方向错误会给买家带来不佳体验，并会延迟或妨碍模型发布。请参阅完整的 [3D 成像对齐指南](https://m.media-amazon.com/images/G/01/imaging/3D/Help_Pages/Amazon_Supplemental_2-3D_Alignment_Guide.pdf)，了解每种对齐类型的示例。

- 所有模型应与地板、墙壁或天花板对齐。模型“正面”由 3D 成像对齐风格指南决定，所有模型必须与面向正 Z 空间的模型“正面”对齐。

- “向上”世界轴为正 Y。

- 网格必须相对于世界空间 0,0,0 正确对齐，才能与特定商品类型（地板、墙壁、落地镜或天花板）对齐。

- **地板/桌面模型对齐（任何通常位于地板、柜台或桌面的商品，包括鞋靴）**

- 所有地板对齐模型必须置于 Y=0 平面上，并且所有几何体延伸到正 Y 空间。

- 所有面向地板的模型以 X 轴和 Z 轴的底面为中心。枢轴点应为 0,0,0。

- 对于鞋靴，请确保鞋头伸展到正 Z 空间。

- **天花板模型对齐（安装在天花板的灯具或吊扇等）。**请注意，“房内查看 (ViYR) AR”应用目前不支持天花板模型。

- 所有面向天花板的模型置于 Y 轴上或 Y=0 平面下方，并且所有几何体延伸到负 Y 空间。

- 所有面向天花板的模型“悬挂”在顶表面的底部。枢轴点应为 0,0,0。

- **墙壁模型对齐**

- 所有面向墙壁的模型的“背面”必须与 XY 平面 (Z=0) 对齐，并且所有几何体延伸到正 Z 空间。

- 所有面向墙壁的模型以 X 和 Y 轴为中心，枢轴点 0,0,0 位于背面的中心点。

- **落地镜对齐（落地镜）**

- 所有面向落地镜的模型的“背面”必须与 XY 平面 (Z=0) 对齐，并且所有几何体延伸到正 Z 空间。

- 倾斜角度。

- **眼镜对齐**

- 使用地板对齐

- 眼镜资产必须轴对齐

- 眼镜前部与世界正 Z 方向一致 (0,0,1)

- 眼镜上部与世界正 Y 方向一致 (0,1,0)

- 眼镜侧面与世界 X 方向一致 (1,0,0) 或 (-1,0,0)

- 镜片面向前面正向

- 枢轴点为 0.0.0，与镜桥对齐。

- **鞋子对齐**

- 使用地板对齐

- 鞋靴资产必须轴对齐

- 鞋靴前部与世界正 Z 方向一致 (0,0,1)

- 鞋靴上部与世界正 Y 方向一致 (0,1,0)

- 鞋面与世界 X 方向一致 (1,0,0) 或 (-1,0,0)

## 3D 文件格式和导出指南

**文件格式**

- 我们接受 .GLB（二进制）和 .glTF 文件格式的资产及其相应的支持纹理。

**如果导出为 glTF**

- 许多 3D 内容创建应用程序有 glTF 导出程序插件，可在 Khronos Group 的 [glTF-Generator-Registry](https://github.com/KhronosGroup/glTF-Generator-Registry/blob/main/dist/REGISTRY.md) 中找到这些插件

- **必须：** 单独导出 glTF 资产（.glTF + .bin + 纹理）。请参阅以下示例作为参考：

![](https://m.media-amazon.com/images/G/01/rainier/help/SEDIT-6133144_1.png)

- 必须使用 [Khronos Group 的 glTF-Validator 工具](https://github.khronos.org/glTF-Validator/)检查文件是否符合技术要求。

## 3D 模型质量保证流程的好处

我们的 3D 模型指南可确保创建的模型在视觉和技术上始终保持准确和逼真。3D 模型的多功能性让我们能够为广泛的 3D 买家体验 (CX) 创建资产和应用程序，包括“房内查看”“虚拟试戴”“3D 视图”“CGI 详情页面图片”“VR 体验”等。以下示例展示了如何将单一资产输入到不同的买家体验中并吸引买家参与互动。

![](https://m.media-amazon.com/images/G/01/rainier/help/SEDIT-6133144_2.png)

## 3D 资产工具和资源

提示和资源链接：

- [Khronos Group 实时资产创建指南](https://github.com/KhronosGroup/3DC-Asset-Creation/blob/main/asset-creation-guidelines/RealtimeAssetCreationGuidelines.md)。

- [glTF 2.0 规范](https://registry.khronos.org/glTF/specs/2.0/glTF-2.0.html)。

- 许多 3D 内容创建软件有 glTF 导出程序，可在 Khronos Group 的 [glTF-generator-registry](https://github.com/KhronosGroup/glTF-Generator-Registry/blob/main/dist/REGISTRY.md) 中找到这些程序的列表。

- Khronos Group 的 [glTF-Validator 工具](https://github.khronos.org/glTF-Validator/)可用于检查文件是否符合技术要求。

- 虽然我们目前不提供亚马逊查看器来预览 3D 资产，但是可以将 glTF 文件拖放到 [Khronos 样本查看器](https://github.khronos.org/glTF-Sample-Viewer-Release/)中，输出结果与我们网站的显示效果几无二致。

- 基于物理的渲染信息

- 介绍[基于物理的渲染](https://substance3d.adobe.com/tutorials/courses/the-pbr-guide-part-1)理论。

- 介绍[创建 PBR 材质](https://substance3d.adobe.com/tutorials/courses/the-pbr-guide-part-2)的指南。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/G7RGSNQFZ2BAG7K3
