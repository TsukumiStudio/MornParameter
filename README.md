# MornParameter

## 概要

Inspectorからパラメータを定数/カーブ/ランダムで簡単に設定できるようになるライブラリ。

## 依存関係

| 種別 | 名前 |
|------|------|
| 外部パッケージ | なし |
| Mornライブラリ | なし |

## 使い方

### 基本的な使用方法

```csharp
[SerializeField] private MornParameterFloat _float1;
[SerializeField] private MornParameterInt _int1;

private void Hoge()
{
    Debug.Log(_float1.Value);
    Debug.Log(_int1.Value);
}
```

### パラメータモード

| モード | 説明 |
|--------|------|
| Constant | 固定値 |
| Curve | AnimationCurveから値を取得 |
| RandomBetweenTwoConstants | 最小値〜最大値で乱数 |
