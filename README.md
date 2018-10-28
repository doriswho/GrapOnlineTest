# GrapOnlineTest
my solution

cases:
1.验证基本功能，填写全部参数（成功）  ①key=KEY,location=Denver,CO,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=true,thumbMaps=false,maxResults=5,outFormat=xml,delimiter=|,intlMode=1BOX,callback=geocodeResult
②key=KEY,location=Denver,CO,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=false,thumbMaps=false,maxResults=5,outFormat=xml,delimiter=|,intlMode=1BOX,callback=geocodeResult
③key=KEY,location=Denver,CO,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=false,thumbMaps=true,maxResults=5,outFormat=xml,delimiter=|,intlMode=1BOX,callback=geocodeResult
④key=KEY,location=Denver,CO,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=true,thumbMaps=false,maxResults=5,outFormat=csv,delimiter=|,intlMode=1BOX,callback=geocodeResult
⑤key=KEY,location=Denver,CO,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=true,thumbMaps=false,maxResults=5,outFormat=csv,delimiter=,,intlMode=1BOX,callback=geocodeResult
⑥key=KEY,location=Denver,CO,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=true,thumbMaps=false,maxResults=5,outFormat=csv,delimiter=:,intlMode=1BOX,callback=geocodeResult
⑦key=KEY,location=Denver,CO,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=true,thumbMaps=true,maxResults=5,outFormat=csv,delimiter=;,intlMode=1BOX,callback=geocodeResult
⑧key=KEY,location=Denver,CO,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=true,thumbMaps=false,maxResults=4,outFormat=csv,delimiter=;,intlMode=auto,callback=geocodeResult
⑨key=KEY,location=Denver,CO,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=true,thumbMaps=false,maxResults=5,outFormat=csv,delimiter=;,intlMode=5BOX,callback=geocodeResult
2.缺少可选项，只填写必填参数（成功）
①key=KEY,location=Denver,CO,boundingBox=,ignoreLatLngInput=,thumbMaps=,maxResults=,outFormat=,delimiter=,intlMode=,callback=
3.缺少必填参数（失败：缺少必填参数）
①key=,location=Denver,CO,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=true,thumbMaps=false,maxResults=5,outFormat=csv,delimiter=;,intlMode=5BOX,callback=geocodeResult
②key=KEY,location=,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=true,thumbMaps=false,maxResults=5,outFormat=csv,delimiter=;,intlMode=5BOX,callback=geocodeResult
③key=,location=,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=true,thumbMaps=false,maxResults=5,outFormat=csv,delimiter=;,intlMode=5BOX,callback=geocodeResult
4.参数越界（失败：参数异常）
①key=KEY,location=Denver,CO,boundingBox=91,-181,90.5,-180.5,ignoreLatLngInput=true,thumbMaps=false,maxResults=5,outFormat=xml,delimiter=|,intlMode=1BOX,callback=geocodeResult
②key=KEY,location=Denver,CO,boundingBox=40.099998,-77.305603,39.099998,-75.305603,ignoreLatLngInput=true,thumbMaps=false,maxResults=5,outFormat=xml,delimiter=|,intlMode=1BOX,callback=geocodeResult
5.改变参数数值类型（失败：错误的参数类型）
6.场景模拟

  
