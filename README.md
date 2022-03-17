# b4x20220317
B4X實驗: B4J B4X 流(Stream)、文件(File)和IO (可參考Java作法)

B4X實驗: B4J B4X 流(Stream)、文件(File)和IO (可參考Java作法)
參考資料:
https://www.b4x.com/android/help/files.html 
https://www.b4x.com/android/help/randomaccessfile.html

https://www.cnblogs.com/java-chen-hao/p/11083740.html
https://kknews.cc/zh-tw/code/azk56jn.html

1.Stream流
在Java IO中，流是一個核心的概念。流從概念上來說是一個連續的數據流。
你既可以從流中讀取數據，也可以往流中寫數據。流與數據源或者數據流向的媒介相關聯。
在Java IO中流既可以是字節流(以字節為單位進行讀寫)，也可以是字符流(以字符為單位進行讀寫)。

2.類InputStream, OutputStream, TextReader 和TextWriter
输入流：InputStream和Reader
输出流：OutputStream和Writer

AsyncStreams
 

那麼OutputStream流到底是一個輸出到目的地的流呢，還是一個產生輸出的流？
InputStream流到底會不會輸出它的數據給讀取數據的程序呢？就我個人而言，
在第一天學習Java IO的時候我就感覺到了一絲疑惑。
原文網址：https://kknews.cc/code/azk56jn.html


Private InputStream1 As InputStream 
InputStream1 = File.OpenInput(File.DirAssets, "smiley.gif") 
Private OutputStream1 As OutputStream 
OutputStream1.InitializeToBytesArray(1000) 
File.Copy2(InputStream1, OutputStream1) 
Private Buffer() As Byte 'declares an empty array 
Buffer = OutputStream1.ToBytesArray


https://www.b4x.com/android/forum/threads/b4x-bytes-to-file.70111/#content




https://github.com/eric19740521/b4x20220317
