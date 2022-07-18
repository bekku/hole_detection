# 車道における陥没穴検出の実験
陥没穴の検出を行う物体検出モデルを構築する。
主に、API構築のための性能評価と仮実装を行う。

## hole+
マンホールや溝の誤検出を減らすために、アノテーションの種類を増やした物体検出モデル

## セグメンテーション + hole+ 性能評価
車道上に限定して、陥没穴の検出を行う。
セグメーてションモデルで車道上を検出し、車道外を黒でマスクする。

※ : 性能評価のためにval.pyを置き換える。

## セグメンテーション + hole+ to API
陥没穴検出APIのための結合

## CAOD：class agnostic object detection
車道上に限定したクラスを無視した物体検出である。
