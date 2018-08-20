
# PCF 설치 가이드
https://docs.pivotal.io/pivotalcf/2-2/customizing/pcf-aws-manual-config.html

## AWS IAM 계정 생성

## 설치 준비
* DNS 
* IAM limit (VM) : 50개 신청
* EIP: 계정 하나에서 vpc여러개 만들 경우 10이상필요.


## aws cli 설치(옵션):
https://aws.amazon.com/cli/

```
$ 
brew install python@2
pip install --upgrade pip setuptools
pip install awscli

```


### aws cli 동작 확인:

```
$ 
aws ec2 describe-availability-zones 
{
    "AvailabilityZones": [
        {
            "State": "available", 
            "ZoneName": "ap-northeast-2a", 
            "Messages": [], 
            "RegionName": "ap-northeast-2"
        }, 
        {
            "State": "available", 
            "ZoneName": "ap-northeast-2c", 
            "Messages": [], 
            "RegionName": "ap-northeast-2"
        }
    ]
}
```


