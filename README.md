# overview
1. Bake animations multiple prefabs to textures
2. Using next frame for linear translation (low fps, less texture size)
3. Use job systems for calculate animation time
4. Use Unity Entities 1.0.0-pre.15 / Graphics 1.0.0-pre.15 / Burst 1.7.4
5. InstanceShader build in shadergraph only for URP (14.0) 

# generation window
> <img src="https://raw.githubusercontent.com/igor-karpushin/com.sniveler-code.gpu-animation/main/Images/AnimationGenerator.jpg" width="400">

1. Batch Name => Name for multiple prefabs 
2. Each Prefab must have one SkinnedMeshRenderer and AnimatorController
3. First Animation (animation index == 0) is T Pose
4. All diffuse textures packed in one (normals/speculars/other in develop)
5. LODS in developing state 
