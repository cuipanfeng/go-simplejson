### go-simplejson

a Go package to interact with arbitrary JSON

[![Build Status](https://secure.travis-ci.org/bitly/go-simplejson.png)](http://travis-ci.org/bitly/go-simplejson)

### 使用说明
    
由于原作者在github中将项目命名为：go-simplejson，而包名是：simplejson。
所以，如果通过go get方式下载的话，建议如下方式使用：

    import simplejson github.com/bitly/go-simplejson

个人更建议直接 ```git clone https://github.com/polaris1119/go-simplejson simplejson```然后可以直接```import simplejson```使用

### 增加新功能

增加了如下函数/方法：
```
func (j *Json) GetStringSlice(key string) []string
```
```
func (j *Json) MustBool(args ...bool) bool
```
```
// 解析json文件，过滤掉注释（只支持注释在单独一行，以"//"注释）
func ParseFile(filename string) (*Json, error)
```
