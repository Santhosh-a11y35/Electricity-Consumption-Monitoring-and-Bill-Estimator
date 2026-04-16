# Electricity Consumption Monitor & Bill Estimator

Simple Java Swing application to manually input meter readings (daily/weekly), visualize usage, estimate monthly bills, and generate PDF reports.

Requirements
- Java 11+
- Maven

Build & Run

1. From project root run:

```powershell
mvn clean compile exec:java -Dexec.mainClass="com.estimator.Main"
```

Notes
- The app uses Apache PDFBox (declared in `pom.xml`) to produce PDF reports.
- Enter cumulative meter readings (total meter value). Consumption is calculated as differences between consecutive readings.
- The chart is a simple in-app bar chart drawn with Swing.

If you'd like a runnable JAR instead, run `mvn package` and then run the produced jar (you may need to include dependencies using the Maven assembly or shade plugin).
