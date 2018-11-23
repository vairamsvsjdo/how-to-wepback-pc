# Kill Process
Sometimes the process that was created from Visual Studio through Kestrel does not get killed even after Visual Studio is shutdown and restarted. In which subsequent restart does not allow to run the application 

In which case, follow these steps below in command promt

``` batch
netstat -ano
taskkill /f /im [pid of the port 5000 from the above command]
```
