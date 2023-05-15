# Native-with-resource
Add resources into native image, follow graavm native-build-tools sample : [java-application-with-resources](https://github.com/graalvm/native-build-tools/tree/master/samples/java-application-with-resources)

# How to use
Use this command:
```
mvn -Pnative clean package
```
If you want skip tests, use this command:
```
mvn -Pnative clean package -DskipTests=true
```
After build complete, you can see messages like this:
```
Finished generating 'example-app' in 22.5s.
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  25.910 s
[INFO] Finished at: 2023-05-15T09:13:40+08:00
[INFO] ------------------------------------------------------------------------
```
Then, you can run this command :
```
./target/example-app
```
The results:
```
{
  "hello": "world"
}
Hello, native!
```

