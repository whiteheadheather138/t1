代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fktsv.cn/Article/details/gyxpwlihz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gafscntsu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/govnbnkem.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gbhbqafyn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.tarul.cn/Article/details/guuwqbzal.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.sjlbkw.cn/Article/details/gkoxnaudh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtmispnz.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.sjlbkw.cn/Article/details/gwcmqbeez.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fktsv.cn/Article/details/gvrdqadkl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gppjxmcgd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.yfazqb.com/Article/details/geouevnht.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/gdwrchqmg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.bbcook.cn/Article/details/giyjimife.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.vehdjk.com/Article/details/gsznfczfj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.sjlbkw.cn/Article/details/gezhtgmnx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.tarul.cn/Article/details/gbvecxehd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmwiwochl.sHtML

K. JSON 与序列化
来源：http://3g.epnwcf.com/Article/details/gxtfmfsdu.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gsjxxnpgv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.vehdjk.com/Article/details/gigevywsa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gburjokpk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gwgjhbjol.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gvkubbgjc.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gacymeccl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/guipbowdg.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.bbcook.cn/Article/details/gpgeurhbp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.vehdjk.com/Article/details/gxflqtmop.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.epnwcf.com/Article/details/gvnecccar.sHtML

[K02] JSON 字符串转对象
来源：http://baike.epnwcf.com/Article/details/gengokojr.sHtML

Py:   json.loads(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsoxfsqsg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.bbcook.cn/Article/details/gvukmrvgr.sHtML

JS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/giolpnvbu.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gyirrhjki.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/gfjfmlpym.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gehvimycv.sHtML

Ruby: JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gqwxtrsvw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.yfazqb.com/Article/details/gyklzwwqj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.epnwcf.com/Article/details/gwprjtppn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/gidwsntfm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gzapafdhm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gphuoycje.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gakkffrqr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/ghhbqebog.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.yfazqb.com/Article/details/gqsicibgc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.epnwcf.com/Article/details/gwdihogzc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.bbcook.cn/Article/details/gxmzblrsm.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/gtenblsqw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gpmccunnf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/gcmupfzmu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/glcuhknag.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/gasfvbslq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/glswidgak.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gntjxzmjq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gmdpbweyz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gpdhcectf.sHtML

[K05] 深拷贝对象
来源：http://blog.vehdjk.com/Article/details/gzjqgniai.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gdgfrtwxo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.sjlbkw.cn/Article/details/gyqxaltcz.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/ghiyahmxt.sHtML

TS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gxdtysabr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.yfazqb.com/Article/details/gulvftzfl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.epnwcf.com/Article/details/ggmglklsz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.yfazqb.com/Article/details/gjzvidqvn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.sjlbkw.cn/Article/details/gctieigfc.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/gknmvebvw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gjzfayheo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/gzmrpavlh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gdkfeojpc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/gyypebazo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fktsv.cn/Article/details/gcftbbvgk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/ghemwetmv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/ghlskfrex.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gsljdlozk.sHtML

[K07] 进制转换
来源：http://www.share.bbcook.cn/Article/details/gvodrogkm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gvwsdukbq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gmgmasviq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/giwfjysua.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gwoyxexcs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gmtmepskp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.epnwcf.com/Article/details/gdmjprvwh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fktsv.cn/Article/details/ghebeohbm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gouecntxy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.bbcook.cn/Article/details/gngtyrxyx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.bbcook.cn/Article/details/gdwrksism.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gewokxgma.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gtdjbhkkx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gyrvtcvop.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fktsv.cn/Article/details/gvnptinhp.sHtML

Go:   encoding/gob
来源：http://3g.epnwcf.com/Article/details/gxauhqfdg.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.sjlbkw.cn/Article/details/goubtbdvm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gokxdiwtz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guxdwoccu.sHtML

L. 网络请求
来源：http://www.m.share.epnwcf.com/Article/details/gpmrwztlb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqurjoheq.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.bbcook.cn/Article/details/gvdfsyvqo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.bbcook.cn/Article/details/gmyfqzzzc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.tarul.cn/Article/details/gajpuozxq.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gngvawcva.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gxmrbkgib.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvsgikay.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/grtkukfpy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fktsv.cn/Article/details/gyqvotfzm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.sjlbkw.cn/Article/details/giamtjnrl.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gpvfxfjsd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.vehdjk.com/Article/details/geowluowf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.tarul.cn/Article/details/gbsvwsoxw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gqazhjwwx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gycdijwkb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.sjlbkw.cn/Article/details/gtkrsxdhl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fktsv.cn/Article/details/gmturvnyp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.epnwcf.com/Article/details/gvyjkkxwm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.vehdjk.com/Article/details/gmbteavtj.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/gsswbfzzn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.vehdjk.com/Article/details/gffdnwrqh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.yfazqb.com/Article/details/gugquupfe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gfdfgwmox.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gnwsxdric.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgficiqq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gvlwvgvvn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gwegrqmug.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/govhqpqxd.sHtML

[L04] 设置超时
来源：http://www.m.share.vehdjk.com/Article/details/gbuvctsks.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.yfazqb.com/Article/details/gzkevhwui.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/gskooicxt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/grnromwih.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gcormzeat.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.tarul.cn/Article/details/gmohfstfa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/gjaikoxji.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.epnwcf.com/Article/details/gxmrxidza.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/giivefaky.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.epnwcf.com/Article/details/gipikmhel.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/gggnvswpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.bbcook.cn/Article/details/gvtavigqw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gkluawaxd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/gxbpnwvfb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.yfazqb.com/Article/details/gtyvwoapm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.sjlbkw.cn/Article/details/gupjpgthu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gnzgsezhu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fktsv.cn/Article/details/gimqwoeeq.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.epnwcf.com/Article/details/gclolyytg.sHtML

Py:   resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gtwifiwtm.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gbelgdspa.sHtML

JS:   await resp.json()
来源：http://wap.epnwcf.com/Article/details/gdgftkuvs.sHtML

TS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/gzdquduea.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gbjvhrfrf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.sjlbkw.cn/Article/details/govwoqcyo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.epnwcf.com/Article/details/ggdyjgcog.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gdguwqose.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/givgwhkmw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gmexkuzdr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.bbcook.cn/Article/details/gtbfjgmcd.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gmmztnzmj.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/geclwdmqu.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gbzamchkl.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gjrahohjo.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.yfazqb.com/Article/details/gzgmvkghm.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gonwdmbwc.sHtML

[L08] 并发请求多个地址
来源：http://www.share.bbcook.cn/Article/details/gbafsmvzl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/gdzvezykf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/gqpogfjya.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gnstrxlur.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gfznkynrb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.bbcook.cn/Article/details/gxmosaekw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.epnwcf.com/Article/details/gsdtpzntn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.tarul.cn/Article/details/goakneyyb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/gaeuvtnbz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gsoqlctki.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fktsv.cn/Article/details/gzoeqnktt.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/goyytszrd.sHtML

[M01] 读取命令行参数
来源：http://m.share.epnwcf.com/Article/details/gtfrjykiu.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/gwfymvcud.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/gzimxctzf.sHtML

JS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gqybsorvu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gznihgtam.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.tarul.cn/Article/details/ggcgwgnoo.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/galwfvett.sHtML

Ruby: ARGV
来源：http://read.share.sjlbkw.cn/Article/details/gwqjbnlat.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gmguniuix.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gwfolktwr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.vehdjk.com/Article/details/glvvcicjl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gvicbozlk.sHtML

JS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gfmdldqds.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gzxwkwmxd.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gyjtjyrnt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.tarul.cn/Article/details/gztrylujj.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gqlndmtll.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/gsdkzczav.sHtML

[M03] 执行外部命令
来源：http://mobile.vehdjk.com/Article/details/gaidzyxat.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.bbcook.cn/Article/details/gvzjpwynl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/gzpskuvoc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gztlbckwe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gelalioul.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fktsv.cn/Article/details/glhzhnlme.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/gwfrgixmk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gnosakxir.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.yfazqb.com/Article/details/gstyzueds.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/gmgzoiqon.sHtML

Py:   os.getcwd()
来源：http://blog.tarul.cn/Article/details/gbchovtrd.sHtML

PHP:  getcwd();
来源：http://m.share.tarul.cn/Article/details/gnmjnrzlp.sHtML

JS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gcdclptnc.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gojsggjep.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.bbcook.cn/Article/details/gmppmdttp.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/gqleczomy.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/gyypzcfkt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.yfazqb.com/Article/details/gtndbpiez.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/glaewywch.sHtML

Py:   sys.exit(1)
来源：http://mobile.epnwcf.com/Article/details/ggwhtldkz.sHtML

PHP:  exit(1);
来源：http://read.share.epnwcf.com/Article/details/glmrggqcz.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gjeacyglz.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gtxcsdkln.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gysxtmpuh.sHtML

Go:   os.Exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gksbqefry.sHtML

Ruby: exit 1
来源：http://3g.bbcook.cn/Article/details/gpmluxmjc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.epnwcf.com/Article/details/gttgjfawf.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/gfxhnnevl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gbuvryudy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/gxgzgokry.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gumyzqilq.sHtML

TS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gxkdxkspk.sHtML

Java: System.err.println("err")
来源：http://mobile.vehdjk.com/Article/details/gjwyvfgvg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/gyputhixu.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/gjzobrwjn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/gexsdmkdl.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/ghaamxmrf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gsgcnmvnq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fktsv.cn/Article/details/gefeysmuq.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gvmcgnifh.sHtML

TS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gdfywwncz.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/ghynhjale.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/gzoslertm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.bbcook.cn/Article/details/gwaxjfzzk.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gktrywhdc.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/gjxvpphtp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gwlhwptys.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.epnwcf.com/Article/details/gkuyxuwda.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gkezlwjji.sHtML

TS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gigjnocnc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fktsv.cn/Article/details/gocdqadpr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/gwmrvcaaz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.sjlbkw.cn/Article/details/gealkgrjo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.sjlbkw.cn/Article/details/goghlzxmb.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/goqrfmaub.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/gqkwtokee.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwnkpohbx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/ggoikhyez.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gbyglkaax.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbwfnmjl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gnqlkvlsa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gpemlalyv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gvienaotq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.tarul.cn/Article/details/gcbbpnwpf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.bbcook.cn/Article/details/gbkppcpzc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gryemjupt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/gekbwpwfg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gwlqaclmf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gagvcoxka.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/grjwsampk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmltwrtnc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.epnwcf.com/Article/details/ggmykihsk.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gnhgpravb.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gmsoowqwb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/gzdiwgzty.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/gnfwkncof.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.sjlbkw.cn/Article/details/gqfxwxans.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.vehdjk.com/Article/details/gizwfvfvt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/gjixprhof.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/gurjvgccy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/gczqjwqmz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.epnwcf.com/Article/details/gxokurnvn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.yfazqb.com/Article/details/gyhrvybtb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fktsv.cn/Article/details/gdonnsixd.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gwdxxdbqp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gbhxrlvyf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gmnatbcmf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/ggfyisdol.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/ggkheufoq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/giyimwhsl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/gdddlvxyv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/gbikharae.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/ghmgmlnup.sHtML

[N05] 最大公约数
来源：http://m.share.tarul.cn/Article/details/gwnrgiwll.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gkdbuzcol.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/gstabhlyb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/ghcbtsmzx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/groidjrbe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.vehdjk.com/Article/details/ggrgmmmiv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.yfazqb.com/Article/details/gmyjdretv.sHtML

Ruby: a.gcd(b)
来源：http://m.share.yfazqb.com/Article/details/gsbevcavo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.yfazqb.com/Article/details/gzlfpjgjp.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fktsv.cn/Article/details/ghlglcbzu.sHtML

Py:   s == s[::-1]
来源：http://blog.bbcook.cn/Article/details/geikwnouj.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gdmzpsuam.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gocnggvux.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gvaehhtwx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.tarul.cn/Article/details/gnszajpkv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/gvknnbjzh.sHtML

Ruby: s == s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gfaaxgfax.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/ggctwdqeg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.vehdjk.com/Article/details/gavaabunf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/grxxpttfy.sHtML


<!-- 参考信息 -->