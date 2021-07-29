# Create a zip file with the contents of C:\Stuff\
```
Compress-Archive -Path <some file path> -DestinationPath archive.zip
```

# Add more files to the zip file
# (Existing files in the zip file with the same name are replaced)
```
Compress-Archive -Path C:\ < Other files >\*.<file extension> -Update -DestinationPath archive.zip
```

# Extract the zip file to C:\Destination\
```
Expand-Archive -Path archive.zip -DestinationPath <Destination path>
```

Reference:
[docs.microsoft.com](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.archive/compress-archive?view=powershell-7.1)
