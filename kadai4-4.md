## 自動販売機（オブジェクト、DOM、イベント処理）のミニレポート
### Q4-1. Itemクラスのメソッドについて説明せよ。
* showItemListがクラスメソッドである理由を考察せよ。
  showItemListがクラスメソッドなのは、全体の商品リストを一括して表示するからで、
　staticというのを入れることでクラスから直接呼び出せるようにしている
* buyItemがインスタンスメソッドである理由を考察せよ。
  buyitemがインスタンスメソッドなのは特定の商品の在庫数を減らすからで、
　特定の商品の情報にアクセスし、変更するにはthisの中にアクセスしなければならない
### Q4-2. 商品の購入ボタンをクリックすると、どのような処理でセルの値が減少するか説明せよ。
* 購入された商品の在庫数のセルをどのようにして特定するのか説明せよ。
  商品一つ一つにidが割り振られているので
　document.getElementById("stock" + this.id)というのでセルを特定している。
* 特定したセルの値をどのように変更するのか説明せよ。
  セルの値は textContent を使って変更する。
　stockElement.textContent = this.stock とすることで、在庫数が1つ減った新しい値に更新される
### Q4-3. 感想
* 今回の課題で苦労したこと
  内容がうまく理解できなかったが、資料見たりコードを見て少しずつ理解を
　深めながら取り組んだ。
* 演習を通して理解できたこと
  DOM操作の方法について学ぶことができました。
* この自動販売機プログラムの追加機能や課題など
　入れた金額に対してのお釣り計算とかあると良いと思う
