# kubernetesのyamlをkustomizeを使って少しでも楽にする
我々の開発ではkubernetesにyamlを使って,サービスがどうあるべきかを定義していた.  

## 問題点
kubernetesを管理するにあたってyamlを使う必要があった.  
ただkubernetesのyamlは似たサービス(akane-auth,akane-convert..etc)は  
ほとんど同じようなyamlの構造になる.
これをサービスを新たに定義するたびに新たに書くのは非効率だと考えた.  

## 解決策
ベースとなるものを作成してそこから新たにyamlを生成ツールを導入した.  
検討したツールとして,以下の２つを検討した.

- helm
- kustomize

### helm
helmは変数という形でyamlを記述する.  
yaml生成からkubernetesへのinstallまでを担当してくれる.  
