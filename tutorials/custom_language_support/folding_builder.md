---
title: 12. Folding Builder
---

A folding builder helps you to fold the code regions and replace it with specific text.

### 12.1. Define a folding builder

Let's replace usages of properties with its values by default.

```java
{% include /code_samples/simple_language_plugin/src/main/java/com/intellij/sdk/language/SimpleFoldingBuilder.java %}
```

### 12.2. Register the folding builder

```xml
<lang.foldingBuilder language="JAVA" implementationClass="com.simpleplugin.SimpleFoldingBuilder"/>
```

### 12.3. Run the project

Now when we open a Java file, it shows the property's value instead of the key.

![Folding](img/folding.png)
