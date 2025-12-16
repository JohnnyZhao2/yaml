# yaml
rule-providers:
  AD:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/earoftoast/clash-rules/main/AD.yaml"
    path: ./rules/AD.yaml
    interval: 86400
    
  EasyList:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/earoftoast/clash-rules/main/EasyList.yaml"
    path: ./rules/EasyList.yaml
    interval: 86400
    
  EasyListChina:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/earoftoast/clash-rules/main/EasyListChina.yaml"
    path: ./rules/EasyListChina.yaml
    interval: 86400

  EasyPrivacy:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/earoftoast/clash-rules/main/EasyPrivacy.yaml"
    path: ./rules/EasyPrivacy.yaml
    interval: 86400

  ProgramAD:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/earoftoast/clash-rules/main/ProgramAD.yaml"
    path: ./rules/ProgramAD.yaml
    interval: 86400

rules:
  - RULE-SET,AD,REJECT
  - RULE-SET,EasyList,REJECT
  - RULE-SET,EasyListChina,REJECT
  - RULE-SET,EasyPrivacy,REJECT
  - RULE-SET,ProgramAD,REJECT