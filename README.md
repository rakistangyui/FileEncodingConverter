# FileEncodingConverter
Program that allows you to change encoding of a file.

Arguments
args[0] - Determine if this is a folder by using Y or N flag.<br>
args[1] - Input file or folder<br>
args[2] - Output file or just put NA if you are using the batch conversion<br>
args[3] - Default encoding when the encoding checker fails to check the current encoding of the file.<br>
args[4] - Your desired encoding for the output file.<br>
<br><br>
When you want to convert files inside a folder<br>
java -jar "C:\Users\u108381\Documents\NetBeansProjects\EncodeFile\dist\EncodeFile.jar" Y "D:\Danny" NA ISO-8859-1 x-UTF-16LE-BOM
<br><br>
When you want to convert a single file<br>
java -jar "C:\Users\u108381\Documents\NetBeansProjects\EncodeFile\dist\EncodeFile.jar" N "D:\Danny\Sample.txt" "D:\Danny\Sample_converted.txt" ISO-8859-1 x-UTF-16LE-BOM

