# spine_naming_tool 动画命名规范模板

## 0. 基础动画命名规范
格式：`[动作类型]_[状态]`
示例：
- hide
- in 
- stand_loop
- out


## 1. 高亮动画命名规范
格式：`track[轨道号]_[关键词]_[状态]_[循环状态]`
参数说明：
- `[轨道号]`：从1开始的数字，多关键词时按顺序递增
- `[关键词]`：自定义标识（如角色名、物品名）
- `[状态]`：highlight（高亮）、cancel（取消）
- `[循环状态]`：可选，loop表示循环动画

示例（单个关键词）：
关键词：apple
```
track1_apple_highlight
track1_apple_highlight_loop
track1_apple_cancel
track1_apple_cancel_loop
```

示例（多个关键词）：
关键词：apple、banna、dog
```
track1_apple_highlight
track1_apple_highlight_loop
track1_apple_cancel
track1_apple_cancel_loop

track2_banna_highlight
track2_banna_highlight_loop
track2_banna_cancel
track2_banna_cancel_loop

track3_dog_highlight
track3_dog_highlight_loop
track3_dog_cancel
track3_dog_cancel_loop
```

## 2. 场景动画命名规范
格式：`[场景关键词]_[状态]`
状态：
- in
- stand_loop
- out
- out_loop

示例：
场景关键词：school
```
school_in
school_stand_loop
school_out
school_out_loop
```

## 3. IP嘴形皮肤命名规范
格式：`[关键词]_[状态]`
状态：
- quiet
- talk

示例：
关键词：zerd、minnie、max、all
```
zerd_quiet
zerd_talk

minnie_quiet
minnie_talk

max_quiet
max_talk

all_quiet
all_talk
```

## 4. Tips动画命名规范
格式：`track[轨道号]_[关键词]_[状态]`
状态：
- in
- in_loop
- out
- out_loop

示例：
关键词：tips1、tips2
```
track1_tips1_in
track1_tips1_in_loop
track1_tips1_out
track1_tips1_out_loop

track2_tips2_in
track2_tips2_in_loop
track2_tips2_out
track2_tips2_out_loop
```

## 5. 高亮+Tips命名规范
格式：`track[轨道号]_[关键词]_[状态]_[循环状态]`
参数说明：
- `[轨道号]`：从1开始的数字，多关键词时按顺序递增
- `[关键词]`：自定义标识（如角色名、物品名）
- `[状态]`：根据关键词自动识别
  - 包含"tips"的关键词：in、in_loop、out、out_loop
  - 其他关键词：highlight、highlight_loop、cancel、cancel_loop
- `[循环状态]`：可选，loop表示循环动画

示例（单个关键词）：
关键词：apple、tips1
```
track1_apple_highlight
track1_apple_highlight_loop
track1_apple_cancel
track1_apple_cancel_loop

track2_tips1_in
track2_tips1_in_loop
track2_tips1_out
track2_tips1_out_loop
```

示例（多个关键词）：
关键词：apple、tips1、panda、tips2
```
track1_apple_highlight
track1_apple_highlight_loop
track1_apple_cancel
track1_apple_cancel_loop

track2_tips1_in
track2_tips1_in_loop
track2_tips1_out
track2_tips1_out_loop

track3_panda_highlight
track3_panda_highlight_loop
track3_panda_cancel
track3_panda_cancel_loop

track4_tips2_in
track4_tips2_in_loop
track4_tips2_out
track4_tips2_out_loop
```

## 自定义说明
你可以根据实际需求修改以上格式，添加/删除规则类别，或调整命名参数顺序。