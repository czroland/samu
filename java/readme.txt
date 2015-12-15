Samu - java version

Instructions:
If after compile you give the linkgrammar library not found you need to make some simbolyc links, in link-grammar's directory for example link-grammar-5.2.5/
So type in terminal in link-grammar's directory:
 
sudo ln -sv "$(pwd)/link-grammar/.libs/liblink-grammar.so.5" /usr/lib/
sudo ln -sv "$(pwd)/bindings/java-jni/.libs/liblink-grammar-java.so" /usr/lib/


After that you can compile the project, in project's directory type the following, where
 /home/username/link-grammar-5.2.5/ is your link-grammar's  directory, the version could be other (5.3.1 or 5.3.2)

javac -cp /home/username/link-grammar-5.2.5/bindings/java/linkgrammar-5.2.5.jar *.java

For running, `pwd` because of simbolyc links.
java -cp /home/username/link-grammar-5.2.5/bindings/java/linkgrammar-5.2.5.jar:`pwd` Main

If you don't have link-grammar
http://www.abisource.com/projects/link-grammar/
