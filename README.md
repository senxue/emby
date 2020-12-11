&nbsp;
<p align="center">
  <img src="https://raw.sevencdn.com/echoops/emby/main/Emby.png" width="120px" alt="Emby" />
</p>
<h3 align="center">
   Your personal media on any device.
</h3>
&nbsp;

## Configure

* Quantumult X
```ini
[policy]
static=Emby, direct, proxy, img-url=https://raw.githubusercontent.com/echoops/emby/main/IconSet/Emby.png

[filter_remote]
https://raw.githubusercontent.com/echoops/emby/main/Filter/Emby.list, tag=Emby, update-interval=86400, enabled=true

[rewrite_remote]
https://raw.githubusercontent.com/echoops/limitless/main/QuantumultX/Rewrite/emby.qxrewrite, tag=Emby Premiere, update-interval=86400, enabled=true
```

* Surge 示例
```ini
[Proxy]
🌐Direct = direct

[Proxy Group]
# EMBY策略
🎞Emby = select,🌐Direct,🌑Proxy
# 代理策略
🌑Proxy = select,✈️Airport
# 机场订阅
✈️Airport = select, policy-path=你的机场订阅地址

[Rule]
RULE-SET,https://raw.githubusercontent.com/echoops/emby/main/Ruleset/Emby.list,🎞Emby
```

* Loon 示例
```ini
[Remote Proxy]
Airport = 你的机场订阅地址

[Proxy Group]
# 代理策略
PROXY = select,Airport
# EMBY策略
Emby = select,DIRECT,PROXY

[Remote Rule]
https://raw.githubusercontent.com/echoops/emby/main/Ruleset/Emby.list, policy=Emby, tag=Emby, enabled=true
```

&nbsp; 
## Disclaimer  

```ini
ONLY FOR STUDY, NOT FOR COMMERCIAL USE  
```

&nbsp;   
&nbsp; 
<h3 align="right"> ENJOY ! </h3>