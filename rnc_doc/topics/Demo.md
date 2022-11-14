[//]: # (title: Demo)
[//]: # (<excerpt>标签页等功能演示.</excerpt>)


## 代码折叠

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
{collapsible="true" default-state="collapsed" collapsed-title="默认折叠的代码"}


```java
class Main {
}
```
{collapsible="true" default-state="expanded" collapsed-title="Title to display when a block is collapsed"}



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
