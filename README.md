# Intro
Ambari 集成 Azkaban

# Major Project Structure
- configuration : azkaban 配置文件
- package : 
  - scripts :  ambari 管理逻辑脚本
    - azkaban_executor.py  
    - azkaban_web.py
    - common.py
    - download.ini
    - params.py
Building from Source
Azkaban builds use Gradle (downloads automatically when run using gradlew which is the Gradle wrapper) and requires Java 8 or higher.

The following commands run on *nix platforms like Linux, OS X.
'''
# Build Azkaban
./gradlew build

# Clean the build
./gradlew clean

# Build and install distributions
./gradlew installDist

# Run tests
./gradlew test

# Build without running tests
./gradlew build -x test
'''
These are all standard Gradle commands. Please look at Gradle documentation for more info.

Gradle creates .tar.gz files inside project directories. eg. ./azkaban-solo-server/build/distributions/azkaban-solo-server-0.1.0-SNAPSHOT.tar.gz. Untar using tar -xvzf path/to/azkaban-*.tar.gz.
# Usage
https://cwiki.apache.org/confluence/display/AMBARI/Overview
