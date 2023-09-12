---
sidebar_label: 'MFT Terminology'
---
# Terminology

**Groups**: defines general attributes for execution of a task

**Endpoints**: or site. MFT has two types of Endpoints: Path and Site endpoints.

**Path Endpoints**: or Local Endpoint, is either a UNC path, ```\\<server>\<directory>```, or a path that includes the drive letter, ```C:\<Directory>```.

**Site Endpoints**: or Managed Sites, is a remote location such as a FTP, FTPS, SFTP, SSH, S3, HTTP or HTTPS servers. When defining UNIX/Linux endpoints SFTP (SSH File Transfer protocol) should be used and FTP, FTPS, HTTP, HTTPS or S3 for other server.

**Tasks**: consists of multiple steps that are executed in a specific order. These individual steps are persisted and provide a restart point after a file transfer failure occurs.

