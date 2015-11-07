
#Google Finance Stock API

##Request

`https://finance.google.com/finance/info?client=ig&q=TPE:2330`


##Response

###NOTE that "//" makes this not real JSON

```
// [ { "id": "674465" ,"t" : "2330" ,"e" : "TPE" ,"l" : "140.00" ,"l_fix" : "140.00" ,"l_cur" : "NT$140.00" ,"s": "0" ,"ltt":"1:30PM GMT+8" ,"lt" : "Nov 6, 1:30PM GMT+8" ,"lt_dts" : "2015-11-06T13:30:01Z" ,"c" : "-2.50" ,"c_fix" : "-2.50" ,"cp" : "-1.75" ,"cp_fix" : "-1.75" ,"ccol" : "chr" ,"pcls_fix" : "142.5" } ]
````

#Google App Engine Currency API

##Reqest

`https://currency-api.appspot.com/api/USD/TWD.json`

##Response

`{"success":true,"source":"USD","target":"TWD","rate":32.707001,"amount":32.71,"message":""}`

###//上方會有 server(resouce) no Access-Control-Allow-Origin 為 true 的 response header 設定，暫時改用 jsonp

##Request

`https://currency-api.appspot.com/api/USD/TWD.jsonp`

##Response

`Object {success: true, source: "JPY", target: "TWD", rate: 0.2655651, amount: 0.27, message: ""}`

###Reference: https://currency-api.appspot.com/