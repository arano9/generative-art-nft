### 使用说明
1. config.py用于配置素材信息
2. assets目录用于放置素材 
3. nft.py即生成工具，放好素材到assets中，直接python nft.py即可在output中看到合成图片
4. 配置详解
```python
# id 表示层数 必须按顺序,由最底层开始
# name表示该层名字，可随意命名不可重名
# directory 对应层数在assets的目录名
# required 代表是否一定需要
# rarity_weights 代表该层素材各个的比重，比如有一层特征有3个素材
#   如果require是true 则 [1,5,4] 代表各个素材比重为10% 50% 40%
#   如果require是false 则 [1,1,4,4] 代表各个素材比重为10% 40% 40%, 第一个10%代表该层特征没有的权重
CONFIG = [
    {
        'id': 1,
        'name': 'background',
        'directory': '第七层背景',
        'required': True,
        'rarity_weights': None,
    },
    {
        'id': 2,
        'name': 'body',
        'directory': '第六层身体',
        'required': True,
        'rarity_weights': None,
    },
    {
        'id': 3,
        'name': 'head',
        'directory': '第五层头部',
        'required': True,
        'rarity_weights': None,
    },
    {
        'id': 4,
        'name': 'hair',
        'directory': '第四层发型',
        'required': True,
        'rarity_weights': None,
    },
    {
        'id': 5,
        'name': 'earrings',
        'directory': '第三层耳饰',
        'required': True,
        'rarity_weights': None,
    },
    {
        'id': 6,
        'name': 'headdress',
        'directory': '第二层头饰',
        'required': True,
        'rarity_weights': None,
    },
    {
        'id': 7,
        'name': 'ornaments',
        'directory': '第一层饰品',
        'required': True,
        'rarity_weights': None,
    },
]
```
