# 随屏元素使用 旋转 平移 缩放 动画,设置参数时注意事项

# 随屏元素添加 RTS 动画 必须设置在父节点下,父节点设置随屏,子节点 RPS 参数初始设置为 0,0,0 (根据需要调整)


 [ 旋转 ]
 暂无注意事项


 [ 缩放 ]
 1. from(Vector3(0.1, 0.1, 0.1)) ,to(Vector3(5, 5, 5)) 中参数为随屏占比值的倍数.


 [ 平移 ]
 1.平移时,x 轴方向 平移测试参数为1. (to(Vector3(1, 0, 0)))
 		 y 轴方向 平移测试参数为1. (to(Vector3(0, 1, 0)))

 2.注意: 改变父节点"screenRatio"参数,会影响元素显示大小,平移距离