### {ms:} 说明

| 名称                    | 说明                                                         |
| :---------------------- | ------------------------------------------------------------ |
| {ms:global.host/}       | 项目域名地址 http://localhost:15424/ms-mcms                  |
| {ms:global.style/}      | 返回当前站点的模板名称  templets/1/company1804               |
| {ms:global.name/}       | 网站title 数据库表app 的app_id =1 的 app_name                |
| {ms:global.url/}        | 返回域名+静态文件                                            |
| {ms:arclist typeid=193} | arclist -> 对应文章表 cms_content;</br>typeid=193 -> 对应 cms_content.content_category_id |
|                         |                                                              |

### field 说明


| 名称             | 说明                                                         |
| ---------------- | ------------------------------------------------------------ |
| [field.litpic/]  | 文章缩略图 -> 对应 数据库表cms_content.content_img.path ; content_img 是json对象字符串 |
| [field.content/] | 文章内容 -> 对应表cms_content.content_details                |
| field.title      | 文章标题 -> 对应表 cms_content.content_title                 |
|                  |                                                              |
|                  |                                                              |



### 模板说明


| 模板          | 说明                                                         |
| ------------- | ------------------------------------------------------------ |
| gdt.htm       | 下方滚动图片 模板                                            |
| case-list.htm | 二级页面模板 , 生成二级页面 点 生成栏目 下拉框一般选顶级栏目 |
| new-show.htm  | 三级页面模板                                                 |
|               |                                                              |



### 数据库表说明

| 表           | 说明               |
| ------------ | ------------------ |
| cms_category | 栏目表             |
| cms_content  | 栏目内容表, 文章表 |





### 其他: 

- HF2的图片 来自 文章管理 -> 首页幻灯 -> 短图

- 生成文章的意思是 生成文章页面 用到的模板是new-show.htm 是三级页面 具体内容对应的是 表cms_content.content_details

- 搜索 对应的是 cms_content.content_keyword