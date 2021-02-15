About Clubhouse

#适用于quantumultX代理服务器不支持udp-relay添加，默认direct
#支持udp-relay的也需添加，默认direct,可自行修改策略偏好

#[policy]
#策略组
;static=Clubhouse, direct, proxy, img-url=https://raw.githubusercontent.com/tengyuankoo/qx/main/Clubhouse.png

#[filter_remote]
#远程分流规则，两条规则需同时添加搭配使用
#域名规则
;https://raw.githubusercontent.com/tengyuankoo/qx/main/Clubhouse.list, tag=Clubhouse, force-policy=Clubhouse, update-interval=86400, opt-parser=false, enabled=true
#IP规则
;https://raw.githubusercontent.com/tengyuankoo/qx/main/Clubhouse_IP.list, tag=Clubhouse_IP, force-policy=direct, update-interval=86400, opt-parser=false, enabled=true
