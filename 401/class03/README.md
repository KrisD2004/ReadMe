# File Manipulation / System.IO

## File and Stream I/O

* File and stream I/O involves the transfer of data to or from a storage medium.
* In .NET, the System.IO namespaces provide types for reading and writing on data streams and files.
* A file is an ordered collection of bytes with persistent storage, while a stream is a sequence of bytes that can be used to read from and write to a backing store.
* The System.IO namespace provides classes for interacting with files and directories, such as File, FileInfo, Directory, and DirectoryInfo.
* Streams support reading, writing, and seeking operations. The Stream class is an abstract base class, and there are various derived classes for different types of streams, such as FileStream, IsolatedStorageFileStream, MemoryStream, NetworkStream, and PipeStream.
* The System.IO namespace also includes reader and writer classes for reading encoded characters from streams and writing them to streams. Some commonly used classes are BinaryReader, BinaryWriter, StreamReader, StreamWriter, StringReader, StringWriter, TextReader, and TextWriter.
* Asynchronous I/O operations are recommended for resource-intensive tasks to keep the application responsive. Asynchronous members with "Async" in their names, such as ReadAsync and WriteAsync, are used along with the async and await keywords.
* The System.IO.Compression namespace provides classes for compressing and decompressing files and streams, including ZipArchive, ZipArchiveEntry, ZipFile, DeflateStream, and GZipStream.
* Isolated storage is a mechanism for storing application data in an isolated and controlled manner. It is particularly useful when the application doesn't have permission to access user files.
* When working with I/O operations in Windows 8.x Store apps, there are some differences compared to traditional .NET applications, such as the use of types in the Windows.Storage namespace instead of System.IO for file operations and the absence of isolated storage.
* Security considerations include following operating system security requirements, managing access control lists (ACLs), and avoiding direct access to physical files in internet or intranet applications.

## how to write text to a file

* There are several classes and methods in .NET that can be used to write text to a file, such as StreamWriter, File, and Path.
* The StreamWriter class provides methods for synchronous (Write, WriteLine) and asynchronous (WriteAsync, WriteLineAsync) writing of text to a file.
* The File class offers static methods for writing text to a file (WriteAllLines, WriteAllText) and appending text to an existing file (AppendAllLines, AppendAllText, AppendText).
* The Path class is used for manipulating file and directory paths, including methods like Combine for concatenating path strings.
* Example 1: Synchronously write text with StreamWriter. It demonstrates how to write text to a new file using StreamWriter in a using statement for proper disposal.
* Example 2: Synchronously append text with StreamWriter. It shows how to append text to an existing file using StreamWriter with the "true" parameter to enable appending mode.
* Example 3: Asynchronously write text with StreamWriter. It illustrates how to asynchronously write text to a new file using the async and await keywords.
* Example 4: Write and append text with the File class. It demonstrates using the File class methods, such as WriteAllText and AppendAllLines, to write and append text to a file.
The examples provided are minimal and should be enhanced with proper error checking and exception handling in real-world applications.

## how to read and write to a newly created data file

* The example demonstrates the usage of the System.IO.BinaryWriter and System.IO.BinaryReader classes for writing and reading data other than character strings.
* The code creates an empty file stream called "Test.data" in the current directory using the FileStream class with FileMode.CreateNew.
* It then uses a BinaryWriter object to write integers 0 through 10 to the file, and sets the file pointer at the end of the file.
* Next, a BinaryReader object is created and used to set the file pointer back to the beginning of the file and read the integers from the file.
* If the file "Test.data" already exists in the current directory, an IOException exception is thrown. To always create a new file without throwing an exception, use FileMode.Create instead of FileMode.CreateNew.


## Things i want to know more about 

