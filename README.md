# 孙玺的通用样式库

## 安装

````
npm i sx-common-css
````

## 使用

### 样式库

#### 只引入编译后的css文件
````
@import '~sx-common-css'
````

#### 只引入编译并压缩后的css文件
````
@import '~sx-common-css/dist/common.min.css'
````


#### 只引入 scss 文件
````
@import '~sx-common-css/index.scss'
````

#### 单独引入部分文件
````
@import '~sx-common-css/style/box.scss'
@import '~sx-common-css/style/flex.scss'
@import '~sx-common-css/style/text.scss'
````

### 屏幕适配 rem
````
@import '~sx-common-css/style/viewport.scss'
````

### 覆盖样式

####样式变量
````

// 边距大小
$extraSmall: 4px;
$small: 8px;
$base: 14px;
$medium: 20px;
$large: 30px;
$extraLarge: 50px;

// 圆角大小
$radius: 5px;
$extraRadius: 16px;

// 阴影
$shadow: 0 0 2px 1px rgba(0, 0, 0, 0.05);
$extraShadow: 0 0 6px 1px rgba(0, 0, 0, 0.1);

// 颜色
$colorPrimary: #409EFF;
$colorSuccess: #67C23A;
$colorDanger: #F56C6C;
$colorWarning: #E6A23C;
$colorInfo: #909399;

// 字体大小
$fontExtraSmall: 12px;
$fontSmall: 13px;
$fontBase: 14px;
$fontMedium: 18px;
$fontLarge: 20px;
$fontExtraLarge: 24px;

````

#### 如何覆盖
````

// 示例, 修改最小字体大小

$fontExtraSmall: 10px;
@import '~sx-common-css/index.scss'

// 编译后: .f-extra-small{ font-size: 10px }

````
