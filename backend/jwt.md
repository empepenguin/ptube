## 認証にはjwtを採用した

jwtの特徴

- 改ざんが検知できる
- ユーザー名などの任意の情報を含めることができる

jwtの採用理由としては以下があげられる

- セッションIDの認証と比べてJwtはTokenを保存しなくて済むので別途DBを用意する手間が省ける
- Validationする際にTokenの改ざんを調べるだけでいいためサーバーの負荷が減る

[jwt-go](https://github.com/dgrijalva/jwt-go)