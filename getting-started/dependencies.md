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
    mavenCentral()
}
```
{% endtab %}

{% tab title="Gradle (Kotlin)" %}
```groovy
repositories {
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
    implementation platform('net.onelitefeather.microtus:bom:version')
    implementation 'net.onelitefeather.microtus:Microtus' // Main Components

    testImplementation 'net.onelitefeather.microtus.testing:testing' // Testing Components
}
```
{% endtab %}

{% tab title="Gradle (Kotlin)" %}
```kotlin
dependencies {
    implementation(platform("net.onelitefeather.microtus:bom:VERSION")
    implementation("net.onelitefeather.microtus:Microtus") // Main components

    testImplementation("net.onelitefeather.microtus.testing:testing") // Test components
}
```
{% endtab %}

{% tab title="Maven (Parent)" %}
```xml
<project ...>
    <modelVersion>4.0.0</modelVersion>
    <groupId>your.project</groupId>
    <artifactId>microtus-project</artifactId>
    <version>0.0.1-SNAPSHOT</version>
    <packaging>pom</packaging>
    <name>Microtus </name>
    <parent>
        <groupId>net.onelitefeather.microtus</groupId>
        <artifactId>bom</artifactId>
        <version>VERSION</version>
    </parent>
    
    <dependencies>
        <!-- ... -->
        <dependency>
            <groupId>net.onelitefeather.microtus</groupId>
            <artifactId>Microtus</artifactId>
        </dependency>
        <dependency>
            <groupId>net.onelitefeather.microtus.testing</groupId>
            <artifactId>testing</artifactId>
            <scope>test</scope>
        </dependency>
    </dependencies>
</project>
```
{% endtab %}

{% tab title="Maven" %}
```xml
<dependencyManagement>
    <dependencies>
        <dependency>
            <groupId>net.onelitefeather.microtus</groupId>
            <artifactId>bom</artifactId>
            <version>VERSION</version>
            <type>pom</type>
            <scope>import</scope>
        </dependency>
    </dependencies>
</dependencyManagement>
<dependencies>
    <!-- ... -->
    <dependency>
        <groupId>net.onelitefeather.microtus</groupId>
        <artifactId>Microtus</artifactId>
    </dependency>
    <dependency>
        <groupId>net.onelitefeather.microtus.testing</groupId>
        <artifactId>testing</artifactId>
        <scope>test</scope>
    </dependency>
</dependencies>
```
{% endtab %}
{% endtabs %}

**A list of versions can be found at** [**https://central.sonatype.com/search?q=microtus**](https://central.sonatype.com/search?q=microtus)**.**
