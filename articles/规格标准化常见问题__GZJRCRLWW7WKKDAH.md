---
title: "规格标准化常见问题"
doc_id: GZJRCRLWW7WKKDAH
source: https://sellercentral.amazon.com/help/hub/reference/external/GZJRCRLWW7WKKDAH
language: zh-CN
fetched_at: 2026-10-30T14:24:29
---

# 规格标准化常见问题

#### 总体而言，有什么变化？

亚马逊对卖家输入的“规格”进行了标准化处理，以便买家对于数量信息有更一致的体验。卖家提供的包含“规格”的信息不再显示，而是显示来自其他目录属性，如 item_weight、dimensions（item_length_width 和 item_length_width_height）、capacity、unit_count、number_of_items、net_content_weight、net_content_volume 和 net_content_count）的信息。目录属性是针对每种商品类型定义的，它们用于计算特定商品类型的规格。规格将以标准格式显示，其中包含与该商城相关的标准计量单位。有关更多信息，请参阅**此更改会影响哪些商品类型？**

#### 为什么要按照所述指南显示规格信息？

买家有权了解其下单后将会收到的商品的规格。此信息目前通过“规格”属性显示。规格信息难以理解会给买家造成困惑，因此，规格信息应采用标准格式。此外，相对于规格信息不完善的商品，规格信息正确的商品有着更高的商品销售总额。亚马逊致力于通过创建相关机制使信息格式保持一致，从而帮助卖家达到此数据质量标准。

#### 这对我的业务有什么好处？

规格信息标准化可以提高买家在购物时发现商品的几率，并改善其购物体验。我们发现，对于具有有效“规格”值的 ASIN，买家购买量更高，因此其商品销售总额也更高。

#### 数量信息标准化对买家有哪些好处？

系统会根据相应地理位置，在“规格”值中仅显示买家熟悉的内容（例如，对于美国境内的买家，重量信息显示为“盎司”；对于英国境内的买家，重量信息显示为“克”）。浏览亚马逊商城时，买家会查看规格信息，这些信息来自商品重量、容量、尺寸、单位计数和商品数量。有关更多信息，请参阅**此更改会影响哪些商品类型？**

#### 什么是标准化规则？为什么会采用这些规则？

标准化规则会在可能的情况下自动重新调整“规格”值的格式。为了方便卖家操作，亚马逊逻辑会在内部从已填写的目录属性中获取数据，并填充显示页面上的规格属性。卖家需要确保从其卖家端更新目录属性。例如，对于“壶铃”商品类型，如果您之前在亚马逊美国商城中提交了 32 磅的值作为规格属性，则根据 item_weight 属性中填写的信息（假设 item_weight 填写为 32 磅或使用其他磅的单位变体），系统会自动将其标准化为“32 磅”。

**重要： **不同的商城将拥有不同的商品。

#### 创建商品信息的体验会有哪些变化？

创建商品信息的过程没有变化。但是，请务必为以下属性输入正确信息，以便系统根据相关商品类型得出对应的“规格”值：

- UNIT_COUNT

- NUMBER_OF_ITEMS

- NET_CONTENT（重量、体积、数量、面积）

- INCONTINENCE_PROTECTOR_SIZE

- TOTAL_SERVINGS_PER_CONTAINER

- Weight（商品重量）

- Dimension（商品长度和宽度，商品长度、宽度和高度，商品厚度、宽度和高度）

- Capacity

- action

- bed_size

- bike_type

- construction_type

- fishing_rod_power

- frame_size.with_mat

- frame_size.without_mat

- ice_production_capacity

- iron_board_surface.length

- iron_board_surface.width

- item_shape

- item_volume

- item_width.maximum

- item_width.minimum

- load_index

- lure_weight.maximum

- lure_weight.minimum

- magnification_maximum

- max_input_sheet_capacity

- number_of_drawers

- number_of_items

- objective_lens.diameter

- paper_size

- pocket_length_width

- rim.size

- section_width

- sheet_count

- tire.aspect_ratio

有关更多信息，请参阅**此更改会影响哪些商品类型？**

#### 标准化“规格”值何时开始显示？

更新后的规格值将于 2022 年 6 月，在列表 1 的**此更改会影响哪些商品类型**部分共享的以下商品类型中可见。列表 2 中的商品类型将于 2023 年 7 月上线。无论是新创建 ASIN 商品信息还是更新现有 ASIN 时，都必须填写必填属性（如**创建商品信息的体验将如何变化**中所述），才能显示“规格”值。

#### 现有 ASIN 的“规格”和变体主题中已经输入的值会怎样？

在“规格”中输入的值不会显示在商品详情页面上。亚马逊将自动合并相应目录属性的值以填充“规格”属性，“规格”将以为商品类型定义的标准格式显示在商品详情页面上。目录属性是针对每个商品类型定义的。有关属性和商品类型列表，请参阅**此更改会影响哪些商品类型**部分。执行新属性后，变体主题的值不会发生变化。如果现有 ASIN 的“规格”值是有效值，则无需重新提交“规格”值。但是如果要更改“规格”值，必须编辑相应的目录属性，这些属性用于计算该商品类型的规格。

#### 如果我使用的是上传数据集成工具，该怎么办？

上述标准同样适用于使用上传数据发布商品信息的方法。因此，如果您使用上传数据集成工具，此工具必须符合属性发布标准。在开始执行新属性之前，亚马逊已提前大约 60 天发布了这些标准，为您留出了充足的时间来采用新标准。

#### 10.如果选项中没有我的商品规格或它被归入其他属性，该怎么办？

首先验证您为商品重量、尺寸（例如 item_length_width、item_length_width_thickness 和 item_length_width_height）、容量、单位计数、商品数量和 Net_Content 等目录属性选择的值是否准确无误，因为这些属性将决定后续属性下的可用值。如果您认为自己确实遇到了选项中没有您商品规格的情况，您可以向销售伙伴支持提交请求，亚马逊将审核您的请求。

#### 为什么网站上显示的规格与我提交的“规格”信息不同？

为了改善买家体验，亚马逊对网站上显示的“尺码”进行了标准化处理，以消除重复信息并规范尺码属性中数量信息的显示方式。提供准确的规格信息和清晰的商品详情页面有助于建立买家信心并提高销量。

以从数量得到的规格为例，如果两位卖家发布的商品具有相同的数量包装，但各自提供的“规格”值却不同（一位卖家提供的值为“32 个”，另一位卖家提供的值为“32 个 [1 件]”），则亚马逊“规格”标准化逻辑将根据“unit_count”/“number_of_items”+ <unit_count.type> + (“Pack of”+ number_of_items) 这一公式来识别有关信息。

因此，如果单位计数为 32 个，商品数量为 1，则亚马逊得出的“规格”值为“32 个（1 件装）”。这样一来，买家只能看到一个版本的“规格”，且这两位卖家的报价都将关联到同一商品。

同样，对于壶铃，如果您之前在亚马逊美国商城中提交了 32 磅的值作为规格属性，则根据 item_weight 属性中填写的信息，系统会自动将其标准化为“32 磅”。不同的商城将具有不同的商品，在本示例中，单位是英镑，此单位仅适用于美国商城。

#### 为什么我的商品规格在商品详情页面上不显示？

为了改善买家体验，亚马逊保留删除不准确或格式错误的尺码的权利。如果“规格”不符合“规格”标准格式，就会被移除。

#### 我是否应该更新全部现有商品的信息？

为了改善买家体验，我们要求所有 SKU 或 ASIN 都更新必填属性。如果您有以下适用商品类型的任何 ASIN 的商品信息，则需按照下文**卖家如何更新属性？**中的说明更新数据。在常规目录编辑（如定价更新和商品信息更新）期间，系统会通知您添加缺少的“商品重量”、“容量”、“商品长宽高”、“商品形态”、“商品数量”等属性信息。

#### 卖家如何更新属性？

卖家可以通过卖家平台编辑单个 ASIN 或批量上传修改后的值。具体操作步骤如下：

**单个 ASIN 属性更新：**

- 前往[管理所有库存](https://sellercentral.amazon.com/myinventory/inventory)。

- 搜索该 ASIN 后点击【编辑】。

**注意： **这将打开一个新选项卡。

- 在【重要信息】部分，填写特定商品类型规格的目录属性，如 【item _weight】、【item_length_width_height】、【item_length_width_thickness】、【item_length_width】、【unit_count】、【unit_count_type】 和 【number_of_items】（请参阅**此更改会影响哪些商品类型**了解不同商品类型的规格属性列表）。

- 点击【保存】。

**属性更新的批量上传流程**：

- 前往[批量上传商品](https://sellercentral.amazon.com/product-search/bulk)。

- 下载名为【库存】文件的库存模板，或生成所需的分类模板。

- 下载特定分类文件并填写 SKU 和目录属性的信息，更新删除（并填写部分更新）。

- 以制表符分隔文本格式保存文件。

- 前往[批量上传商品](https://sellercentral.amazon.com/product-search/bulk)，然后上传您的库存文件。

- 文件类型选择【库存文件（默认）】，然后上传。

#### 此变更会影响哪些商品类型？

规格标准化适用于消费类商品和硬百货商品的商品类型。以下是规格标准化范围内的两个商品类型列表。

## 列表 1 - 规格来自数量目录属性

| 商品类型 | 规格值依据的属性 |
| --- | --- |
| WRITING_INSTRUMENT | 单位计数和商品数量 |
| WATER | 单位计数和商品数量 |
| WASTE_BAG | 单位计数和商品数量 |
| VITAMIN | 单位计数和商品数量 |
| VINEGAR | 单位计数和商品数量 |
| TOPICAL_HAIR_REGROWTH_TREATMENT | 单位计数和商品数量 |
| TOOTHBRUSH_HEAD | 单位计数和商品数量 |
| TOOTHBRUSH | 单位计数和商品数量 |
| TOOTH_WHITENER | 单位计数和商品数量 |
| TOOTH_CLEANING_AGENT | 单位计数和商品数量 |
| TOILET_PAPER | 单位计数、商品数量和净含量 |
| THICKENING_AGENT | 单位计数和商品数量 |
| TEXTILE_DEODORIZER | 单位计数和商品数量 |
| SYRUP | 单位计数和商品数量 |
| SURFACE_PROTECTION_WAX | 单位计数和商品数量 |
| SURFACE_CLEANING_WIPE | 单位计数和商品数量 |
| SUNSCREEN | 单位计数和商品数量 |
| SUGAR_SUBSTITUTE | 单位计数和商品数量 |
| SUGAR | 单位计数和商品数量 |
| SNACK_MIX | 单位计数和商品数量 |
| SNACK_FOOD_BAR | 单位计数、商品数量和净含量 |
| SNACK_CHIP_AND_CRISP | 单位计数和商品数量 |
| SLEEP_MASK | 单位计数和商品数量 |
| SKIN_TREATMENT_MASK | 单位计数和商品数量 |
| SKIN_SERUM | 单位计数和商品数量 |
| SKIN_MOISTURIZER | 单位计数和商品数量 |
| SKIN_FOUNDATION_CONCEALER | 单位计数和商品数量 |
| SKIN_EXFOLIANT | 单位计数和商品数量 |
| SKIN_CLEANING_WIPE | 单位计数和商品数量 |
| SKIN_CLEANING_AGENT | 单位计数和商品数量 |
| SKIN_BLEMISH_REMOVAL_TOOL | 单位计数和商品数量 |
| SHELLFISH | 单位计数和商品数量 |
| SHAVING_AGENT | 单位计数和商品数量 |
| SHAMPOO | 单位计数和商品数量 |
| SELF_TANNER | 单位计数和商品数量 |
| SEASONING | 单位计数和商品数量 |
| SEAFOOD | 单位计数和商品数量 |
| SANITARY_NAPKIN | 单位计数和商品数量 |
| SAFETY_MASK | 单位计数和商品数量 |
| RICE_MIX | 单位计数和商品数量 |
| RAZOR_BLADE_CARTRIDGE | 单位计数和商品数量 |
| PUFFED_SNACK | 单位计数和商品数量 |
| PROTEIN_SUPPLEMENT_POWDER | 单位计数和商品数量 |
| PROTEIN_DRINK | 单位计数和商品数量 |
| PRETZEL | 单位计数和商品数量 |
| POPCORN | 单位计数和商品数量 |
| PET_FOOD | 单位计数和商品数量 |
| PERSONAL_FRAGRANCE | 单位计数和商品数量 |
| PASTRY | 单位计数和商品数量 |
| PAPER_TOWEL | 单位计数、商品数量和净含量 |
| PAINT | 单位计数和商品数量 |
| PACKAGED_SOUP_AND_STEW | 单位计数和商品数量 |
| NUTRITIONAL_SUPPLEMENT | 单位计数、商品数量和每个容器内的总食用分量 |
| NUT_BUTTER | 单位计数和商品数量 |
| NOODLE | 单位计数和商品数量 |
| NON_DAIRY_CREAM | 单位计数和商品数量 |
| NAIL_TREATMENT | 单位计数和商品数量 |
| NAIL_POLISH_REMOVER | 单位计数和商品数量 |
| NAIL_POLISH | 单位计数和商品数量 |
| MOUTHWASH | 单位计数和商品数量 |
| MINERAL_SUPPLEMENT | 单位计数和商品数量 |
| MILK_SUBSTITUTE | 单位计数和商品数量 |
| MENSTRUAL_CUP | 单位计数和商品数量 |
| MEDICATION | 单位计数和商品数量 |
| MEDICAL_TEST_STRIP | 单位计数和商品数量 |
| MEAL_REPLACEMENT_BEVERAGE | 单位计数和商品数量 |
| MASCARA | 单位计数和商品数量 |
| MANUAL_SHAVING_RAZOR | 单位计数和商品数量 |
| MAKEUP_PRIMER | 单位计数和商品数量 |
| LIP_COLOR | 单位计数和商品数量 |
| LIP_BALM | 单位计数、商品数量和净含量 |
| LEGUME | 单位计数和商品数量 |
| LEAVENING_AGENT | 单位计数和商品数量 |
| LAUNDRY_DETERGENT | 单位计数和商品数量 |
| JUICE_AND_JUICE_DRINK | 单位计数和商品数量 |
| JERKY | 单位计数和商品数量 |
| INSECT_REPELLENT | 单位计数和商品数量 |
| INCONTINENCE_PROTECTOR | 单位计数、商品数量和失禁防护用品规格 |
| HONEY | 单位计数和商品数量 |
| HERBAL_SUPPLEMENT | 单位计数和商品数量 |
| HAND_SANITIZER | 单位计数和商品数量 |
| HAIRBAND | 单位计数和商品数量 |
| HAIR_TIE | 单位计数和商品数量 |
| HAIR_STYLING_AGENT | 单位计数和商品数量 |
| HAIR_ROLLER | 单位计数和商品数量 |
| HAIR_REMOVAL_AGENT | 单位计数和商品数量 |
| HAIR_COLORING_AGENT | 单位计数和商品数量 |
| HAIR_CLIP | 单位计数和商品数量 |
| HAIR_CLEANER_CONDITIONER | 单位计数和商品数量 |
| GIFT_WRAP | 单位计数、商品数量和净含量 |
| FOOT_SCRAPER | 单位计数和商品数量 |
| FOOD_COLORING | 单位计数和商品数量 |
| FLOUR | 单位计数和商品数量 |
| FLAVORED_DRINK_CONCENTRATE | 单位计数和商品数量 |
| FALSE_NAIL | 单位计数和商品数量 |
| FALSE_EYELASH | 单位计数、商品数量和净含量 |
| FACIAL_TISSUE | 单位计数和商品数量 |
| FACE_SHAPING_MAKEUP | 单位计数和商品数量 |
| FABRIC_SOFTENER | 单位计数和商品数量 |
| EYELID_COLOR | 单位计数和商品数量 |
| EYEBROW_COLOR | 单位计数和商品数量 |
| ESSENTIAL_OIL | 单位计数和商品数量 |
| EDIBLE_OIL_ANIMAL | 单位计数和商品数量 |
| EARPLUG | 单位计数、商品数量和净含量 |
| DRY_SHAMPOO | 单位计数和商品数量 |
| DISHWASHER_DETERGENT | 单位计数和商品数量 |
| DENTAL_FLOSS | 单位计数和商品数量 |
| DAIRY_BASED_DRINK | 单位计数和商品数量 |
| CULINARY_SALT | 单位计数和商品数量 |
| CRACKER | 单位计数和商品数量 |
| COSMETIC_SPONGE | 单位计数和商品数量 |
| COSMETIC_POWDER | 单位计数和商品数量 |
| CONTACT_LENSES | 单位计数和商品数量 |
| CONDOM | 单位计数和商品数量 |
| CONDITIONER | 单位计数和商品数量 |
| COFFEE | 单位计数和商品数量 |
| CLEANING_AGENT | 单位计数和商品数量 |
| CHEWING_GUM | 单位计数和商品数量 |
| CAKE | 单位计数和商品数量 |
| BREAKFAST_CEREAL | 单位计数和商品数量 |
| BOTTLE_NIPPLE | 单位计数和商品数量 |
| BODY_LUBRICANT | 单位计数和商品数量 |
| BODY_DEODORANT | 单位计数和商品数量 |
| BLEACH | 单位计数和商品数量 |
| BATHWATER_ADDITIVE | 单位计数和商品数量 |
| BATHING_SPONGE | 单位计数和商品数量 |
| BAKING_MIX | 单位计数和商品数量 |
| BABY_FORMULA | 单位计数和商品数量 |
| BABY_BOTTLE | 单位计数和商品数量 |
| ASTRINGENT_SUBSTANCE | 单位计数和商品数量 |
| AREA_DEODORIZER | 单位计数和商品数量 |

## 列表 2 - 规格来源于商品重量、尺寸、容量和其他目录属性

| 亚马逊美国商城、印度商城和日本商城： | | | | | | |
| --- | --- | --- | --- | --- | --- | --- |
| 序号 | 商品类型 | 目录属性 | 计量单位 | 规格显示格式/（规格值示例） | | |
| 美国 | 日本 | 印度 | | | | |
| 1 | PROJECTILE_BOW | 弓箭拉力 | 磅 | X 磅（10 磅） | X 磅 | X 磅（10 磅） |
| 2 | ICE_CHEST | 容量 | 夸脱或升 | X 夸脱（10 夸脱） | X 升 | X 升（10 升） |
| 3 | KETTLEBELL | 商品重量 | 磅或千克 | X 磅（10 磅） | X 千克（10 千克） | X 千克（10 千克） |
| 4 | FISHING_LINE | 商品尺寸 | 码或米 | X 码（22 码） | X 米 | X 米（10 米） |
| 断裂强度 | 磅 | X 磅（10 磅） | Y 磅 | Y 磅（12 磅） | | |
| 5 | BEER | 单位计数 | - | XX 个（YY 件）/2 个（10 件） | XX 个（x YY 件） | 不适用于印度 |
| number_of_items | - | | | | | |
| 6 | RESPIRATOR | 单位计数 | - | XX 个（YY 件）/2 个（10 件） | XX 个（x YY 件） | XX 个（YY 件）/2 个（10 件） |
| number_of_items | - | | | | | |
| 7 | PET_BED_MAT | 商品长度、宽度和厚度 | 英寸/厘米 | 长 x 宽 x 高（英寸）（12 x 10 x 15 英寸） | 长 x 宽 x 高（厘米）（12 x 10 x 15 厘米） | 长 x 宽 x 高（厘米）（12 x 10 x 15 厘米） |
| 8 | ANIMAL_CARRIER | 商品长度、宽度和高度 | 英寸/厘米 | 长 x 宽 x 高（英寸）（12 x 10 x 15 英寸） | 长 x 宽 x 高（厘米）（12 x 10 x 15 厘米） | 长 x 宽 x 高（厘米）（12 x 10 x 15 厘米） |
| 9 | ANIMAL_CAGE | 商品长度、宽度和高度 | 英寸/厘米 | 长 x 宽 x 高（英寸）（12 x 10 x 15 英寸） | 长 x 宽 x 高（厘米）（12 x 10 x 15 厘米） | 长 x 宽 x 高（厘米）（12 x 10 x 15 厘米） |
| 10 | CURTAIN | 商品长度和宽度 | 英寸/厘米 | 长（英寸）x 宽（英寸）（YY 件）/ 10 英寸 x 12 英寸（2 件） | 长（x 厘米）x 宽（y 厘米）（x YY 件）/长 10 厘米 x 宽 12 厘米（2 件） | 长门 - 9 英尺 x 4 英尺（2 件） |
| number_of_items | | | | | | |
| 11 | WALL_ART | 商品长度和宽度 | 英寸/厘米 | 长 x 宽（英寸）（10 x 12 英寸） | 宽（x 厘米）x 高（y 厘米）（即：宽 10 厘米 x 高 12 厘米） | 宽 x 高（英寸）（12 x 10 英寸） |
| 12 | TOWEL | 商品长度和宽度 | 英寸/厘米 | 长 x 宽（英寸）（10 x 12 英寸） | 长（x 厘米）x 宽（y 厘米）（即：长 10 厘米 x 宽 12 厘米） | 长 x 宽（厘米）（10 x 12 厘米） |
| 13 | CABINET | 商品深度、宽度和高度 | 英寸/厘米 | 长 x 宽 x 高（英寸）（10 x 12 x 15 英寸） | 长（x 厘米）x 宽（y 厘米）x 高（z 厘米）（即：长 10 厘米 x 宽 12 厘米 x 高 15 厘米） | 长 x 宽 x 高（厘米）（12 x 10 x 15 厘米） |
| 14 | SHELF | 商品深度、宽度和高度 | 英寸/厘米 | 深（x 英寸）x 宽（y 英寸）x 高（z 英寸）（即：深 10 英寸 x 宽 12 英寸 x 高 15 英寸） | 长（x 厘米）x 宽（y 厘米）x 高（z 厘米）（即：长 10 厘米 x 宽 12 厘米 x 高 15 厘米） | 长 x 宽 x 高（厘米）（12 x 10 x 15 厘米） |

| Q3 2024 | | | | | | |
| --- | --- | --- | --- | --- | --- | --- |
| 序号 | 商品类型 | 属性 | 美国 | 印度 | 加拿大 | 日本 |
| 1 | PITCHER | capacity | 10.5 盎司 | 1.5 升 | 45 盎司 | 1.5 升 |
| 2 | THERMOS | capacity | 10.5 盎司 | 200.0 毫升 | 10.2 盎司 | 120 毫升 |
| 3 | SPRAY_BOTTLE | capacity | 10.5 盎司 | 20.4 毫升 | 10.5 盎司 | 250 毫升 |
| 4 | SLOW_COOKER | capacity | 10.5 夸脱 | 4.5 升 | 10.5 夸脱 | 3.5 升 |
| 5 | STOVETOP_KETTLE | capacity | 10.5 盎司 | 1.9 升 | 2.6 夸脱 | 2.1 升 |
| 6 | PRESSURE_COOKER | capacity | 10.1 夸脱 | 10.5 升 | 2.6 夸脱 | 120 升 |
| 7 | BOTTLE | capacity | 10.5 盎司 | 20 毫升/1 升 | 45 盎司 | 250 毫升 |
| 8 | ELECTRIC_WATER_BOILER | capacity | 10.5 夸脱 | 10.5 升 | 10.5 夸脱 | 10.5 升 |
| 9 | KITCHEN_KNIFE | blade.length | 6.6 英寸 | 15.5 厘米 | 6 英寸 | 180 毫米 |
| 10 | KNIFE | blade.length | 6.6 英寸 | 15.5 厘米 | 6 英寸 | 180 毫米 |
| 11 | DISH_DRYING_MAT | item_length_width | 30.5 x 15.5 英寸 | 31.5 x 15.5 厘米 | 48.5（长）x 30.5（宽）厘米 | 31.5 x 15.5 厘米 |
| 12 | BINOCULAR | magnification_maximum | 10 x 42 | 8 x 50 | 8 x 50 | 8 x 50 |
| objective_lens.diameter | | | | | | |
| 13 | DESK_PAD | item_length_width | 31.5 x 15.7 英寸 | 31.5 x 15.7 厘米 | 39.9（长）x 80.5（宽）厘米 | 60.8 x 35.7 厘米 |
| 14 | WALLPAPER | item_length_width | 10 x 12 英寸 | 45.6 x 600.8 厘米 | 45（宽）x 299（长）厘米 | 90.3（宽）x 2.5（长）米 |
| 15 | LIQUID_INK | item_volume | 3.5 液盎司 | 100 毫升 | 50 毫升 | 15 毫升 |
| 16 | WINDOW_SHADE | item_length_width | 42（宽）x 72（高）英寸 | 2 英尺 7 英寸 x 1 英尺 11 英寸（宽 x 高） | 56（宽）x 150（高）厘米 | 100（长）x 178（宽）厘米 |
| 17 | GOLF_PRACTICE_MAT | item_length_width_thickness | 10 英尺 5 英寸 x 5 英尺 5 英寸（长 x 宽） | 10 英尺 5 英寸（长）x 5 英尺 6 英寸（宽） | 10 英尺 5 英寸 x 5 英尺 5 英寸（长 x 宽） | 30（长）x 14.5（宽）厘米 |
| 18 | GRIDDLE_PLATE | item_length_width_thickness | 14.0 x 31.0 x 3.0 英寸 | ‎33.0 x 33.5 x 4.2 厘米 | 50.8（长）x 26.4（宽）x 2.5（高）厘米 | 33（长）x 33（宽）x 5（厚）厘米 |
| 19 | TAPE_MEASURE | blade.length | 6 米 | 5 米 | 12 英尺 3 英寸 | 5.5 米（长） |
| 20 | COOKING_POT | capacity | 10.5 夸脱 | 6. 0 升，26.0 厘米 | 10.5 夸脱 | 10.5 升，直径 23.3 厘米 |
| item_diameter | | | | | | |
| 21 | 搁脚凳 | item_depth_width_height | 13（长） x 17（宽） x 13（高）英寸 | 20（长）x 15（宽）x 14（高）厘米 | 37.5（长）x 37.5（宽）x 45（高）厘米 | 20（长）× 15（宽）× 14（高）厘米 |
| 22 | FURNITURE_LINER | item_length_width | 30.5（宽）x 15.5（长）英寸 | 5（宽）x 15.5（长）厘米（长 0.2 米） | 6（宽）x 200（长）厘米 | 5（长）× 0.4（宽）米 |
| 23 | SELF_STICK_NOTE | item_dimensions | 3.1 x 3.5 英寸 | 15 x 76 毫米 | 3.1 x 3.5 英寸 | 76 x 76 毫米 |
| 24 | WALL_ART | item_length_width | 10.0（长）x 12.5（宽）英寸 | 22.3（长）x 17.8（宽）厘米 | 50（长）x 100（宽）厘米 | 100.3（长）x 40.7（宽）厘米 |
| 25 | BATHTUB_SHOWER_MAT | item_length_width | 27 英寸（圆形） | 250 厘米（圆形） | 250 厘米（圆形） | 300 厘米（圆形） |
| item_shape | 39 x 16 英寸（方形） | 45 x 45 厘米（正方形） | 45 x 45 厘米（正方形） | 50（长）x 70（宽）厘米（椭圆形） | | |
| 26 | POOL_COVER | item_length_width | 5 英尺 3 英寸 （圆形） | 4 米（圆形） | 5 英尺 3 英寸 （圆形） | 300 厘米（圆形） |
| item_shape | 6 英尺 7 英寸 x 9 英尺 1 英寸（方形） | 3 米 x 3 米（矩形） | 6 英尺 7 英寸 x 9 英尺 1 英寸（方形） | 570 × 250 厘米（矩形） | | |
| 27 | RUG | item_length_width | 5 英尺 3 英寸 （圆形） | 5 英尺 3 英寸 （圆形） | 5 英尺 3 英寸 （圆形） | 300 厘米（圆形） |
| item_shape | 9 英尺 1 英寸 x 6 英尺 7 英寸（方形） | 3 英尺 5 英寸 x 4 英尺 7 英寸（矩形） | 6 英尺 7 英寸 x 9 英尺 1 英寸（方形） | 200 × 250 厘米（矩形） | | |
| 28 | RUG_PAD | item_length_width | 5 英尺 3 英寸 （圆形） | 5 英尺 3 英寸 （圆形） | 5 英尺 3 英寸 （圆形） | 300 厘米（圆形） |
| item_shape | 9 英尺 1 英寸 x 6 英尺 7 英寸（方形） | 3 英尺 5 英寸 x 4 英尺 7 英寸（矩形） | 6 英尺 7 英寸 x 9 英尺 1 英寸（方形） | 200 × 250 厘米（矩形） | | |
| 29 | CLOTH_NAPKIN | item_length_width | 12 x 11 英寸（2 件装） | 45 x 45 厘米（4 件装） | 45（长）x 45（宽）厘米（2 件装） | 43 × 43 厘米（2 件装） |
| 30 | CURTAIN | item_length_width | 22.5（宽）x 36.5（长）英寸（2 件装） | | 52.5（宽）x 108.5（长）英寸（2 片装） | 135.5（宽） x 100.5 厘米（2 件装） |
| number_of_items | | | | | | |
| 31 | DECORATIVE_PILLOW_COVER | item_length_width | 10.5 x 12.2 英寸（2 件装） | 16 x 16 英寸（5 件装） | 45.7（长）x 45.7（宽）厘米（2 件装） | 60 × 60 厘米（2 件装） |
| number_of_items | | | | | | |
| 32 | ANTI_FATIGUE_FLOOR_MAT | item_length_width_thickness | 32（长）x 20（宽）x 0.75（厚）英寸 | 100（长）x 62.5（宽）x 1.0（厚）厘米 | 32（长）x 20（宽）x 0.75（厚）英寸 | 30（长）× 30（宽）× 1.2（厚）厘米 |
| 33 | HVAC_AIR_FILTER | item_length_width_thickness | 19.5 x 24.5 x 0.75 英寸 | 11.8（长）x 11.8（宽）x 2（高）厘米 | 19.5 x 24.5 x 0.75 英寸 | 13（长）x 24（宽）x 0.5（厚）厘米 |
| 34 | CALENDAR | item_width_height | 11.4（宽）x 7.5（高）英寸 | 11.4（宽）x 7.5（高）英寸 | 27.9（宽）x 43.2（高）厘米 | 22.8（宽）x 25.6（长）厘米 |
| 35 | CRIB | item_length_width_height | 54.25（长）x 29.5（宽）x 35（高）英寸 | 41.3（长）x 24.8（宽）x 21.5（高）英寸 | 135.5（长）x 74.3（宽）x 99（高）厘米 | 90（长）x 53（宽）x 17（高）厘米 |
| 36 | CYCLING_TIRE_TUBE | item_diameter | 27 英寸 x 2 英寸 - 2.5英寸 | 27 英寸 x 2 英寸 - 2.5英寸 | 27 英寸 x 2 英寸 - 2.5英寸 | 700 × 31 ~ 34 毫米 |
| compatible_tire_width_minimum | | | | | | |
| compatible_tire_width_maximum | | | | | | |
| 37 | DRESSER | item_depth_width_height | 13（长）x 17（宽）x 13（高）英寸（2 个抽屉） | 24（长）x 15（宽）x 14（高）厘米（2 个抽屉） | 37.5（长）x 37.5（宽）x 45（高）厘米（2 个抽屉） | 64（长）× 36（宽）× 76（高）厘米（抽屉数量： 2） |
| number_of_drawers | | | | | | |
| 38 | IRONING_BOARD | working_surface_length_width | 47.5（长）x 15（宽）英寸 | 47（长）x 15（宽）英寸 | 47（长）x 15（宽）英寸 | 110（长）x 30（宽）厘米 |
| 39 | CUTTING_BOARD | item_length_width_thickness | 18.5（长）x 11.5（宽）英寸 | 31.5（长）x 15.7（宽）厘米 | 18.5（长）x 11.5（宽）英寸 | 31.5（长）× 15.7（宽）厘米 |
| 40 | PET_PLACEMAT | item_length_width | 18.5（长）x 11.5（宽）英寸 | 18.5（长）x 11.5（宽）英寸 | 18.5（长）x 11.5（宽）英寸 | 31.5（长）× 15.7（宽）厘米 |
| 41 | TRAY | item_length_width_height | 7.3 x 12 x 2.2 英寸 | 13 x 6.5 x 5 英寸 | 13 x 6.5 x 5 英寸 | 90（长）x 53（宽）x 17（高）厘米 |
| item_shape | 7.3 英寸 | 4.5 英寸 | 7.3 英寸 | 20.2 厘米（长度） | | |
| 42 | JAR | capacity | 10.5 盎司 | 10 毫升 | 10 毫升 | 120 毫升 |
| 43 | WRITING_BOARD | item_width_height | 36（宽）x 24（高）英寸 | 2 x 3 英尺 | 36（宽）x 24（高）英寸 | 22（宽）x 25（高）厘米 |
| 44 | BAKING_MAT | item_length_width | 11.5（长）x 9.5（宽）英寸 | 78.5（长）x 52.5（宽）厘米 | 11.5（长）x 9.5（宽）英寸 | 31.5（长）× 15.7（宽）厘米 |
| 45 | MOUSE_PAD | item_length_width | 9.4（长）x 8.1（宽）英寸 | 31.5（长）x 15.7（宽）厘米 | 9.4（长）x 8.1（宽）英寸 | 360（长）x 275（宽）毫米 |
| 46 | PINBOARD | item_length_width | 30 x 15.5 英寸 | 1.5 x 2 英尺 | 20 x 30.1 英寸 | 30（长）x 40（宽）厘米 |
| 47 | HOME_MIRROR | item_length_width | 11.5（长）x 9.5（宽）英寸 | 11.5（长）x 9.5（宽）英寸 | 11.5（长）x 9.5（宽）英寸 | 31.5（长）× 15.7（宽）厘米 |
| 48 | TREE_SKIRT | item_diameter | 36 英寸 | 60 英寸 | 60 英寸 | 78 厘米 |
| 49 | ARTIFICIAL_TREE | item_depth_width_height.height | 6 英尺 5 英寸 | 6 英尺 5 英寸 | 6 英尺 5 英寸 | 78 厘米 |

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GZJRCRLWW7WKKDAH
