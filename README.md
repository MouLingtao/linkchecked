##LinkChecked是什么?
一款基于jQuery开发的checkbox插件。当改变checkbox父项的选中状态的时候，自动将子项全部选择或取消选择。并且当之类选择改变的时候，也会改变父类的选择状态。


##如何使用他？
正如DEMO所示，每一个checkbox都有一个唯一的名称，该名称命名规则为“{根名称}\_{一级名称}\_{二级名称}\_{三级名称}”

然后一个 $.linkchecked('{根名称}'); 就OK啦~


##插件文档
`$.linkchecked(prefix,nameKey,parentKey);`
> prefix:名称前缀，也就是根名称。

> nameKey:将该checkbox的那个属性作为他的名称。

> parentKey:将该checkbox的那个属性作为他父级的名称。当该名称值为空的时候，自动根据名称获取其父级名称。反之使用该属性值作为父级的名称。(该功能暂时不可用)


当然，两堆checkbox的前缀相同的时候。使用如下方式初始化即可。

` $('selector').linkchecked(prefix,nameKey,parentKey);`

或者

` $.linkchecked(prefix,nameKey,parentKey,$('selector'));`