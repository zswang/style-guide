#html编码规范#

版本：0.1

状态：草稿

##Doctype##

```<!DOCTYPE HTML>```

##编码(文档和文件)##

文件：UTF-8无BOM的编码格式 <br>
文档：```<meta charset="UTF-8">```
> 使用meta标签设置文档编码。因为如果不指定编码，有些浏览器依据自己的原则解析，可能出现字符乱码。

##书写格式##

+ 所有的HTML元素及其属性名称均使用小写
+ 所有的都要闭合,如```<br />```
+ 标签要合理嵌套，避免inline元素嵌套block元素
+ 标签属性值必须包含在双引号中，如 ```<input type="text" name="" id="" maxlength="20" readonly="readonly" checked="checked" disabled="disabled" />```
+ 尽量减少嵌套层次
+ 使用 *4个空格* 进行代码缩进，以保证不同编辑器格式相同(代码大小可以通过压缩手段解决)
+ 将编辑器中的换行符设置成Unix格式

##标签(语义化)##


**标签语义中英文对照表:**
<table>
    <thead>
        <tr>
            <th>标签名</th>
            <th>英文全拼</th>
            <th>中文翻译</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>a</td>
            <td>anchor</td>
            <td>锚</td>
        </tr>
        <tr>
            <td>abbr</td>
            <td>abbreviation</td>
            <td>缩写词</td>
        </tr>
        <tr class="del">
            <td>acronym</td>
            <td>acronym</td>
            <td>取首字母的缩写词</td>
        </tr>
        <tr>
            <td>address</td>
            <td>address</td>
            <td>地址</td>
        </tr>
        <tr>
            <td>b</td>
            <td>bold</td>
            <td>粗体</td>
        </tr>
        <tr class="del">
            <td>big</td>
            <td>big</td>
            <td>变大</td>
        </tr>
        <tr>
            <td>blockquote</td>
            <td>block&nbsp;quotation</td>
            <td>区块引用于</td>
        </tr>
        <tr>
            <td>br</td>
            <td>break</td>
            <td>换行</td>
        </tr>
        <tr class="del">
            <td>caption</td>
            <td>caption</td>
            <td>标题</td>
        </tr>
        <tr class="del">
            <td>center</td>
            <td>center</td>
            <td>居中</td>
        </tr>
        <tr>
            <td>dd</td>
            <td>definition&nbsp;description</td>
            <td>定义描述</td>
        </tr>
        <tr>
            <td>del</td>
            <td>delete</td>
            <td>删除</td>
        </tr>
        <tr>
            <td>div</td>
            <td>division</td>
            <td>分隔</td>
        </tr>
        <tr>
            <td>dl</td>
            <td>definition&nbsp;list</td>
            <td>定义列表</td>
        </tr>
        <tr>
            <td>dt</td>
            <td>definition&nbsp;term</td>
            <td>定义术语</td>
        </tr>
        <tr>
            <td>em</td>
            <td>emphasized</td>
            <td>加重</td>
        </tr>
        <tr>
            <td>fieldset</td>
            <td>fieldset</td>
            <td>域集</td>
        </tr>
        <tr>
            <td>font</td>
            <td>font</td>
            <td>字体</td>
        </tr>
        <tr>
            <td>h1~h6</td>
            <td>header1~header6</td>
            <td>标题1~标题6</td>
        </tr>
        <tr>
            <td>hr</td>
            <td>horizontal&nbsp;rule</td>
            <td>水平尺</td>
        </tr>
        <tr>
            <td>i</td>
            <td>italic</td>
            <td>斜体</td>
        </tr>
        <tr>
            <td>ins</td>
            <td>inserted</td>
            <td>插入</td>
        </tr>
        <tr>
            <td>legend</td>
            <td>legend</td>
            <td>图标</td>
        </tr>
        <tr>
            <td>li</td>
            <td>list&nbsp;item</td>
            <td>列表项目</td>
        </tr>
        <tr>
            <td>ol</td>
            <td>ordered&nbsp;list</td>
            <td>排序列表</td>
        </tr>
        <tr>
            <td>p</td>
            <td>paragraph</td>
            <td>段落</td>
        </tr>
        <tr>
            <td>pre</td>
            <td>preformatted</td>
            <td>预定义格式</td>
        </tr>
        <tr class="del">
            <td>s</td>
            <td>strikethrough</td>
            <td id="">删除线</td>
        </tr>
            <tr class="del">
            <td>small</td>
            <td>small</td>
            <td id="">变小</td>
        </tr>
        <tr>
            <td>span</td>
            <td>span</td>
            <td>范围</td>
        </tr>
        <tr>
            <td>strong</td>
            <td>strong</td>
            <td>加重</td>
        </tr>
        <tr>
            <td>sub</td>
            <td>subscripted</td>
            <td>下表</td>
        </tr>
        <tr>
            <td>sup</td>
            <td>superscripted</td>
            <td id="">上标</td>
        </tr>
        <tr class="del">
            <td>u</td>
            <td>underlined</td>
            <td>下划线</td>
        </tr>
        <tr>
            <td>ul</td>
            <td>unordered&nbsp;list</td>
            <td>不排序列表</td>
        </tr>
        <tr>
            <td>var</td>
            <td>variable</td>
            <td>变量</td>
        </tr>
    </tbody>
</table>

> 语义化你的代码：http://mrthink.net/html-tips-semantization/

##注释##

```<!--#S 这里是注释-->
<div id="content">
    <div class="box"></div>
</div><!--#E 这里是注释-->```
