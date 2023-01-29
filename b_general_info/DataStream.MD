## PRIMARY DATA STREAM AND ALTERNATE DATA STREAM

- In the Windows NTFS file system, every file has one or more data streams associated with it. The primary data stream is the default data stream for a file and is the one that is typically used when a file is opened or edited. It is also the stream that is typically displayed by Windows Explorer and other file managers when you view the properties of a file.

- The primary data stream contains the main data of the file, such as its text or binary content. It is also the stream that is typically displayed by Windows Explorer and other file managers when you view the properties of a file.

- When a file is created, the primary data stream is automatically created along with it. It is the "normal" contents of a file, that can be viewed or modified with regular file editing tools.

- It is important to note that the primary data stream is not visible to the user, it can be accessed only through the File System API, that means that the primary data stream is not an additional file or folder, it is just a part of the normal file, Windows Operating System understands that a file has a primary data stream, but the user does not have a way to see it directly.

- Also, NTFS allows the creation of Alternate Data Streams, which are additional data streams that can be associated with a file, they are not visible to the user and can only be accessed through the File System API.