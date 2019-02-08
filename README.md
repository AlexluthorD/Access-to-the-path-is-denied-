# Access-to-the-path-is-denied-
Hello,  
i just develop a antivirus in vb.net, and i'm getting the error below. The application needs to scan files in the given path, 
and i'm being denied access.  Can you explain what could be causing the error? could it be code bug? 
thanks

System.UnauthorizedAccessException
  HResult=0x80070005
  Message=Access to the path 'C:\Users\admin\AppData\Local\Application Data' is denied.
  Source=mscorlib
  StackTrace:
   at System.IO.__Error.WinIOError(Int32 errorCode, String maybeFullPath)
   at System.IO.FileSystemEnumerableIterator`1.CommonInit()
   at System.IO.FileSystemEnumerableIterator`1..ctor(String path, String originalUserPath, String searchPattern, SearchOption searchOption, SearchResultHandler`1 resultHandler, Boolean checkHost)
   at System.IO.DirectoryInfo.InternalGetFiles(String searchPattern, SearchOption searchOption)
   at System.IO.DirectoryInfo.GetFiles(String searchPattern, SearchOption searchOption)
   at New_Design.Custom_Scan.Getfiles(String Path) in C:\Users\admin\source\repos\New Design\New Design\Custom Scan.vb:line 30
   at New_Design.Custom_Scan.Getfiles(String Path) in C:\Users\admin\source\repos\New Design\New Design\Custom Scan.vb:line 34
   at New_Design.Custom_Scan.Getfiles(String Path) in C:\Users\admin\source\repos\New Design\New Design\Custom Scan.vb:line 34
   at New_Design.Custom_Scan.Scan(String Path) in C:\Users\admin\source\repos\New Design\New Design\Custom Scan.vb:line 61
   at New_Design.Custom_Scan.BackgroundWorker1_DoWork(Object sender, DoWorkEventArgs e) in C:\Users\admin\source\repos\New Design\New Design\Custom Scan.vb:line 121
   at System.ComponentModel.BackgroundWorker.OnDoWork(DoWorkEventArgs e)
   at System.ComponentModel.BackgroundWorker.WorkerThreadStart(Object argument)
