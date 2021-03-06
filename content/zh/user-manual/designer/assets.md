---
title: 资源
template: usermanual-page.tmpl.html
position: 6
---

资源面板管理了所有的项目中的可用资源。从这个面板可以创建，上传，删除，查看和编辑任何资源。

![Assets Panel][1]

## 层级文件夹

文件夹面板帮助你以文件夹树的形式管理所有资源。

点击 Add Asset (+) 按钮然后选择 'Folder' 创建一个新文件夹。另外，右键点击想创建文件夹的目的地，然后选择 ‘New Asset' >  'Folder’ 也是一样的效果。

双击文件夹可以在检查器中的名称栏位中修改文件夹的名字。

在层级菜单中双击文件夹然后点击删除可以删除一个文件夹。同样也可以右键点击想删除的文件夹，然后在上下文菜单中选择 'Delete'。

文件夹可以互相拖拽，可以使用这种方式重新组织目录结构。

## 创建和上传资源

可以通过拖放本地文件到资源面板来完成新的资源创建。编辑器会自动上传和转换文件为可用资源。

一些特定的资源类型可以在 Add Asset (+) 图标中创建。

选择想要删除的资源然后点击垃圾桶按钮删除资源。

## 编辑资源

特定的基于文本的资源可以通过 PlayCanvas 的脚本编辑器来打开和编辑。譬如文本，json，shader，html，css 以及脚本资源。双击这些资源图标就可以。

## 检查资源

在资源面板中选择缩略图，检查器就会同步显示出资源的详细信息。

## 过滤

在过滤器下来菜单中筛选类型以过滤其它非相关类型的资源。

## 搜索

在搜索框中可以对工程中的资源进行全局搜索。简单的在搜索框中输入关键字，编辑器会实时进行资源搜索。

The Search box supports wildcards. For example, *. will list every asset in your project.

## 拖放

资源可以通过从主面板拖放到文件夹的树形结构来移动。资源支持多选，按 CTRL+A 可以选中当前目录下的全部资源。

还可以通过拖放把资源从资源面板链接到[检查器][2]的高亮位置上。检查器上的高亮位置通常是组件的资源属性或者是资源类型的脚本属性。

此外还可以拖动模型，材质以及 cubemap 资源直接到[视口][3] 中进行应用。

* 如果拖动模型资源到视口中，编辑器将会创建一个新的实体并添加模型组件同时将模型资源添加至模型组件引用。视口摄影机将会自动缩放至呈现新创建实体的位置。
* 如果拖动材质至视口中的模型实体上时，材质将会实时替换掉模型上的材质 (用于预览)。如果确定需要替换材质，则松开鼠标完成拖放即可。
* 如果拖放 Cubemap 到视口中的场景背景上，Cubemap 会被做为场景的天空盒使用。在[场景设置][4]中也有对应的参数可以修改。

## Checking References

Sometimes it's useful to know where assets are being used (or referenced) within a particular scene. If the Editor cannot detect any references for an asset, a small dot will be displayed on its thumbnail:

![Unreferenced Asset][5]

<div class="alert alert-info">
Note that the Editor cannot detect references to assets that are made in code. So think carefully before you delete an asset based on this indicator!
</div>

If an asset does have references, you can check them via the References content menu item:

![Asset References][6]

Selecting a reference will load it into the Inspector panel.

[1]: /images/user-manual/editor/assets-panel.png
[2]: /user-manual/designer/inspector
[3]: /user-manual/designer/viewport
[4]: /user-manual/designer/settings
[5]: /images/user-manual/editor/assets-panel/unreferenced-asset.png
[6]: /images/user-manual/editor/assets-panel/asset-references.png

