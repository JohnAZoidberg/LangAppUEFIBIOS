# VFR to HTML converter

## Building and running

###### Prerequisites
Maven and JDK8

###### Building

```
mvn compile
mvn package
```

###### Running

The example VFR file from Williams' thesis is included as `example.vfr`, as
well as the required strings in `strings.txt`.

```
java -jar target/vfr-to-html-0.1.0.jar
```

###### Enjoy the HTML
```
firefox vfr_preview.html
```

## Generating the parsing code

###### Prerequisites
ANTLR4

###### Building
```
cd ../ANTLR/
antlr vfr.g4
cp *.java ../vfr/src/main/java/com/williamleara/utexas/mastersreport/
```
