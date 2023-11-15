---
hide:
  # - navigation
  - toc
---

# CLI命令

Clash.Rev支持的CLI命令如下：

```bash
Usage:
  clash [flags]

Flags:
      --cfg-header string   specify configuration file url header, env: CLASH_CONFIG_URL_HEADER
      --cfg-url string      specify configuration file url, env: CLASH_CONFIG_URL
  -f, --config string       specify configuration file, env: CLASH_CONFIG_FILE
  -d, --dir string          specify configuration directory, env: CLASH_HOME_DIR
      --ext-ctl string      override external controller address, env: CLASH_OVERRIDE_EXTERNAL_CONTROLLER
      --ext-ui string       override external ui directory, env: CLASH_OVERRIDE_EXTERNAL_UI_DIR
  -m, --geodata             set geodata mode
  -h, --help                help for clash
  -t, --test                test configuration and exit
  -v, --version             show current version of clash
```

## 配置文件

### `-d, --dir string`

指定配置文件目录，不传递时会使用环境变量`CLASH_HOME_DIR`的值，如果环境变量也没有设置，则会使用默认值`~/.config/clash`。

### `-f, --config string`

指定配置文件路径，不传递时会使用环境变量`CLASH_CONFIG_FILE`的值，如果环境变量也没有设置，则会使用默认值`config.yaml`。

### `--cfg-url string`

通过URL指定配置文件，不传递时会使用环境变量`CLASH_CONFIG_URL`的值。

### `--cfg-header string`

指定配置文件URL的头部，不传递时会使用环境变量`CLASH_CONFIG_URL_HEADER`的值。

## 控制器

### `--ext-ctl string`

指定外部控制器地址，不传递时会使用环境变量`CLASH_OVERRIDE_EXTERNAL_CONTROLLER`的值。

### `--ext-ui string`

指定外部UI目录，不传递时会使用环境变量`CLASH_OVERRIDE_EXTERNAL_UI_DIR`的值。

## 其他

### `-m, --geodata`

GEO数据模式。

### `-h, --help`

显示帮助信息。

### `-t, --test`

测试配置文件并退出。

### `-v, --version`

显示当前版本。
