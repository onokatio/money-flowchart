```mermaid
flowchart LR
  %% 還元情報
		%% VISA
		LINEPayVisa[LINEPayVisa 0%]
	  エポスゴールド[エポスゴールド +0.5%]
	  エポスゴールド2[エポスゴールド +1.5%]
		%% Master
		三井住友NL_VISA[三井住友NL VISA 0.5%]
    TカードPrime[TカードPrime 1.5%]
    三井住友NL_Master[三井住友NL Master 0.5%]
		%% JCB
		PayPayカード[PayPayカード +1%]
		ファミマTカード[ファミマTカード +0.5%]
		%% プリペイド
		ソフトバンクカード[ソフトバンクカード +0.5%]
    LinePayプリペイド[LinePayプリペイド +1%]
    Kyash[Kyash +0.2%]
    6gram[MIXI M 6gram]
		auPay[auPay +0.5%]
    TOYOTAWallet[TOYOTAWallet +1%]
    dカードプリペイド[dカードプリペイド +0.5%]
		ANAJCBプリペイド[ANAJCBプリペイド +0.5%]
    IDARE[IDARE +0.16%/月]
		%%スマホ決済
		PayPay[PayPay +1.5%]
    d払い[d払い +0.5%]
    FamiPay[FamiPay +10円]
    楽天Edy[楽天Edy +0.5%]

	%% クレジット
	TカードPrime --> auPay
  TカードPrime --> Kyash
  エポスゴールド2 --> 6gram
  エポスゴールド --> auPay
  LINEPayVisa --> TOYOTAWallet
  Payeasy --> Kyash
  エポスゴールド --> Bankit
  エポスゴールド2 --> ちょコムショップ
	エポスゴールド2 --> モバイルSuica
  PayPayカード --> ARIGATO
  PayPayカード --> FamiPay
	三井住友NL_VISA --> かぞくのおさいふ
	楽天カード_JCB --> 楽天バーチャルプリペイドカード
	JALカード --> JMB_WAON
	%% プリペイド
	auPay --> 6gram
  auPay --> B/43
  %%auPay --> nanaco
  %%auPay --> WAON
  %%auPay --> Revolut
  Kyash --> Revolut
  Kyash --> TOYOTAWallet
  Kyash --> 6gram
  Kyash --> IDARE
  Kyash --> B/43
  Kyash --> dカードプリペイド
  Kyash --> バンドルカード
  Kyash --> nanaco
	%%Kyash --> d払い
  6gram --> dカードプリペイド
  6gram --> モバイルSuica
  6gram --> WAON
  6gram --> nanaco
	Revolut --> ARIGATO
  %%Revolut --> モバイルSuica
  Revolut --> B/43
  Revolut --> Binance
  Revolut --> ソフトバンクまとめて決済
  %%Revolut --> |$-0.45| Wiseドル
  %%Revolut --> |-63円| Wise円
	TOYOTAWallet --> auかんたん決済
  TOYOTAWallet --> |Apple Pay| モバイルSuica
  TOYOTAWallet --> |0.5| Amazonギフト残高
  TOYOTAWallet --> WAON
  TOYOTAWallet --> nanaco
	ソフトバンクカード --> Amazonギフト残高
  ソフトバンクカード --> モバイルSuica
  ソフトバンクカード --> nanaco
  %%ソフトバンクカード --> 楽天ペイ
	IDARE --> B/43
  IDARE --> Revolut
  IDARE --> ShuttlePay
	%%Tマネー --> B/43
  %%Tマネー --> モバイルSuica
  %%Tマネー --> nanaco
	%%Tマネー --> 6gram
	ANAJCBプリペイド --> ARIGATO
  ANAJCBプリペイド --> ShuttlePay
	B/43 --> モバイルSuica
  B/43 --> ソフトバンクまとめて決済
  ARIGATO --> ShuttlePay
  ARIGATO --> ソフトバンクまとめて決済
  バンドルカード --> Revolut
  バンドルカード --> IDARE
  バンドルカード --> TOYOTAWallet
	%%LinePayプリペイド --> Kyash
	エポスプリペイド --> Revolut
	楽天バーチャルプリペイドカード --> auPay
  UCギフト --> Revolut
	%% 電子マネー・QR決済
	nanaco --> |ー4%|Vプリカ
  nanaco --> 楽天キャッシュ
	nanaco --> ANAプリペイド
  nanaco --> ベネフィットワン
  FamiPay --> バンドルカード
  FamiPay --> UltraPay
  FamiPay --> |コンビニ| ANAJCBプリペイド
  FamiPay --> IDARE
  FamiPay --> |0.5%| 楽天キャッシュ
	Revolut --> モバイルSuica
  モバイルSuica --> |2.5%| Amazonギフト残高
  楽天Edy --> |2.5%| Amazonギフト残高
  WAON --> バニラVISA
  WAON --> 楽天キャッシュ
	%% 携帯料金
	ソフトバンクまとめて決済 --> ソフトバンクカード
  ソフトバンクまとめて決済 --> PayPay残高
	ソフトバンクまとめて決済 --> Google支払い
	auかんたん決済 --> auPay
	楽天モバイル決済 --> Google支払い
	ドコモ電話料金合算払い --> dカードプリペイド
	%% ギフトカード
	Amazonギフトカード --> Amazonギフト残高
  %%Tマネーギフトカード --> Tマネー
  楽天ギフト --> 楽天キャッシュ
  majica --> POSA
	%% ネットショップ
	Giftee --> FamiPay
  Giftee --> auPay
  Giftee --> Kyashギフト
  Giftee --> majica
  ちょコムeマネー --> nanaco
  ちょコムショップ --> |+0.5%| nanaco
  ベネフィットワン --> UCギフト
  ベネフィットワン --> Giftee
	%% 残高利用
	楽天キャッシュ --> |+1%| 楽天ペイ
  PayPay残高 --> PayPay
	%% 外貨
	%%JPYC -> "Giftee Box"
	%%Binance --> USDT
  %%USDT --> USDC
  %%USDC --> JPYC
  %%Wiseドル --> |$-0.04| Wise円
  %%Wise円 --> |-200円| Kyash
  ```
  
## 使えないもの

```
- FamiPay -> Kyash #塞がれた
- "Shuttle Pay" -> Revolut 塞がれた
- dカードプリペイド -> "6gram" #塞がれた
- TOYOTAWallet -> 楽天Edy #塞がれた
- "6gram" -> Revolut #できない(6gramが悪い)
- "6gram" -> TOYOTAWallet #できない(6gramが悪い)
- "6gram" -> Kyash #できない(kyashが悪い)
- "6gram" -> "Shuttle Pay" #塞がれた
- "6gram" -> ARIGATO #塞がれた
- "B/43" -> Revolut #できない
- TOYOTAWallet -> Kyash #できない
- TOYOTAWallet -> "6gram" [label="+1%",color="red",fontcolor="red"] #塞がれた
- TOYOTAWallet -> "B/43" #塞がれた
- TOYOTAWallet -> 楽天Edy #塞がれた
- TOYOTAWallet -> nanaco #塞がれた
- TOYOTAWallet -> WAON #塞がれた
- Revolut -> TOYOTAWallet #できない
- Revolut -> Kyash #できない
- Revolut -> "6gram" #塞がれた
- Revolut -> IDARE #塞がれたっぽい
- TOYOTAWallet -> Revolut #できない
- TOYOTAWallet -> auPay #できない
- auPay -> TOYOTAWallet [label="+0.5%",color="red",fontcolor="red"] #塞がれた
- LINEPayVisa -> auかんたん決済 #塞がれた
- 6gram --> nanaco 塞がれた
- 6gram --> WAON
```
