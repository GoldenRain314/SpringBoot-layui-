# 解决springBoot架构下使用layui前端架构后，前端页面使用字体图标显示方块问题。
# 在pom.xml中的build标签下添加如下代码
 <pluginManagement>
            <plugins>
                <plugin>
                    <artifactId>maven-resources-plugin</artifactId>
                    <configuration>
                        <encoding>utf-8</encoding>
                        <useDefaultDelimiters>true</useDefaultDelimiters>
                        <nonFilteredFileExtensions>
                           <nonFilteredFileExtension>woff</nonFilteredFileExtension>
                            <nonFilteredFileExtension>woff2</nonFilteredFileExtension>
                            <nonFilteredFileExtension>eot</nonFilteredFileExtension>
                            <nonFilteredFileExtension>ttf</nonFilteredFileExtension>
                            <nonFilteredFileExtension>svg</nonFilteredFileExtension>
                        </nonFilteredFileExtensions>
                    </configuration>
                </plugin>
            </plugins>
        </pluginManagement>
        <resources>
            <resource>
                <directory>src/main/resources</directory>
                <includes>
                    <include>**.*</include>
                    <include>**/**.*</include>
                </includes>
                <filtering>true</filtering>
            </resource>
        </resources>
