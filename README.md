# MSI B450M MORTAR MAX (MS-7B89)

使用 Open Core 引导  系统版本 macOS 10.15.2

+ 具体配置：

        处理器 : AMD 3600 
 
        显卡 : AMD Radeon RX 580 8G
    
        内存 :16G DDR4 2666
    
+ 达芬奇导出视频对比实测

    >系统版本 : macOS 10.15.2 AMD_Vanilla
    >
        软件版本 :DaVinci Resolve 16
    
        原始素材 : mp4 h.264 01:40:39 1080p 50fps 50m 
    
        导出视频 : mp4 1080p 50fps 6000kb 

        编码 : h.264 完成时间 : 01:25

        编码 : h.265 完成时间 : 00:43

        编码 : h.264 开启硬件加速 完成时间 : 01:20

    
    >系统版本 : Windows 10 1909
    >
        软件版本 :DaVinci Resolve 16

        原始素材 : mp4 h.264 01:40:39 1080p 50fps 50m 

        导出视频 : mp4 1080p 50fps 6000kb 

        编码 : h.264 原生 完成时间 : 00:54

        编码 : h.265 AMD 完成时间 : 00:28

        编码 : h.264 AMD 完成时间 : 00:48

+ GeekBench 跑分

    > Geekbench 4 

    - Windowns 10 1909

            CPU 单核 5319 多核 26963  https://browser.geekbench.com/v4/cpu/     15066532

            GPU 138227 https://browser.geekbench.com/v4/compute/4677679

    - macOS 10.15.2 AMD_Vanilla
            
            CPU 单核 5595 多核 29783  https://browser.geekbench.com/v4/cpu/15066696

            GPU 122623   https://browser.geekbench.com/v4/compute/4677747

    > Geekbench 5

    - Windowns 10 1909

            CPU 单核 1207 多核 6890 https://browser.geekbench.com/v5/cpu/861352
    
            GPU 48759 https://browser.geekbench.com/v5/compute/363947
    
    - macOS 10.15.2 AMD_Vanilla

            CPU 单核 1230 多核 6898 https://browser.geekbench.com/v5/cpu/861892

            GPU 33202 https://browser.geekbench.com/v5/compute/364190

