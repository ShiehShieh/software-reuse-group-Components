## Packer 压缩构件

> 提供文件定时压缩功能，并提供是否需要在压缩之前解压缩以及加密等功能。

### PackerTimer

#### 创建实例

```
	PackerTimer packerTimer = new PackerTimer("/iPath","/oPath");
```
#### 设置时间间隔
> 默认 1 TimeUnit.DAYS

```
	packerTimer.setInterval(1,TimeUnit.MINUTES);
```
#### 设置时间延时
> 默认 0 TimeUnit.DAYS

```
	packerTimer.setDelay(1,TimeUnit.MINUTES);
```
#### 开始

```
	packerTimer.start();
```
#### 停止

```
	packerTimer.stop();
```
#### 设置文件后缀
> 默认 *.log*

```
	packerTimer.setPackSuffix(".log");
```

#### 设置文件输出日期格式
> 默认 *yyyy-MM-dd*

```
	packerTimer.setPackDateFormat("yyyy-MM-dd");
```
#### 设置是否保留原文件
> 默认 *false*

```
	packerTimer.setbReserve(true);
```
#### 设置是否需要解压缩
> 默认 *false*

```
	packerTimer.setbUnpack(true);
```
#### 设置是否需要解压缩
> 默认 *true*

```
	packerTimer.setbEncryptIt(false);
```
