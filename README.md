# mybatis-generator-core
mybatis generator改写 UTF-8编码 字段和方法中文注释
- UTF-8编码
- 添加类注释 作者信息
- 添加字段以及数据库字段注释
- 添加方法注释
- XML文件换行
# 使用方法
- 1.将jar包放置到本地maven仓库org\mybatis\generator\mybatis-generator-core\1.3.6-zh-CN下
- 2.pom中  
            ``<plugin>
                <groupId>org.mybatis.generator</groupId>
                <artifactId>mybatis-generator-maven-plugin</artifactId>
                <version>1.3.6</version>
                <configuration>
                    <configurationFile>src/main/resources/mybatis-generator/generatorConfig.xml</configurationFile>
                    <verbose>true</verbose>
                    <overwrite>true</overwrite>
                </configuration>

                <dependencies>
                    <dependency>
                        <groupId>org.mybatis.generator</groupId>
                        <artifactId>mybatis-generator-core</artifactId>
                        <version>1.3.6-zh-CN</version>
                    </dependency>
                    <dependency>
                        <groupId>mysql</groupId>
                        <artifactId>mysql-connector-java</artifactId>
                        <version>${mysql.version}</version>
                    </dependency>
                </dependencies>
            </plugin>`
