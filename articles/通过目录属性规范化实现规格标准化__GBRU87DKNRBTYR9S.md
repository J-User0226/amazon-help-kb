---
title: "通过目录属性规范化实现规格标准化"
doc_id: GBRU87DKNRBTYR9S
source: https://sellercentral.amazon.com/help/hub/reference/external/GBRU87DKNRBTYR9S
language: zh-CN
fetched_at: 2026-10-30T14:24:39
---

# 通过目录属性规范化实现规格标准化

亚马逊对卖家输入的“规格”进行了标准化处理，以便买家对于规格信息有更一致的体验，并移除重复项。您提供的包含规格的信息不可见，但来源于其他目录属性，如商品重量、尺寸（例如商品长度、宽度和高度）、容量、单位计数、商品数量、净含量重量、净含量体积和净含量计数。请参阅下面的表 1 和表 2，查看所有目录属性和商品类型详情列表。

请务必遵循指定的指南显示规格信息，因为买家有权获知购买后收到商品的规格。规格信息不清晰会导致买家产生困惑。

提供准确的规格信息和清晰的商品详情页面有助于建立买家信心并提高销量。亚马逊致力于通过创建标准化和一致的格式机制显示规格详情，帮助您达到此数据质量标准。如果用于生成规格的目录属性未填充，则规格未标准化。

根据买家的地理位置，“规格”值将显示他们熟悉的规格格式。例如，对于美国买家，将以盎司或磅为单位显示重量信息；而对于欧洲买家，将以克或千克为单位显示重量信息。

## 数量属性的标准化规则

标准化规则会在可能的情况下自动重新调整“规格”值的格式。为了方便供应商操作，我们对不符合我们格式标准的任何规格属性的数量信息应用标准化规则。为此，我们会为买家删除模糊不清的详情并移除重复项。例如，如果您之前向亚马逊美国商城提交的值为“32 个”或“32 个（1 件）”，则系统会自动将其转换为“32 个（1 件装）”。有关更多信息，请参阅**表 1： 特定于数量的商品类型目录属性列表**。

**注意： ****表 2 中也没有列出具有数量属性的商品类型： 商品类型目录属性列表，包括商品重量、尺寸、容量和其他属性**。

如果两位卖家发布的商品具有相同的数量包装，但各自提供的“规格”值却不同（一位卖家提供的值为“32 个”，另一位卖家提供的值为“32 个 [1 件]”），则亚马逊“规格”标准化逻辑将根据 unit_count / number_of_items + unit_count.type + (“pack of” + number_of_items) 这一公式来识别有关信息。

如果单位计数为 32 个，商品数量为 1，则亚马逊得出的“规格”值为“32 个（1 件装）”。这样一来，买家只能看到一个版本的“规格”，且这两位卖家的报价都将关联到同一商品。

创建商品信息的过程没有变化。但是，请务必为下列属性添加正确信息：

- 单位计数

- 商品数量

- 净含量（重量、体积、数量和面积）

- 纸尿裤规格

- 每个容器内的总量

## 适用于数量之外的目录属性的标准化规则

此外，还针对尺寸、容量和商品重量等属性实施标准化规则。根据用于计算特定商品类型的规格的目录属性，该商品的规格将相应更新。

**商品重量：** 对于其规格来源于商品重量的商品类型，规格值可通过将商品重量信息转换为特定于商城的标准单位格式进行填充。例如，在美国，如果壶铃 ASIN 的商品重量填写为 10 千克，则该商品的规格将填充为 22.04 磅，因为磅是美国的标准重量单位。

此外，如果商品重量填写为 22.04 磅，则标准化规则标准化此商品，将规格值设为 22.04 磅。

**尺寸：** 规范化规则会根据特定于商城标准单位，将目录属性中填写的值（例如长、宽、高、深）转换成为商品类型定义的标准显示格式。例如，在美国，如果货架的 item_depth_width_height（深、宽和高）分别填写 30 厘米、15 厘米和 20 厘米，则规格将显示为深 12 英寸 x 宽 6 英寸 x 高 8 英寸。同样，对于动物笼子，item_depth_width_height 规格显示为 12 英寸 x 6 英寸 x 8 英寸。

**容量：** 标准化规则会将填入的容量值转换为标准显示格式，并使用特定于商城的标准单位。例如，如果冷藏箱商品类型的容量属性填写 1 升，则标准化规则将显示规格为 1.06 夸脱，因为夸脱是美国的标准体积单位。

**注意： **请参阅【包含的商品类型】部分，了解完整的商品类型列表以及相应的目录属性和尺寸显示格式。

所有新创建的 ASIN 商品信息和对现有 ASIN 的更新都必须具有必填属性，才能显示“规格”值。在“规格”中输入的值不会显示在商品详情页面上。

亚马逊会自动合并目录属性的值以填充“规格”属性。目录属性是针对每个商品类型定义的。变体主题的值不会发生变化。如果现有 ASIN 的“规格”值是有效值，则无需重新提交“规格”值。

如果选项中没有您的商品规格，它也不属于附加属性，请确认您已为生成规格定义的属性选择了准确值，因为这些值将决定后续属性下的可用值。如果您认为自己确实遇到了选项中没有您商品规格的情况，您可以联系销售伙伴支持，亚马逊将审核您的请求。

**注意： **亚马逊的卖家助手可以通过此主题提供帮助。对于大多数语言设置，卖家助手还可以直接将您转接至销售伙伴支持。

## 要更新您的规格属性，请执行以下操作：

**单个 ASIN 属性更新：**

- 前往 [管理所有库存](https://sellercentral.amazon.com/gp/help/help.html?itemID=/myinventory/inventory)

- 搜索 ASIN 并点击 【编辑】。

**注意： **这将打开一个新选项卡。

- 在【商品详情】部分，填写特定商品类型规格的目录属性，如 **item _weight**、**item_length_width_height**、**item_length_width_thickness**、**item_length_width**、**unit_count**、**unit_count_type** 以及 **number_of_items**（请参阅**包含的商品类型**，了解商品类型、属性和规格格式的更多信息）。

- 点击 **保存**。

**属性更新的批量上传流程：**

- 前往[添加商品](https://sellercentral.amazon.com/gp/help/help.html?itemID=/product-search)

- 选择【下载电子表格】选项卡，然后点击【更新商品详情】部分下的【获取商品模板】。

- 在弹出窗口中，选择【商品模板】，然后在下一个窗口中，选择【电子表格语言】下的电子表格语言。选择要更新的商品的商品类型。点击【生成模板】，下载特定分类的模板，并填写 SKU、Brand、Update Delete 以及其他列的信息。

- 以制表符分隔文本格式保存文件。

- 前往 [添加商品](https://sellercentral.amazon.com/gp/help/help.html?itemID=/product-search)，然后在 【上传电子表格】 选项卡中上传您的库存文件。

## 包含的商品类型

以下商品类型中的所有 SKU 和 ASIN 必须使用必填属性进行更新。您将在常规目录编辑期间收到通知，添加缺少的商品形态和商品数量（例如商品重量、商品长度、商品宽度、商品高度、容量、单位计数、商品净含量、纸尿裤规格以及每个容器的总量）。

标准化规则适用于以下商品类型的消费类商品和硬百货商品：

| 表 1： 特定于数量的商品类型目录属性列表 | |
| --- | --- |
| 商品类型 | 规格值依据的属性 |
| Area deodorizer | 单位计数和商品数量 |
| Astringent substance | 单位计数和商品数量 |
| Baby bottle | 单位计数和商品数量 |
| Baby formula | 单位计数和商品数量 |
| Baking mix | 单位计数和商品数量 |
| Bathing sponge | 单位计数和商品数量 |
| Bathwater additive | 单位计数和商品数量 |
| Bleach | 单位计数和商品数量 |
| Body deodorant | 单位计数和商品数量 |
| Body lubricant | 单位计数和商品数量 |
| Bottle nipple | 单位计数和商品数量 |
| Breakfast cereal | 单位计数和商品数量 |
| Cake | 单位计数和商品数量 |
| Chewing gum | 单位计数和商品数量 |
| Cleaning agent | 单位计数和商品数量 |
| Coffee | 单位计数和商品数量 |
| Conditioner | 单位计数和商品数量 |
| Condom | 单位计数和商品数量 |
| Contact lenses | 单位计数和商品数量 |
| Cosmetic powder | 单位计数和商品数量 |
| Cosmetic sponge | 单位计数和商品数量 |
| Cracker | 单位计数和商品数量 |
| Culinary salt | 单位计数和商品数量 |
| Dairy based drink | 单位计数和商品数量 |
| Dental floss | 单位计数和商品数量 |
| Dishwasher detergent | 单位计数和商品数量 |
| Dry shampoo | 单位计数和商品数量 |
| Earplug | 单位计数、商品数量和净含量 |
| Edible oil animal | 单位计数和商品数量 |
| Essential oil | 单位计数和商品数量 |
| Eyebrow color | 单位计数和商品数量 |
| Eyelid color | 单位计数和商品数量 |
| Fabric softener | 单位计数和商品数量 |
| Face shaping makeup | 单位计数和商品数量 |
| Facial tissue | 单位计数和商品数量 |
| False eyelash | 单位计数、商品数量和净含量 |
| False nail | 单位计数和商品数量 |
| Flavored drink concentrate | 单位计数和商品数量 |
| Flour | 单位计数和商品数量 |
| Food coloring | 单位计数和商品数量 |
| Foot scraper | 单位计数和商品数量 |
| Gift wrap | 单位计数、商品数量和净含量 |
| Hair cleaner conditioner | 单位计数和商品数量 |
| Hair clip | 单位计数和商品数量 |
| Hair coloring agent | 单位计数和商品数量 |
| Hair removal agent | 单位计数和商品数量 |
| Hair roller | 单位计数和商品数量 |
| Hair styling agent | 单位计数和商品数量 |
| Hair tie | 单位计数和商品数量 |
| Hairband | 单位计数和商品数量 |
| Hand sanitizer | 单位计数和商品数量 |
| Herbal supplement | 单位计数和商品数量 |
| Honey | 单位计数和商品数量 |
| Incontinence protector | 单位计数、商品数量和纸尿裤规格 |
| Insect repellent | 单位计数和商品数量 |
| Jerky | 单位计数和商品数量 |
| Juice and juice drink | 单位计数和商品数量 |
| Laundry detergent | 单位计数和商品数量 |
| Leavening agent | 单位计数和商品数量 |
| Legume | 单位计数和商品数量 |
| Lip balm | 单位计数、商品数量和净含量 |
| Lip color | 单位计数和商品数量 |
| Makeup primer | 单位计数和商品数量 |
| Manual shaving razor | 单位计数和商品数量 |
| Mascara | 单位计数和商品数量 |
| Meal replacement beverage | 单位计数和商品数量 |
| Medical test strip | 单位计数和商品数量 |
| Medication | 单位计数和商品数量 |
| Menstrual cup | 单位计数和商品数量 |
| Milk substitute | 单位计数和商品数量 |
| Mineral supplement | 单位计数和商品数量 |
| Mouthwash | 单位计数和商品数量 |
| Nail polish | 单位计数和商品数量 |
| Nail polish remover | 单位计数和商品数量 |
| Nail treatment | 单位计数和商品数量 |
| Non-dairy cream | 单位计数和商品数量 |
| Noodle | 单位计数和商品数量 |
| Nut butter | 单位计数和商品数量 |
| Nutritional supplement | 单位计数、商品数量和每个容器内的总食用分量 |
| Packaged soup and stew | 单位计数和商品数量 |
| Paint | 单位计数和商品数量 |
| Paper towel | 单位计数、商品数量和净含量 |
| Pastry | 单位计数和商品数量 |
| Personal fragrance | 单位计数和商品数量 |
| Pet food | 单位计数和商品数量 |
| Popcorn | 单位计数和商品数量 |
| Pretzel | 单位计数和商品数量 |
| Protein drink | 单位计数和商品数量 |
| Protein supplement powder | 单位计数和商品数量 |
| Puffed snack | 单位计数和商品数量 |
| Razor blade cartridge | 单位计数和商品数量 |
| Rice mix | 单位计数和商品数量 |
| Safety mask | 单位计数和商品数量 |
| Sanitary napkin | 单位计数和商品数量 |
| Seafood | 单位计数和商品数量 |
| Seasoning | 单位计数和商品数量 |
| Self tanner | 单位计数和商品数量 |
| Shampoo | 单位计数和商品数量 |
| Shaving agent | 单位计数和商品数量 |
| Shellfish | 单位计数和商品数量 |
| Skin blemish removal tool | 单位计数和商品数量 |
| Skin cleaning agent | 单位计数和商品数量 |
| Skin cleaning wipe | 单位计数和商品数量 |
| Skin exfoliant | 单位计数和商品数量 |
| Skin foundation concealer | 单位计数和商品数量 |
| Skin moisturizer | 单位计数和商品数量 |
| Skin serum | 单位计数和商品数量 |
| Skin treatment mask | 单位计数和商品数量 |
| Sleep mask | 单位计数和商品数量 |
| Snack chip and crisp | 单位计数和商品数量 |
| Snack food bar | 单位计数、商品数量和净含量 |
| Snack mix | 单位计数和商品数量 |
| Sugar | 单位计数和商品数量 |
| Sugar substitute | 单位计数和商品数量 |
| Sunscreen | 单位计数和商品数量 |
| Surface cleaning wipe | 单位计数和商品数量 |
| Surface protection wax | 单位计数和商品数量 |
| Syrup | 单位计数和商品数量 |
| Textile deodorizer | 单位计数和商品数量 |
| Thickening agent | 单位计数和商品数量 |
| Toilet paper | 单位计数、商品数量和净含量 |
| Tooth cleaning agent | 单位计数和商品数量 |
| Tooth whitener | 单位计数和商品数量 |
| Toothbrush | 单位计数和商品数量 |
| Toothbrush head | 单位计数和商品数量 |
| Topical hair regrowth treatment | 单位计数和商品数量 |
| Vinegar | 单位计数和商品数量 |
| Vitamin | 单位计数和商品数量 |
| Waste bag | 单位计数和商品数量 |
| Water | 单位计数和商品数量 |
| Writing instrument | 单位计数和商品数量 |

## 上传数据集成商

相同的标准也适用于使用上传数据发布商品信息的方法。因此，如果您使用上传数据集成工具，此工具需要符合属性发布标准。在开始执行新属性之前，亚马逊已提前大约 60 天发布了这些标准，为您留出了充足的时间来采用新标准。

**表 2： 商品类型目录属性列表，包括商品重量、尺寸、容量和其他属性**

| 亚马逊美国商城、印度商城和日本商城： | | | | | | |
| --- | --- | --- | --- | --- | --- | --- |
| 序号 | 商品类型 | 目录属性 | 计量单位 | 规格显示格式/（规格值示例） | | |
| 美国 | 日本 | 印度 | | | | |
| 1 | PROJECTILE_BOW | archery_draw_weight | Pounds/lbs | X Pounds (10 Pounds) | X lb | X lbs (10 Pounds) |
| 2 | ICE_CHEST | capacity | Quarts/liters | X Quarts (10 Quartz) | X liters | X liters (10 liters) |
| 3 | KETTLEBELL | item_weight | Pounds/kg | X 磅（10 磅） | X kgs (10 kgs) | X kg (10 kg) |
| 4 | FISHING_LINE | item_dimensions | Yards/m | X Yards (22 Yards) | X m | X m (10 m) |
| breaking_strength | Pounds/lbs | X Pounds (10 Pounds) | Y lb | Y lbs (12 lbs) | | |
| 5 | BEER | unit_count | - | XX Count (Pack of YY) / 2 Count (Pack of 10) | XX pieces (x YY pack) | 不适用于印度 |
| number_of_items | - | | | | | |
| 6 | RESPIRATOR | unit_count | - | XX Count (Pack of YY) / 2 Count (Pack of 10) | XX pieces (x YY pack) | XX Count (Pack of YY) / 2 Count (Pack of 10) |
| number_of_items | - | | | | | |
| 7 | PET_BED_MAT | item_length_width_thickness | inches/cm | L” x W” x H” (12” x 10” x 15”) | L x W x H cm (12x10x15 cm) | L x W x H cm (12 x 10 x 15 cm) |
| 8 | ANIMAL_CARRIER | item_length_width_height | inches/cm | L” x W” x H” (12” x 10” x 15”) | L x W x H cm (12 x 10 x 15 cm) | L x W x H cm (12 x 10 x 15 cm) |
| 9 | ANIMAL_CAGE | item_length_width_height | inches/cm | L” x W” x H” (12” x 10” x 15”) | L x W x H cm (12 x 10 x 15 cm) | L x W x H cm (12 x 10 x 15 cm) |
| 10 | CURTAIN | item_length_width | 英寸/厘米 | L" x W" （YY件） /22.5"W x 36.5"L （2件） | L xcm x W ycm (L 10 cm x W 12 cm) | |
| number_of_items | | | | | | |
| 11 | WALL_ART | item_length_width | inches/cm | L" x W" (10” x 12”) | W xcm x H ycm (W10 cm x H12 cm) | W x H inches (12 x 10 inches) |
| 12 | TOWEL | item_length_width | inches/cm | L" x W" (10” x 12”) | L xcm x W ycm (L10 cm x W12 cm) | L x W cm (10 x 12 cm) |
| 13 | 橱柜 | item_depth_width_height | inches/cm | x" L x y" W x z" H (10”L x 12”W x 15”H) | L xcm x W ycm x H zcm (L 10cm x W 12cm x H 15cm) | L x W x H cm (12 x 10 x 15 cm) |
| 14 | SHELF | item_depth_width_height | inches/cm | x" D x y" W x z" H (10" D x 12" W x 15" H) | L xcm x W ycm x H zcm (L 10 cm x W 12 cm x H 15 cm) | L x W x H cm (12 x 10 x 15 cm) |

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

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GBRU87DKNRBTYR9S
