# depthkit-builtin-rp-vfx-template
Depthkit Studioコンテンツ取り込み用のプロジェクトテンプレート（Built-in Rendering Pipeline・VFX対応版）

VFX Graphは公式にはBuilt-in Renderingに対応していないが、無理やり対応させている[こちら](https://github.com/LastAbyss/unity-visualeffectgraph-builtin)のライブラリを使用している。

## Depthkitコンテンツの取り込み方
### サンプルシーンでの使い方
1. Scenes/SampleSceneを開く
2. `Props/Room1/Depthkit Clip + Studio VFX Look` と `Props/Room1/Depthkit Clip + Studio Shader Graph Look` がそれぞれVFX用のオブジェクト・そのまま表示用のオブジェクトです。
3. 自分のコンテンツと差し替える場合、InspectorのDepthkit Clip -> MetadataをDepthkitから書き出されたJSONファイルに差し替え、Video Player->Video ClipをDepthkitから書き出された動画ファイルに差し替えます。Depthkit Clip -> Posterを、動画から書き出した画像に差し替えると、Unity再生中でなくてもDepthkitでの再生された様子をプレビューできます。Poster項目はセットしなくても問題ないです。

### 新規シーンでの使い方
1. VFXを使う場合
Assets/Samples/Depthkit Studio Visual Effect Graph/0.4.2/Prefabs - Depthkit Studio Visual Effect Graph/Depthkit Clip + Studio VFX Look.prefab
をシーンにドラッグ&ドロップ
Depthkit Clip -> Metadata とVideo Player->Video Clipをセット。Depthkit Clip -> Posterもあればセット。

2. VFXでなくそのまま表示する場合
Assets/Samples/Depthkit Studio Shader Graph/0.4.2/Prefabs - Depthkit Studio Shader Graph/Depthkit Clip + Studio Shader Graph Look.prefab
をシーンにドラッグ&ドロップ
Depthkit Clip -> Metadata とVideo Player->Video Clipをセット。Depthkit Clip -> Posterもあればセット。
