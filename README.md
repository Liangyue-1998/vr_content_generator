# vr_content_generator

1. https://developer.picoxr.com/zh/document/unity/create-a-developer-account-organization-and-app/
2. Unity hub version 3.11.1
3. Unity editor version 2022.3.29f1

4. ![image](https://github.com/user-attachments/assets/6e3ec543-8cd1-4ba8-b708-9bef9280f2d0)
5. ![image](https://github.com/user-attachments/assets/0b914031-4359-4399-949e-3ca22171eb96)
6. ![image](https://github.com/user-attachments/assets/90168588-653a-4fb3-a974-05568c9d146a)
7. ![image](https://github.com/user-attachments/assets/c884e487-486b-4421-9965-48fb77edcc3e)


## Panorama
![image](https://github.com/user-attachments/assets/ef1068e6-62f9-4fef-bb8d-7b1900fc342c)
![image](https://github.com/user-attachments/assets/7cb715d2-9945-4f14-890e-856e91e1db58)

#### 将全景图拖入Assets，右键图片：

Texture Shape > 2D（部分版本需选Default）

Wrap Mode > Clamp（防止接缝）

#### 创建材质球：

右键Assets > Create > Material（命名如PanoramaMat）

#### Shader选择：
- 或Pico SDK提供的VR Panorama Shader（若有）
将全景图拖到材质球的对应插槽（6 Sided模式需拖到Front）

#### 场景配置
删除或禁用默认的Main Camera
添加Pico VR相机：
从Pico SDK预制体拖入PXR_SDK/Prefabs/PXR_InteractionCameraRig

#### 设置天空盒：
Window > Rendering > Lighting
Environment > Skybox Material 选择你的全景材质
