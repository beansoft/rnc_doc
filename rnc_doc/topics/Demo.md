[//]: # (title: Demo)
[//]: # (<excerpt>标签页等功能演示.</excerpt>)


## 常用代码片段
```java
class Main {
    public static void main(String[] args) {
        System.out.println("Enter two numbers");
        int first = 10;
        int second = 20;
        System.out.println(first + " " + second);
// add two numbers
        int sum = first + second;
        System.out.println("The sum is: " + sum);
    }
}
```
{collapsible="true" default-state="collapsed"
collapsed-title="默认折叠的代码"}


```java
class Main {
}
```
{collapsible="true" default-state="expanded"
collapsed-title="Title to display when a block is collapsed"}


## control

Use the `control` tag to refer to UI elements such as buttons, dialogs, checkboxes, and so on.


<control>
Check out from Version Control
</control>

## ui-path

Use the `ui-path` tag to specify a path to a menu option.

In the <ui-path>Settings/Preferences</ui-path> dialog <shortcut>Ctrl+Alt+S</shortcut>

## path

Use the `path` tag for paths to directories and files on your computer or file extensions.

The TOC is stored in the product's
<path>.tree</path> file.

## 样式和小段落
<format style="bold" color="Red">Hello, world!</format>

{style="narrow"}
Default value
: `true`

Example
: 小段落

## 提示信息

> These pages have moved to [JetBrains Marketplace Documentation](https://plugins.jetbrains.com/docs/marketplace). Please update your bookmarks.
> {style="warning"}

<tip>Alternatively, you can change the settings directly in the configuration file.</tip>

<note>
    hello
</note>
<warning>warning</warning>

<tip>Tip</tip>

&lt;tooltip&gt; 标记需要在 <path>cfg/glossary.xml</path> 中添加解释.
<tooltip term="RN">RN Console</tooltip>

> This is a warning
>
{style="warning"}

> This is a note in markdown
>
{style="note"}

> This is a tip
>
{style="tip"}

> This is a todo
>
>

## 步骤
<procedure title="步骤" collapsible="true">
    <step>
        <p>
            Call the following command in the terminal:
        </p>
        <code-block lang="bash">
            run this --that
        </code-block>
    </step>
</procedure>

## 图片
![Getting Service](rnconsole-install-dark.png){thumbnail="true" thumbnail-same-file="true"}

<img src="screenshot_.gif" alt="" />

[//]: # (![Screenshot]&#40;screenshot_.gif&#41;&#41;{width="32" animated="true"  alt="Alt" border-effect="rounded" thumbnail="true" thumbnail-same-file="true"})

## 左右表格
<table>
            <tr>
                <td width="50%">Markup</td>
                <td width="50%">Result</td>
            </tr>
            <tr>
                <td>
                    <code-block>
                        ![](sample-image-white.png) alt="Sample image"  {width="250px"}
                    </code-block>
                </td>
                <td>
                    <img src="screenshot_.gif" alt="Sample image" width="250"/>
                </td>
            </tr>
</table>

## 标签页 + Markdown
<tabs>
    <code lang="java">Java code</code>
    <code lang="groovy">Groovy code</code>
</tabs>


<tabs group="languages">
<tab title="Kotlin" group-key="kotlin">

```kotlin
plugins {
    id("org.jetbrains.intellij") version "..."
}
```

</tab>
<tab title="Groovy" group-key="groovy">

```groovy
plugins {
    id "org.jetbrains.intellij" version "..."
}
```

</tab>
</tabs>

## 标签页联动

<tabs group="languages">
    <tab title="Kotlin" group-key="kotlin">
        <p>This is Kotlin.</p>
    </tab>
    <tab title="Java" group-key="java">
        <p>This is Java.</p>
    </tab>
</tabs>

<tabs  group="languages">
    <tab title="Kotlin Theory" group-key="kotlin">
        <p>This is Kotlin theory.</p>
    </tab>
    <tab title="Java Theory" group-key="java">
        <p>This is Java theory.</p>
    </tab>
</tabs>
