# ObjectExplorer

Fork from [DimitrisAndreou/memory-measurer](https://github.com/DimitrisAndreou/memory-measurer) 

1. Rewrite it by using pure Java 8 API instead of Google Guava
2. Convert it to maven project 


## How to use

```java
long memory = MemoryMeasurer.measureBytes(new HashMap());
```

or

```java
Footprint footprint = ObjectGraphMeasurer.measure(new HashMap());
```

### Quick tip

- `mvn clean package` - to package jar
- To use the MemoryMeasurer (to measure the footprint of an object
graph in bytes), this parameter needs to be passed to th VM:
`-javaagent:path/to/object-explorer.jar`
