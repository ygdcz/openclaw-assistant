# openclaw-assistant
openclaw (clawbot) workspace

1. 配置允许的origins：     // 可跳过                                                                                               
  openclaw config set gateway.controlUi.allowedOrigins '["http://localhost:18789", "http://127.0.0.1:18789"]'               
                                                                                                                            
2. 启动OpenClaw：                                                                                                         
openclaw gateway --port 18789
                                                                                                                        
启动后，保持Codespace终端运行，然后：                                                                                     
                                                                                                                        
3. 在你的本地电脑终端运行SSH隧道：
gh codespace ssh -- -N -L 18789:127.0.0.1:18789

4. 在浏览器打开：
http://localhost:18789/#token=113a564b1d310833c7bf09fb351b477de48e5a9cdae006fc

这样应该就能正常访问OpenClaw的Dashboard了。
