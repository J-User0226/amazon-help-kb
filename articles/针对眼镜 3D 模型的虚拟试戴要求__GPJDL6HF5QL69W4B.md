---
title: 针对眼镜 3D 模型的虚拟试戴要求
doc_id: GPJDL6HF5QL69W4B
source: https://sellercentral.amazon.com/help/hub/reference/external/GPJDL6HF5QL69W4B
language: zh-CN
fetched_at: 2026-10-30 13:46:55
---

# 针对眼镜 3D 模型的虚拟试戴要求

为了在体验时确保 3D 模型的正确位置，需要定义节点。使用 glTF 文件，可通过将 3D 模型切割为单独的网格，并应用所需的命名规则来定义节点。定位和碰撞系统依赖于节点名称在 CX 中实现正确的操作。

节点名称应遵循以下术语： Frame、TempleR、TempleL、LensR、LensL。

*3D 网格中的节点示例*

*节点名称*

*Frame node（镜框网状切割）*

*TempleL node（左侧太阳穴网格切割）*

*LensL node（左侧镜片网格切割）*

**例外情况**

对于一片式镜片（请参见以下示例），节点名称应遵循以下术语： Frame、TempleR、TempleL、Lens。

**材料**

为了以遵循基本物理规律的方式呈现透明材料，必须对眼镜模型的相关部分应用 glTF 扩展 KHR_materials_transmission。

如果 glTF 清单文件中存在 KHR_materials_transmission，则“alphaMode”的值必须设置为“OPAQUE”，并且“transmissionFactor”必须设置为 (0,1] 的范围内。

镜片的粗糙度值应设置为 1（白色）或 0（黑色），不支持介于中间的值。

**方向与对齐**

**前面正向**： 镜片面向前面正向

**对齐：** 中心

**中心点：** 对齐眼镜鼻梁的中心位置

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GPJDL6HF5QL69W4B
