
port: 7890
socks-port: 7891
allow-lan: true
mode: Rule
log-level: info
external-controller: :9090
proxies:
  - {name: 🇸🇬 EPIC_新加坡1, server: sg.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇸🇬 EPIC_新加坡2, server: sg2.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇸🇬 EPIC_新加坡3, server: sg3.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇩🇪 EPIC_德国, server: de2.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇺🇸 EPIC_美国, server: us1.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇺🇸 EPIC_美国2, server: sf3.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇬🇧 EPIC_英国1, server: uk.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇬🇧 EPIC_英国2, server: uk2.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇬🇧 EPIC_英国3, server: vd2.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇫🇷 EPIC_法国1, server: fr.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇫🇷 EPIC_法国2, server: fr2.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇫🇷 EPIC_法国3, server: fr3.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇳🇱 EPIC_荷兰1, server: ne.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇳🇱 EPIC_荷兰2, server: ne2.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇳🇱 EPIC_荷兰3, server: ne3.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇮🇳 EPIC_印度1, server: ne.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇮🇳 EPIC_印度2, server: ne2.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇮🇳 EPIC_印度3, server: ne3.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇨🇦 EPIC_加拿大1, server: ca.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇨🇦 EPIC_加拿大2, server: ca2.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
  - {name: 🇨🇦 EPIC_加拿大3, server: ca3.epicbrowser.net, port: 8888, type: http, tls: true, skip-cert-verify: false, udp: true}
proxy-groups:
  - name: 🚀 节点选择
    type: select
    proxies:
      - ♻️ 自动选择
      - DIRECT
      - 🇸🇬 EPIC_新加坡1
      - 🇸🇬 EPIC_新加坡2
      - 🇸🇬 EPIC_新加坡3
      - 🇩🇪 EPIC_德国
      - 🇺🇸 EPIC_美国
      - 🇺🇸 EPIC_美国2
      - 🇬🇧 EPIC_英国1
      - 🇬🇧 EPIC_英国2
      - 🇬🇧 EPIC_英国3
      - 🇫🇷 EPIC_法国1
      - 🇫🇷 EPIC_法国2
      - 🇫🇷 EPIC_法国3
      - 🇳🇱 EPIC_荷兰1
      - 🇳🇱 EPIC_荷兰2
      - 🇳🇱 EPIC_荷兰3
      - 🇮🇳 EPIC_印度1
      - 🇮🇳 EPIC_印度2
      - 🇮🇳 EPIC_印度3
      - 🇨🇦 EPIC_加拿大1
      - 🇨🇦 EPIC_加拿大2
      - 🇨🇦 EPIC_加拿大3
  - name: ♻️ 自动选择
    type: url-test
    url: http://www.gstatic.com/generate_204
    interval: 300
    tolerance: 50
    proxies:
      - 🇸🇬 EPIC_新加坡1
      - 🇸🇬 EPIC_新加坡2
      - 🇸🇬 EPIC_新加坡3
      - 🇩🇪 EPIC_德国
      - 🇺🇸 EPIC_美国
      - 🇺🇸 EPIC_美国2
      - 🇬🇧 EPIC_英国1
      - 🇬🇧 EPIC_英国2
      - 🇬🇧 EPIC_英国3
      - 🇫🇷 EPIC_法国1
      - 🇫🇷 EPIC_法国2
      - 🇫🇷 EPIC_法国3
      - 🇳🇱 EPIC_荷兰1
      - 🇳🇱 EPIC_荷兰2
      - 🇳🇱 EPIC_荷兰3
      - 🇮🇳 EPIC_印度1
      - 🇮🇳 EPIC_印度2
      - 🇮🇳 EPIC_印度3
      - 🇨🇦 EPIC_加拿大1
      - 🇨🇦 EPIC_加拿大2
      - 🇨🇦 EPIC_加拿大3
  - name: 🌍 国外媒体
    type: select
    proxies:
      - 🚀 节点选择
      - ♻️ 自动选择
      - 🎯 全球直连
      - 🇸🇬 EPIC_新加坡1
      - 🇸🇬 EPIC_新加坡2
      - 🇸🇬 EPIC_新加坡3
      - 🇩🇪 EPIC_德国
      - 🇺🇸 EPIC_美国
      - 🇺🇸 EPIC_美国2
      - 🇬🇧 EPIC_英国1
      - 🇬🇧 EPIC_英国2
      - 🇬🇧 EPIC_英国3
      - 🇫🇷 EPIC_法国1
      - 🇫🇷 EPIC_法国2
      - 🇫🇷 EPIC_法国3
      - 🇳🇱 EPIC_荷兰1
      - 🇳🇱 EPIC_荷兰2
      - 🇳🇱 EPIC_荷兰3
      - 🇮🇳 EPIC_印度1
      - 🇮🇳 EPIC_印度2
      - 🇮🇳 EPIC_印度3
      - 🇨🇦 EPIC_加拿大1
      - 🇨🇦 EPIC_加拿大2
      - 🇨🇦 EPIC_加拿大3
  - name: 📲 电报信息
    type: select
    proxies:
      - 🚀 节点选择
      - 🎯 全球直连
      - 🇸🇬 EPIC_新加坡1
      - 🇸🇬 EPIC_新加坡2
      - 🇸🇬 EPIC_新加坡3
      - 🇩🇪 EPIC_德国
      - 🇺🇸 EPIC_美国
      - 🇺🇸 EPIC_美国2
      - 🇬🇧 EPIC_英国1
      - 🇬🇧 EPIC_英国2
      - 🇬🇧 EPIC_英国3
      - 🇫🇷 EPIC_法国1
      - 🇫🇷 EPIC_法国2
      - 🇫🇷 EPIC_法国3
      - 🇳🇱 EPIC_荷兰1
      - 🇳🇱 EPIC_荷兰2
      - 🇳🇱 EPIC_荷兰3
      - 🇮🇳 EPIC_印度1
      - 🇮🇳 EPIC_印度2
      - 🇮🇳 EPIC_印度3
      - 🇨🇦 EPIC_加拿大1
      - 🇨🇦 EPIC_加拿大2
      -
