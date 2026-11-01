代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.vehdjk.com/Article/details/gyqyaspjp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gatwpxnfk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gjhjxjbnz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fktsv.cn/Article/details/gcoqvylqz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.bbcook.cn/Article/details/gwawghzic.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.epnwcf.com/Article/details/gnvrqpwmy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.tarul.cn/Article/details/gixdpacfq.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.yfazqb.com/Article/details/gksnzcypt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fktsv.cn/Article/details/gqxewktiq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.epnwcf.com/Article/details/gebothgza.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gmhewvuam.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/gkysrqnha.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.vehdjk.com/Article/details/gbctmgrmk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.vehdjk.com/Article/details/gvyyvgbob.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.epnwcf.com/Article/details/grhmysxds.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.epnwcf.com/Article/details/gaeftplxy.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/glkgmehre.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/gayvfuqcu.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gpbbftcui.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gwdffshwb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fktsv.cn/Article/details/gjalepjtl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/goesovasq.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/goacgpcir.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gywslnsmb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.yfazqb.com/Article/details/gezbwjose.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gzeiuscze.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gyndyeftg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/gfflaxart.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.vehdjk.com/Article/details/gvtnonloe.sHtML

Py:   json.loads(s)
来源：http://mobile.tarul.cn/Article/details/gfdltnjrm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.sjlbkw.cn/Article/details/gitfebmmy.sHtML

JS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gtscjdzcj.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gppyhmfqk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.epnwcf.com/Article/details/gxkstdywr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gbchrdzqm.sHtML

Ruby: JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gxmnqtnra.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.sjlbkw.cn/Article/details/ghoigmhrp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/gjeppcrub.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gkuvcflyr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fktsv.cn/Article/details/gokfhfiwc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gdrvslzyn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gfjcagjnr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gkbugigny.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/gdqzsnlsi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gftvhfqjy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.epnwcf.com/Article/details/glbynednx.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.bbcook.cn/Article/details/gqlaiyyul.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gfamnrimd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.tarul.cn/Article/details/gigvgotnd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/guzvntdvp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gebjkkzyr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsvqrecf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gendysysb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/ggezwrggt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gvigcgfnd.sHtML

[K05] 深拷贝对象
来源：http://www.share.epnwcf.com/Article/details/gppxjkawn.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.yfazqb.com/Article/details/gtgtdwexd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.epnwcf.com/Article/details/gzzuvfpts.sHtML

JS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gzzptpshg.sHtML

TS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gnihbqgwp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.yfazqb.com/Article/details/goqcafbxo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/gadvlcdah.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.bbcook.cn/Article/details/gogjlntjz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fktsv.cn/Article/details/gaxheftql.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fktsv.cn/Article/details/geqibrods.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gamqbggwo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.tarul.cn/Article/details/gycqqaued.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/grfjhijbh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gpmnxisvn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/gxbufosgk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gacftzvnh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/glluxmvnm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gjpnrifkb.sHtML

[K07] 进制转换
来源：http://read.share.vehdjk.com/Article/details/gqcitvydk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gazflcqyu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvvnooap.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gvyhtfutp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gtbattrrl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gqwtwqikz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.epnwcf.com/Article/details/gguajaelj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.sjlbkw.cn/Article/details/gdzwovojw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gpusthccw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gmhxxjxdj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/gaaqhjjqg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/geyqwkjsc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/gkolqdkpw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gbjlfypdk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/gdgvczjej.sHtML

Go:   encoding/gob
来源：http://baike.vehdjk.com/Article/details/gfzootiob.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.yfazqb.com/Article/details/gqmqoejog.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.epnwcf.com/Article/details/goiopeazx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbldrfpdk.sHtML

L. 网络请求
来源：http://blog.yfazqb.com/Article/details/gmintcsqt.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzoexckgf.sHtML

[L01] 发送 GET 请求
来源：http://www.share.tarul.cn/Article/details/gngirtqxl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gmxxsvpbx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.tarul.cn/Article/details/gukyajcog.sHtML

JS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gebquqknf.sHtML

TS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gfteuztca.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.bbcook.cn/Article/details/gynitydao.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.sjlbkw.cn/Article/details/gzukfyecy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.tarul.cn/Article/details/grgvonkjr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gyjmqhkxq.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/grajysydb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gpaivwamw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.sjlbkw.cn/Article/details/glrhqyiii.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gzcddbnfn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gtswxaoob.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fktsv.cn/Article/details/gxzbtqvku.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gflcyycjf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwffzrawo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.bbcook.cn/Article/details/gpalvovfu.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/gjovhwvke.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.yfazqb.com/Article/details/gbhbxoqgo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.vehdjk.com/Article/details/gynvdyetf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/glrjtzbba.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gxurqyyxe.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.sjlbkw.cn/Article/details/gscckkxcc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/giezqompd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/gvhrxjkxw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gmnsxwkkn.sHtML

[L04] 设置超时
来源：http://baike.fktsv.cn/Article/details/gciqxphot.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.yfazqb.com/Article/details/gcgkthqeu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/grnlkwepv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/guqunrkmo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gfwpefuvu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.sjlbkw.cn/Article/details/ggrbaenrl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.epnwcf.com/Article/details/goamfawuo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.yfazqb.com/Article/details/gwlzznfzx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.vehdjk.com/Article/details/gnitfxksi.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/gvzspvhmg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gbfoexzed.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.epnwcf.com/Article/details/gsvlnoiud.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gsovqnetd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/geubibkng.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.bbcook.cn/Article/details/gxcsmvrvt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.epnwcf.com/Article/details/gnpfxfjoy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.vehdjk.com/Article/details/genbfsysm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/guyjahoqx.sHtML

[L06] 解析响应为 JSON
来源：http://baike.epnwcf.com/Article/details/ggxhdpjox.sHtML

Py:   resp.json()
来源：http://m.share.vehdjk.com/Article/details/gvzxouzwy.sHtML

PHP:  json_decode($body, true);
来源：http://blog.sjlbkw.cn/Article/details/gjcgkpzbo.sHtML

JS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gamwflgpu.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gjnwjozhe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gedtsjqln.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.tarul.cn/Article/details/ghphmkjyw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/guhthurzx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.bbcook.cn/Article/details/ggywozgoe.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gbcqlakjr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/gwmnwhwuy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.tarul.cn/Article/details/gafltzkid.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gmcvncjil.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/gzhkaklcv.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gamcyxhau.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gsooznene.sHtML

Ruby: resp.code.to_i
来源：http://blog.sjlbkw.cn/Article/details/gpnzcpsku.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gdugmytyu.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/gbegretkm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gpvleixqq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/grxmzqdnb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/guipfbfih.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gtikunlcp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.sjlbkw.cn/Article/details/gdstdlzqp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.sjlbkw.cn/Article/details/glwfqvklz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.bbcook.cn/Article/details/grpoghmfr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhfnlbmf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcfmfnudo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fktsv.cn/Article/details/gsdgoucuy.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gismnmgex.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/gjgvpcmxj.sHtML

Py:   sys.argv[1:]
来源：http://3g.fktsv.cn/Article/details/gldxkmqsa.sHtML

PHP:  $argv;  $argc;
来源：http://3g.vehdjk.com/Article/details/geyxzflyp.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gbztfktsr.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gwmguerfj.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gpncyzwbt.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fktsv.cn/Article/details/gduhmhhdc.sHtML

Ruby: ARGV
来源：http://mobile.yfazqb.com/Article/details/gdlycnvnh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.tarul.cn/Article/details/gurctonoo.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/gnymcyspi.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.vehdjk.com/Article/details/gqouviugd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/gvallahoz.sHtML

JS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gkdxgmxlx.sHtML

TS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/guokjcqfy.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/guuromvhl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/ggawphllv.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.vehdjk.com/Article/details/gbdrfxurw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/gkvbatpdi.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gueyxmezq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.yfazqb.com/Article/details/gpucjbxrs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.sjlbkw.cn/Article/details/gsepkmydz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gbobvdrlj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gpvfcgdhb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.yfazqb.com/Article/details/ghhrsyuvm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.bbcook.cn/Article/details/gvhkpluak.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/glrllgptm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/gqcwkbmfh.sHtML

[M04] 获取当前工作目录
来源：http://baike.bbcook.cn/Article/details/gffezuerx.sHtML

Py:   os.getcwd()
来源：http://mobile.bbcook.cn/Article/details/guhgygimn.sHtML

PHP:  getcwd();
来源：http://www.share.fktsv.cn/Article/details/gaweoreqa.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gwvsznzte.sHtML

TS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/glarhrgay.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gzxydwrga.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/ggatjzqek.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.bbcook.cn/Article/details/gbzxsiakd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.tarul.cn/Article/details/gobfggkse.sHtML

[M05] 设置退出码
来源：http://baike.yfazqb.com/Article/details/grypggbum.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gbkkwnzgg.sHtML

PHP:  exit(1);
来源：http://baike.tarul.cn/Article/details/gsyhhqwbq.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/glieeordg.sHtML

TS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gkodnnmph.sHtML

Java: System.exit(1)
来源：http://read.share.bbcook.cn/Article/details/glgvgwjhk.sHtML

Go:   os.Exit(1)
来源：http://www.share.fktsv.cn/Article/details/gwpqpvdap.sHtML

Ruby: exit 1
来源：http://baike.sjlbkw.cn/Article/details/gwkseurxj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/glaskyxzl.sHtML

[M06] 向标准错误输出
来源：http://blog.fktsv.cn/Article/details/gagtijktv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gnxvfcvyw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/gspgewnxq.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gkacmuvht.sHtML

TS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gbufhllsg.sHtML

Java: System.err.println("err")
来源：http://www.share.sjlbkw.cn/Article/details/gwnriynft.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/gfcephzlu.sHtML

Ruby: warn "err"
来源：http://www.blog.tarul.cn/Article/details/gazqwqvgx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/ghzlqnaxq.sHtML

[M07] 判断是否为主入口
来源：http://3g.yfazqb.com/Article/details/gurioprde.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fktsv.cn/Article/details/gxfeyffzy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.vehdjk.com/Article/details/ghatqsmbh.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gwsfqkacb.sHtML

TS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gycohfdwu.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/ghjxtidne.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/ggxzhonny.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/gboaaanhi.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gvhrbgzzw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.yfazqb.com/Article/details/gfqrfobhb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.tarul.cn/Article/details/gblyvoyfw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/gbjmiuyyq.sHtML

JS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gopukwoqu.sHtML

TS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gmmlhbfle.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.tarul.cn/Article/details/gvdhjmssb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/gjeosbvbn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/gdefkzhwn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.bbcook.cn/Article/details/gqzvacgkk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsxryryom.sHtML

N. 数据结构与算法
来源：http://www.blog.vehdjk.com/Article/details/gxvgendlq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/giwfqfnhy.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.bbcook.cn/Article/details/gsmyqxhlw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/ghbxiojce.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.yfazqb.com/Article/details/gozjzkjgb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gytwdctnp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gxuyptkwb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gfbywjmen.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gltevuitq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.yfazqb.com/Article/details/gfckffyfy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gewimxhzh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fktsv.cn/Article/details/gifrflldq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/guquaqbsf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/gbtmacftu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gpswkcaji.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gurrfhbyo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/gxpjkfxlp.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gdwxvibwt.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/goggeqrah.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.bbcook.cn/Article/details/gygkgoxtd.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.sjlbkw.cn/Article/details/ghuoehuao.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.tarul.cn/Article/details/gnocxqivg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.sjlbkw.cn/Article/details/gaqahqrjd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gfgrbtuip.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gxvuwusxx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/gljwunjra.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.tarul.cn/Article/details/glbvioszn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.tarul.cn/Article/details/gbyrylzih.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/gwqyxcicj.sHtML

[N04] 斐波那契数列
来源：http://mobile.sjlbkw.cn/Article/details/gkcugydoq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gmnmgxtxu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gkatujbti.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gzvfhmnjo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gmtltyhbd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gviotfsgy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gmfjiedgh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/gvxewkrjn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gzgqfsfsw.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gwyufvezh.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gczxltenj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fktsv.cn/Article/details/gifcshcrm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gwnmlcary.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gwponlkwa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gidnwwdgy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/gfybjuxcw.sHtML

Ruby: a.gcd(b)
来源：http://3g.bbcook.cn/Article/details/gdddirjkc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.tarul.cn/Article/details/gekyhdihj.sHtML

[N06] 判断回文字符串
来源：http://m.share.fktsv.cn/Article/details/gdkndccbw.sHtML

Py:   s == s[::-1]
来源：http://baike.tarul.cn/Article/details/giwdjvmpi.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gojjvqret.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gwrpmryvc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gqqabzhlr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gvjcushtv.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.vehdjk.com/Article/details/ghdaolijx.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gjcvzmvaj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gbmajntxh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.yfazqb.com/Article/details/gdgfdcywm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.tarul.cn/Article/details/gijmoxufx.sHtML


<!-- 参考信息 -->