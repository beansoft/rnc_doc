Content other than text or CDATA in a code block, for example, HTML/XML-like tags

出错原因(不允许混合使用 HTML + <td> ？)：
<td>
<code-block lang="plain text">
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
\```
</code-block>
</td>

改用
<code-block><![CDATA[
                    ```kotlin
                    ```
                    {src="newTest.kt"}
            ]]></code-block>

？