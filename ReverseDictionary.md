# 逆引き索引
<dl>
    <dt>基本的な用語<dt/>
    <dd>
    
| 目的 | 使用する時に必要なキーワード |
----|----
| ゲームに登場させる基本単位 | GameObject |
| モジュールを追加させること | アタッチ |
| モジュールを追加させるメソッド | AddComponent |
| 機能を追加させるコードを書く時に使う用語 | MonoBehaviour 継承クラス, イベント関数 |
| 初期化処理のイベント関数 | Awake, Start |
| 毎フレーム更新させるイベント関数, 入力判定を記述する場所 | Update, FixedUpdate |
| パターンが決まっている物を利用する時 | プレハブ (Prefab) |

<dd/>
    <dt>独自の動きをさせたい<dt/>
    <dd>MonoBehaviour 継承クラス、イベント関数, Awake, Start, Update<dd/><br/>
    <dt>画像</dt>
    <dd>

| 目的 | 使用する時に必要なキーワード |
----|---- 
| 接触判定時に使うメソッド | OnTriggerEnter2D, Exit2D, Stay2D メソッド |
<dd/>

| 目的 | 使用する時に必要なキーワード |
----|----
| 画像を表示したい | UnityUI（ジャンル） , Sprite, Image |
| 画像を動かしたい | Transform クラス<br/>Transform.position(localPosition)プロパティ（単純な移動） <br/> Rigidbody.MovePosition メソッド（衝突判定利用時）|

</dd>

<dt> 画像を動かす時に使う用語 </dt>
<dd> 物理演算、衝突・接触判定 </dd>
<dd>

| 目的 | キーワード |
----|----
| 物理演算 | Rigidbody2D, AddForce メソッド|
| 物理演算を使わない場合 | Rigidbody2D　クラス, Kinematic プロパティ, MovePosition　メソッド |
| 衝突・接触判定に必要なクラス | Collider2D クラス|
| 衝突・接触判定時に使う関数 |　OnTriggerEnter2D イベント関数<br/> OnCollisionEnter2D イベント関数|

</dd>

<dt>動作確認を行いたい</dt>
<dd>Dbug.Log メソッド<dd/>


</dl>
