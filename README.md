# MSI B450M MORTAR MAX (MS-7B89)

## rEFInd → Open Core 0.5.2 → macOS 10.15.2

> 同步更新地址：https://shiyangyu.com/b450m-mortar-hackintosh/

## 更新日志

 + 2020.01.16 更新EFI 添加rEFInd多系统引导
 
      具体使用说明： https://github.com/techysy/rEFInd
        
      当然你也可以使用Open Core添加自定义引导

  ![EFI](/ScreenShot/EFI.jpg) 

 + 2019.12.23 首次提交
        
## 具体配置：

        处理器 : AMD® Ryzen5 3600 （电压-0.05v 运行 迫击炮默认电压太高）
 
        显卡 : AMD® Radeon RX 580 8G （硬解可用）
    
        内存 : 16G DDR4 2666 （光威® 2 * 8g  2400 c17 → 2666 c18 ）
        
        网卡 : Realtek® RTL8111H-CG
        
        无线 : BCM943602CS (免驱 蓝牙+2.4G+5G 都可用)

        声卡 : Realtek® ALC892 Codec
    
## 已知bug：

        3.5mm 麦克风🎤 没声音 （目前解决方案外置USB免驱声卡）

        3.5mm 🎧耳机还是走面板或者主板

        Windows下声卡那个UWP驱动（Realtek Audio Console）也不好用 感觉不是常驻后台 
        
  ~~直接插耳机🎧 麦克风🎤系统不会识别 需要打开这个软件再插~~

  ~~音质木耳都能听出区别 也可能是推力不够 外置声卡音量相对也要小一些 可能算我钱没给够~~
  
  ~~所以还是开UWP在插吧 迫击炮这个系列都会有 B250M（IU） 我也遇到过~~
  
## 达芬奇导出视频对比实测

   + 原始素材 : mp*4* h.*264* *1080*p *50*fps *50*m *01:40:39*
    
   + 导出视频 : mp*4* *1080*p *50*fps *6000*kb 

> macOS 10.15.2 AMD_Vanilla + DaVinci Resolve 16
   
        编码 : h.264 完成时间 : 01:25

        编码 : h.265 完成时间 : 00:43

        编码 : h.264 开启硬件加速 完成时间 : 01:20
        
![md](/ScreenShot/macOS_达芬奇导出页面.jpg)
    
> Windows 10 1909 + DaVinci Resolve 16
      
        编码 : h.264 原生 完成时间 : 00:54

        编码 : h.265 AMD 完成时间 : 00:28

        编码 : h.264 AMD 完成时间 : 00:48

![md](/ScreenShot/Windows_达芬奇导出页面.png)

## Geekbench 跑分

### Geekbench 4 

> macOS 10.15.2 AMD_Vanilla
            
        CPU 单核 5595 多核 29783  

        https://browser.geekbench.com/v4/cpu/15066696

        GPU 122623   
        
        https://browser.geekbench.com/v4/compute/4677747

> Windowns 10 1909

        CPU 单核 5319 多核 26963  
        
        https://browser.geekbench.com/v4/cpu/    15066532

        GPU 138227
        
         https://browser.geekbench.com/v4/compute/4677679

### Geekbench 5
    
> macOS 10.15.2 AMD_Vanilla

        CPU 单核 1230 多核 6898 
          
        https://browser.geekbench.com/v5/cpu/861892

        GPU 33202 
            
        https://browser.geekbench.com/v5/compute/364190

> Windowns 10 1909

        CPU 单核 1207 多核 6890 
            
        https://browser.geekbench.com/v5/cpu/861352
    
        GPU 48759 
            
        https://browser.geekbench.com/v5/compute/363947

## Cinebench R20  

> macOS 10.15.2 AMD_Vanilla

![mr](/ScreenShot/macOS_Cinebench_R20_跑分结果.jpg)


> Windowns 10 1909

![wr](/ScreenShot/Windows_Cinebench_R20_跑分结果.png)

## VideoProc 硬件加速检测

![hevc](/ScreenShot/VideoProc_硬解.jpg)
