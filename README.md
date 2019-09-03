![GitHub release (latest by date)](https://img.shields.io/github/v/release/hank-cp/spring-static-ctx)
![JitPack](https://img.shields.io/jitpack/v/github/hank-cp/spring-static-ctx)
![GitHub](https://img.shields.io/github/license/hank-cp/spring-static-ctx)


A Spring helper to get `ApplicationContext` in static way.

### Usage
```
    @Bean
    public ApplicationContextAware multiApplicationContextProviderRegister() {
        return MultiApplicationContextProvider::registerApplicationContext;
    }

    ApplicationContextProvider.getBean(MyBean.class);
```

* Maven
    ```
    <repositories>
        <repository>
            <id>jitpack.io</id>
            <url>https://jitpack.io</url>
        </repository>
    </repositories>
     
    <dependency>
        <groupId>com.github.hank-cp</groupId>
        <artifactId>spring-static-ctx</artifactId>
        <version>0.1.0</version>
    </dependency>
    ```
* Gradle
    ```
    allprojects {
        repositories {
            ...
            maven { url 'https://jitpack.io' }
        }
    }
        
    dependencies {
        implementation 'com.github.hank-cp:spring-static-ctx:0.1.0'
    }
    ```

### License 

```
/*
 * Copyright (C) 2019-present the original author or authors.
 *
 * Licensed under the Apache License, Version 2.0 (the "License");
 * you may not use this file except in compliance with the License.
 * You may obtain a copy of the License at
 *
 *     http://www.apache.org/licenses/LICENSE-2.0
 *
 * Unless required by applicable law or agreed to in writing, software
 * distributed under the License is distributed on an "AS IS" BASIS,
 * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 * See the License for the specific language governing permissions and
 * limitations under the License.
 */
```