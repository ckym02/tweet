- URL（PATH）とMethod、何をやるかの一覧作成

対象の機能は以下の通り。

- ユーザを表示する
- ツイートする
- ツイートに返信する
- リツイートする(引用リツイートも)
- フォローする
- フォロー一覧を表示する
- フォロワー一覧を表示する
- リストを追加する
- リストにユーザーを追加する
- リストからユーザーを削除する
- リスト一覧を表示する


|Method|Path|Description|
|---|---|---|
|GET|/users/{user_id}|user_idに基づいてユーザを表示する|
|POST|/tweets|ツイートする|
|POST|/tweets/{tweet_id}/replies|tweet_idのツイートに返信する|
|POST|/tweets/{tweet_id}/retweets|tweet_idのツイートをリツイートする|
|POST|/followings/{user_id}|user_idのユーザをフォローする|
|GET|/followings|フォロー一覧を表示する|
|GET|/followings/followers|フォロワー一覧を表示する|
|POST|/lists|リストを追加する|
|POST|/lists/{list_id}/list_users|list_idのリストにユーザを追加する|
|DELETE|/list/{list_id}/list_users/{user_id}|list_idのリストからuser_idのユーザを削除する|
|GET|/lists|リスト一覧を表示する|
