# zlog

> 这是一个日志功能整合包，包含了日志等级输出、日志按日期切分、日志内容格式化。使用了包括 go.uber.org/zap   github.com/lestrrat/go-file-rotatelogs

[![GoDoc][godoc-image]][godoc-url] [![License][license-image]][license-url]

* 傻瓜化，已经使用默认的配置，如果你想修改可以直接复制文件，然后修改配置
``` go
	cf := Options{
		LogFileDir: "./logs",        	//默认生成文件夹为程序文件夹下logs
		MaxSize:    10,			// 一个文件多少Ｍ大于该数字开始切分文件
		MaxBackups: 7,			// MaxBackups是要保留的最大旧日志文件数
		MaxAge:     360,		// MaxAge是根据日期保留旧日志文件的最大天数
		Config: zap.Config{},
	}
```

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
