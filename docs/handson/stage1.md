---
title: Stage1
permalink: /handson/stage1/
---

(File)-(New Scene)を選択して、新しいシーンを作成してください。
(File)-(Save As)を選択して、ScenesフォルダにStage1.unityとして保存してください。


# 1. カメラ設定

- Hierarchy内のMain Cameraを削除
- Projectタブの検索エリアにCameraRigと入力
- 検索エリア直下のSearch:からAllを選択
- OVRCameraRigをHierarchyにドラッグ&ドロップ

OVR Managerの設定
- Hierarchy内のOVRCameraRigを選択
- Inspector内のOVR Manager(Component)を確認
- Tracking Origin TypeをFloor Levelに設定


# 2. コントローラの設定
- Projectタブの検索エリアにOVRInteractionComprehensiveと入力
- 検索エリア直下のSearch:からAllを選択
- OVRInteractionComprehensiveをOVRCameraRigにドラッグ&ドロップで子要素として追加
<img src="{{ site.baseurl }}/handson/asset/stage1/image.png" alt="alt text" width="400" style="display:block; margin:0;">

**ハンドトラッキングの設定**
- Hierarchy内のOVRCameraRigを選択
- Inspector内のOVR Manager(Component)を確認
- Hand Tracking SupportをControllers and Handsに設定

<img src="{{ site.baseurl }}/handson/asset/stage1/image-1.png" alt="alt text" width="400" style="display:block; margin:0;">


**ControllerのRay表示**

(OVRInteractionComprehensive)-(LeftInteractions)-(Interactors)-(Cntroller)-(ControllerRayInteractor)-(Visuals)-(ControllerRay)を選択
<img src="{{ site.baseurl }}/handson/asset/stage1/image-2.png" alt="alt text" width="400" style="display:block; margin:0;">
Inspectorで**Controller Ray Visual**の**Hide WHen No Interactable**のチェックをOFFに設定
<img src="{{ site.baseurl }}/handson/asset/stage1/image-3.png" alt="alt text" width="400" style="display:block; margin:0;">


# 3. Cubeの配置
- Hierarchy内で右クリック-(3D Object)-(Cube)を選択してCubeを配置
- CubeのTransformを以下のように設定
  - Position: (0, 1, 3)
  - Scale: (0.2, 0.2, 0.2)


　**注意**: OvrCameraRigの位置が(0,0,0)に設定