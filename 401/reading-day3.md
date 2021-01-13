# System.I.O

## File and Stream I/O
- file and stream I/O (input/output) refers to the transfer of data either to or from a storage medium. In .net the System.IO namespaces contain types that enable reading or writing both synchronously and asynchronously, on data streams and files. 
- these namespaces also contain types that perform compression & decompression on files, as well as types that enable communication through pipes and serial ports. 
- A file is an ordered & named collection of bytes that has persistent storage. When you work w/ files, you work with directory paths, disk storage and file/directory names. 
- *Files and directories*:
- You can use the "System.IO" namespace to interact with files and directories. Ex: you can get and set properties for files & directories, retrieve collections of files and directories based on search criteria.
- **Commonly used file & directory classes:**
- File- provides static methods for creating, copying, deleting, moving, and opening files.
- FileInfo- provides instance methods for creating, copying, deleting, moving and opening files.
- Directory- provides static methods for creating, moving, and enumerating through directories and subdirectories
- DirectoryInfo- provides instance methods for creating, moving, and enumerating through directories and subdirectories.
- Path- provides methods and properties for processing directory strings in a cross-platform manner.
- **Streams**:
- This abstract base class supports reading and writing bytes. All classes that represent streams inherit from the Stream class. This class and its derived classes provide a common view of data sources and repositories, and isolate the programmer from the specific details of operating system and underlying devices.
- *Streams involve 3 fundamental operations:
- Reading- transferring data from a stream into a data structure, such as an array of bytes.
- Writing- transferring data to a stream from a data source.
- Seeking - querying and modifying the current position within a stream.
- **Readers and writers**:
- BinaryReader and BinaryWriter- for reading and writing primitive data types as binary values.
- StreamReader and StreamWriter- for reading and writing characters by using an encoding value to convert the characters to and from bytes.
- StringReader and StringWriter- for reading and writing characters to and from strings.
- TextReader and TextWriter- serve as the abstract base classes for other readers and writers that read and write characters and strings, but not binary data.
- **Asynchronous I/O operations**:
- With synchronous I/O operations, the UI thread is blocked until the resource-intensive operation has completed.
- **Compression**:
- refers to the process of reducing the size of a file for storage. 
- https://docs.microsoft.com/en-us/dotnet/standard/io/

## Write to a file
- Classes and methods are typically used to write text to a file:
- **StreamWriter** contains methods to write to a file synchronously (Write and WriteLine) or asynchronously (WriteAsync and WriteLineAsync).
- **File** provides static methods to write text to a file, such as WriteAllLines and WriteAllText, or to append text to a file, such as AppendAllLines, AppendAllText, and AppendText.
- **Path** is for strings that have file or directory path information. It contains the Combine method and, in .NET Core 2.1 and later, the Join and TryJoin methods, which allow concatenation of strings to build a file or directory path.
- https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-write-text-to-a-file 

## Read to a file
- https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-read-and-write-to-a-newly-created-data-file 

- **Reference the above article for the information/coding example**
