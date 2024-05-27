---
description: Describes how to add Minestom as a dependency in your project.
---

# Dependencies

{% hint style="info" %}
Minestom needs Java 21 or newer in order to run. If you are using Gradle, you must use version 8.5 or higher.
{% endhint %}

Adding Microtus to your Java project is really simple, you only need to add a few repositories:

## Repositories

{% tabs %}
{% tab title="Gradle (Groovy)" %}
```groovy
repositories {
    // ...
    mavenCentral()
}
```
{% endtab %}

{% tab title="Gradle (Kotlin)" %}
```groovy
repositories {
    // ...
    mavenCentral()
}
```
{% endtab %}
{% endtabs %}

## Dependencies

{% tabs %}
{% tab title="Gradle (Groovy)" %}
```groovy
dependencies {
    // ...
    implementation 'net.onelitefeather.microtus:Microtus:VERSION'
}
```
{% endtab %}

{% tab title="Gradle (Kotlin)" %}
```groovy
dependencies {
    //...
    implementation("net.onelitefeather.microtus:Microtus:VERSION")
}
```
{% endtab %}

{% tab title="Maven" %}
```markup
<dependencies>
    <!-- ... -->
    <dependency>
        <groupId>net.onelitefeather.microtus</groupId>
        <artifactId>Microtus</artifactId>
        <version>VERSION</version>
    </dependency>
</dependencies>
```

When using Maven it is recommended to exclude the artifact `shrinkwrap-resolver-depchain` from the group `org.jboss.shrinkwrap.resolver` as otherwise resolving the dependencies will fail. Shrinkwrap can be added as a separate dependency if needed without issues to restore its functionality.
{% endtab %}
{% endtabs %}

A list of versions can be found at [https://central.sonatype.com/search?q=microtus](https://central.sonatype.com/search?q=microtus).
