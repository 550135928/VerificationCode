# VerificationCode

# Swift4.0
> pod 'VerifyCodeSwift' -> , '~>2.0'

# Swift5.0
> pod 'VerifyCodeSwift' -> , '~>3.0'


### 支持swift4.0以下的
#### 依赖于SnapKit
##### 下载完成后需要pod install

## 工具类
![工具类.jpg](https://upload-images.jianshu.io/upload_images/2094754-d0116e762526d75f.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 依赖的方法、可以使用自己项目的方法替换
![依赖类.jpg](https://upload-images.jianshu.io/upload_images/2094754-7d23542eb01f6de1.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


## 效果：
![验证码输入Demo.gif](https://upload-images.jianshu.io/upload_images/2094754-768de1c89184e230.gif?imageMogr2/auto-orient/strip)


## 思路：
视图层级：


- 最底层一个隐藏的UITextView，上面铺的Label

- 输入焦点在UITextView，监听UITextView的输入，给Label赋值

- 通过Label显示输入的文字使用CAShapeLayer绘制光标

- 通过光标的显示隐藏来控制光标的移动

- 基础动画控制光标闪动



## 使用：
          // 初始化验证码输入框数量
        let codeView = TDWVerifyCodeView.init(inputTextNum: 6)
    
         // 监听验证码输入的过程
        codeView.textValueChange = { [weak self] str in
            // 要做的事情
        }
        
        // 监听验证码输入完成
        codeView.inputFinish = { [weak self] str in
            // 要做的事情
        }
###


#### 简书链接：
#### https://www.jianshu.com/p/d258714f7095

## 喜欢的点个star，谢谢老铁们

