# Fdfs_client for go

The Golang interface to the Fastdfs Ver 4.06.

## Notice:Only realized the upload,download, delete functions

## Installation

```bash
$ go get github.com/weilaihui/fdfs_client
```

## Getting Started

see client_test.go please 

## Test

```bash
go test -v
=== RUN   TestParserFdfsConfig
    TestParserFdfsConfig: client_test.go:21: /data/fastdfs/client
--- PASS: TestParserFdfsConfig (0.00s)
=== RUN   TestNewFdfsClientByTracker
--- PASS: TestNewFdfsClientByTracker (0.01s)
=== RUN   TestUploadByFilename
    TestUploadByFilename: client_test.go:45: group1
    TestUploadByFilename: client_test.go:46: group1/M00/00/00/rBAKCl58nK2AeKzdAAAHXcwzLJY82.conf
--- PASS: TestUploadByFilename (0.02s)
=== RUN   TestUploadByBuffer
    TestUploadByBuffer: client_test.go:77: group1
    TestUploadByBuffer: client_test.go:78: group1/M00/00/00/rBAKCl58nK2AVHukAAAABTfs2ic638.txt
--- PASS: TestUploadByBuffer (0.01s)
=== RUN   TestUploadSlaveByFilename
    TestUploadSlaveByFilename: client_test.go:93: group1
    TestUploadSlaveByFilename: client_test.go:94: group1/M00/00/00/rBAKCl58nK2AfBnhAAAHXcwzLJY22.conf
    TestUploadSlaveByFilename: client_test.go:101: group1
    TestUploadSlaveByFilename: client_test.go:102: group1/M00/00/00/rBAKCl58nK2AfBnhAAAHXcwzLJY22_test
--- PASS: TestUploadSlaveByFilename (0.02s)
=== RUN   TestDownloadToFile
    TestDownloadToFile: client_test.go:120: group1
    TestDownloadToFile: client_test.go:121: group1/M00/00/00/rBAKCl58nK2AaZCsAAAHXcwzLJY60.conf
    TestDownloadToFile: client_test.go:131: 1885
    TestDownloadToFile: client_test.go:132: group1/M00/00/00/rBAKCl58nK2AaZCsAAAHXcwzLJY60.conf
--- PASS: TestDownloadToFile (0.01s)
=== RUN   TestDownloadToBuffer
    TestDownloadToBuffer: client_test.go:147: group1
    TestDownloadToBuffer: client_test.go:148: group1/M00/00/00/rBAKCl58nK2AL9xeAAAHXcwzLJY69.conf
    TestDownloadToBuffer: client_test.go:157: 1885
    TestDownloadToBuffer: client_test.go:158: group1/M00/00/00/rBAKCl58nK2AL9xeAAAHXcwzLJY69.conf
--- PASS: TestDownloadToBuffer (0.01s)
=== RUN   TestGetConnection
--- PASS: TestGetConnection (0.01s)
PASS
ok  	github.com/hzde0128/fdfs_client	1.225s
```
