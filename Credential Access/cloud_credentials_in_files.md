# cloud credentials in files



在att&ck云相关映射表中，[Credential Access](https://attack.mitre.org/tactics/TA0006/)提到了credentials in file

除了传统的代码配置文件中会存在这些凭证以外，云本身提供的cli、sdk、客户端等工具也会保存这些凭证文件

本文就以市面上常见的公有云厂家为例来探索这些凭证究竟都存在哪里了

持续更新



## CLI(Command Line Interface)



### aws



工具名称：aws-cli



平台：linux

```
~/.aws/credentials
~/.aws/config
~/.aws/cli/cache			#缓存凭证位置
```

平台：windows

```
%UserProfile%\.aws\credentials
%UserProfile%\.aws\config
%UserProfile%\.aws\cli\cache #缓存凭证位置
```

注明：%USERPROFILE% =C:\Users\用户名



### aws-cn



与aws国际版相同



### aliyun



工具名称：aliyun-cli



平台：linux

```
~/.aliyun/config.json
```

平台：windows

```
%UserProfile%\.aliyun\config.json
```

注明：%USERPROFILE% =C:\Users\用户名



### tencent



工具名称：tccli



平台：linux

```
~/.tccli/default.credential
~/.tccli/default.configure
```

平台：windows

```
%UserProfile%\.tccli\default.credential
%UserProfile%\.tccli\default.configure
```

注明：%USERPROFILE% =C:\Users\用户名



### azure-cn



敬请期待



### azure



敬请期待



### gcp



工具名称：gcloud



平台：linux

```
~/.config/gcloud/access_tokens.db
~/.config/gcloud/credentials.db
~/.config/gcloud/application_default_credentials.json
```



平台：windows

```
%UserProfile%\.config\gcloud\access_tokens.db
%UserProfile%\.config\gcloud\credentials.db
%UserProfile%\.config\gcloud\application_default_credentials.json
```

注明：%USERPROFILE% =C:\Users\用户名



### ucloud



工具名称：ucloud-cli



平台：linux

```
~/.ucloud/config.json
~/.ucloud/credential.json
~/.ucloud/cli        #这个文件保存了cli工具历史记录
```

平台：windows

```
%UserProfile%\.ucloud\config.json
%UserProfile%\.ucloud\credential.json
%UserProfile%\.ucloud\cli        #这个文件保存了cli工具历史记录
```

注明：%USERPROFILE% =C:\Users\用户名



### jd



工具名称：jdc

平台：linux

```
~/.jdc/config
~/.jdc/current
```

平台：windows

```
%UserProfile%\.jdc\config
%UserProfile%\.jdc\current
```

注明：%USERPROFILE% =C:\Users\用户名



## SDK

### aws



### aws-cn



### aliyun



### tencent



### azure-cn



### azure



### gcp



### ucloud



### jd



## 客户端



### 对象存储



工具名称：osstil



平台：linux

```
~/.ossutilconfig
```

平台：windows

```
%UserProfile%\.ossutilconfig
```

注明：%USERPROFILE% =C:\Users\用户名
