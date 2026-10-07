# deposit-calculator (лабораторная работа № 2)

Калькулятор банковских вкладов (простые и сложные проценты), собираемый Apache Ant, Apache Maven и Gradle.

## Требования
JDK 17+, Apache Ant 1.10.x (с ant-junitlauncher и ant-junit), Apache Maven 3.9.x. Gradle — по желанию.

## Ant (JAR для JUnit 5 лежат в lib/)
    ant -p
    ant clean all      # полная чистая сборка: тесты, HTML-отчёт, JAR
    ant run
Отчёты: build/reports/xml, build/reports/html/index.html

## Maven
    mvn clean verify
    mvn surefire-report:report     # HTML: target/site/surefire-report.html

## Gradle (расширение)
    gradle wrapper --gradle-version 9.8   # один раз
    ./gradlew build

## Структура
src/main/java/by/student/deposit/{model/Deposit,service/DepositCalculator,Main}.java
src/test/java/by/student/deposit/DepositCalculatorTest.java (10 тестов)
