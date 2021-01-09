# 数字框带加减操作
uni-app 数字框组件（number-box）

1. 支持加减、禁用
2. 支持自定义步长
3. 支持小数
4. 支持v-model



## 组件使用方式

将 **long-number-box 复制到 uni-app项目中的 **components**目录即可

```vue
<template>
	<view>
		整数 <long-num-box 
			v-model="count"
			@change="change"
		>
		</long-num-box>
		小数 <long-num-box
			v-model="count1"
			:step="0.1"
			@change="change"
		>
		</long-num-box>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				count: 0,
				count1: 0
			}
		},
		onLoad() {

		},
		methods: {
			change (val) {
				console.log(val)
			}
		}
	}
</script>

```



## 属性

| 名称     | 类型             | 默认值 | 说明                             |
| -------- | ---------------- | ------ | -------------------------------- |
| v-model  | Number           | 0      | 文本框的值                       |
| min      | [String, Number] | 0      | 最小值                           |
| max      | [String, Number] | 空     | 最大值，默认为空不限制           |
| step     | Number           | 1      | 加减步长，每次加减多少，支持小数 |
| disabled | Boolean          | false  | 是否禁用，禁用则不可进行加减操作 |

## 事件

| 名称   | 返回值 | 说明           |
| ------ | ------ | -------------- |
| change | Number | 当前文本框的值 |

## 使用示例

详细代码 [Demo](https://github.com/songhailong8174/categories)

## 插件截图

![img](https://cdn.jsdelivr.net/gh/songhailong8174/images/img/1.png)

![img](https://cdn.jsdelivr.net/gh/songhailong8174/images/img/2.png)

![img](https://cdn.jsdelivr.net/gh/songhailong8174/images/img/3.png)

PS：如有问题可联系QQ（1365763165）或者提issure，如果帮到你了还请不要吝啬给个 [Star](https://github.com/songhailong8174/categories)哈

