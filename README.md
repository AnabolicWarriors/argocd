# argocd
> argocd는 쿠버네티스의 지속적인 배포를 자동화 해주는 서비스이다. 이 레포지터리의 YAML을 갱신하기만 하면 자동으로 서버의 쿠버네티스에 적용된다.

## vnc/deployment-vncserver.yaml
### 쿠버네티스의 디플로이먼트를 만드는 YAML파일
>  vncserver, x11윈도우가 설치된 cli상의 리눅스 파드를 디플로이하는 YAML

## vnc/service-vncserver.yaml
### 쿠버네티스의 서비스를 만드는 YAML파일
> 위의 파드를 노출시켜주는 서비스를 생성하는 YAML
