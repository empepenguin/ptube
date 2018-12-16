# kubernetesのyamlをkustomizeを使って少しでも楽にする
我々の開発ではkubernetesにyamlを使って,サービスがどうあるべきかを定義していた.  

## 問題点
kubernetesを管理するにあたってyamlを使う必要があった.  
ただkubernetesのyamlは似たサービス(akane-auth,akane-convert..etc)は  
ほとんど同じようなyamlの構造になる.
