## Vue3 常遇到的开发问题

### `$listener` 已被弃用

```nginx
# Issuse 描述
【Vue warn】 Property "$listener" was accessed during render but is not defined on instance. 
【Vue warn】 v-on with no argument expects an object value.

# Issuse 提示
Vue3 已弃用 '$listener', 无法在 <template> 中使用 '$listener'.
v-on="$listener" 已归档在 $attrs, 所以使用 v-bind="$attrs" 即可.

# Issuse 解决
~ md:before
<CustomComponent v-on="$listener" />

~ md:after
<CustomComponent v-bind="$attrs" />

```



### CSS 样式穿透处理

```nginx
# Issues 描述
【@vue/compiler-sfc】 ::v-deep usage as a combinator has been deprecated. Use :deep(<inner-selector>) instead.

# Issues 提示
我们熟知 CSS 样式穿透的几种方式:
1. 新增 <style scoped /> 进行重定义样式,必要时可添加 !important;
2. 采用 CSS 样式穿透语法 >>>, /deep/, ::v-deep, :deep(<selector>) 进行处理.

而以上 Issues 描述,建议使用 :deep(<selector>) 这一方式进行处理.

# Issues 解决
~ md:before
.p ::v-deep .a { color: red; }

~ md:after
.p :deep(.a) { color: red; }

```





### Issues 标题

```nginx
# Issues 描述

# Issues 提示

# Issues 解决
~ md:before

~ md:after

```

