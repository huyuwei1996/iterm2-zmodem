## mac安装lrzsz

brew install lrzsz

## 配置iterm2 Trigger

选择Profiles > Default > Advanced > Triggers > Edit


### 发送 sz

```
Regular expression: rz waiting to receive.\*\*B0100
Action: Run Silent Coprocess
Parameters: /opt/homebrew/bin/iterm2-send-zmodem.sh
```
### 接收 rz

```
Regular expression: \*\*B00000000000000
Action: Run Silent Coprocess
Parameters: /opt/homebrew/bin/iterm2-recv-zmodem.sh
```