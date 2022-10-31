[//]: # (title: Tabs)
<excerpt>标签页等功能演示.</excerpt>

![Getting Service](rnconsole-install-dark.png){thumbnail="true" thumbnail-same-file="true"}

![动图](screenshot_.gif)){width="706"}{animated="true"}{border-effect="rounded"}

{style="narrow"}
Default value
: `true`

Example
:
小段落

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

> These pages have moved to [JetBrains Marketplace Documentation](https://plugins.jetbrains.com/docs/marketplace). Please update your bookmarks.
> {style="warning"}

<tip>Alternatively, you can change the settings directly in the configuration file.</tip>

<note>
    hello
</note>
<warning>warning</warning>

<tip>Tip</tip>
<tooltip>Tooltip</tooltip>

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
