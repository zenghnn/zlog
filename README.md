# zlog

> 这是一个日志功能整合包，包含了日志等级输出、日志按日期切分、日志内容格式化。使用了包括 go.uber.org/zap   github.com/lestrrat/go-file-rotatelogs

[![GoDoc][godoc-image]][godoc-url] [![License][license-image]][license-url]

## Get

``` bash
go get -u github.com/zenghnn/zlog
```

## Usage

``` go
package main

import (
	"github.com/zenghnn/zlog"
)

func main() {
	zlog.Debug("测试日志功能:")
}

```

## MIT License

``` text
    Copyright (c) 2023 zenor
```

[License-Url]: http://opensource.org/licenses/MIT
[License-Image]: https://img.shields.io/npm/l/express.svg
[GoDoc-Url]: https://godoc.org/github.com/LyricTian/queue
[GoDoc-Image]: https://godoc.org/github.com/LyricTian/queue?status.svg
