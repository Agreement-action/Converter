# 协议：转换（Converter）
将物品变成积分，于下个存档中使用

## 开发计划

- [ ] 创捷一个方块 _inputBlock_ ，名称为转换器
   - [ ] 收集外部的资源，销毁并记录为csv格式的文件或其他能记录时间和校验的持久保存的方法
      - 记录要求
        - [ ] 记录销毁时累计游戏时间
        - [ ] 记录销毁物品
        - [ ] 记录存档名称
        - [ ] 记录config文件夹和mods文件夹校验码
        - [ ] 记录存档的大小
- [ ] 编写核心逻辑
   - [ ] 使用sha256或其他方法验证config文件夹和mods文件夹做校验
   - [ ] 记录存档名称和大小与config文件夹和mods文件夹做校验码存储
   - [ ] 使用ini格式或类似其他模组的config文件允许其他的整合包创作者修改物品所对应的积分
- [ ] 添加方块的面板和制作一个专门用与查看积分的面板
   - [ ] 每5s刷新一次（提供一分钟等可选项）
   - [ ] 将近2h的游戏时长输入的物品类型产生的积分变为可跨存档的积分
   - [ ] 将该游戏存档的所有产生的积分可兑换为其他联动的模组的能量或空间等
- [ ] 添加兑换面板
   - 就上面的积分和联动兑换
- [ ] 制作一个常驻游戏屏幕的面板