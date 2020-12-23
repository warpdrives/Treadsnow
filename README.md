# Treadsnow
iOS traceless buried point solution, support objc/swift

埋点自动化，真正无侵入（objc-runtime，swift-protocol extension)
• 提供类名、方法名、参数key-value（objc-value在方法触发时，从类实例对象中动态获取，swift-value在协议中编译期直接引用，容错兜底处理）
• 维护一个埋点注册表（注册表为objc-superClass-category，swift-superClass/superStrcut-protocol，基于基类/协议自由扩展），启动时注册
• Debug调试检测输出，埋点成功/失败、上传服务器状态
