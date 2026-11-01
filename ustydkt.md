代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.epnwcf.com/Article/details/glriowyrg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gtsrygwsp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gyxwqpoxx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.yfazqb.com/Article/details/gqgtrjcgu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.epnwcf.com/Article/details/gkwcsuyeb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.epnwcf.com/Article/details/gkrrrfleo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.sjlbkw.cn/Article/details/gdhrvcqkz.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/gxxszhhjx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.tarul.cn/Article/details/gobmffdce.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gdxlyembv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.vehdjk.com/Article/details/gxqpcqhlt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gipozekyj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fktsv.cn/Article/details/gtroeysvj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.vehdjk.com/Article/details/gtppdymvb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.sjlbkw.cn/Article/details/gdamflavu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/gshenrkvw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwznjadzi.sHtML

K. JSON 与序列化
来源：http://m.share.yfazqb.com/Article/details/gmoxhjqor.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gonpbrxqb.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.vehdjk.com/Article/details/gnoxpuexa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fktsv.cn/Article/details/giyqtrmpd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gjvewxpam.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gszecfuvq.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/gadjyikgo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/gldmhlwtz.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzcvnqln.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/goxbmxflq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gpdwsynzu.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.yfazqb.com/Article/details/ggojjzaal.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/ggmrzbrct.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.bbcook.cn/Article/details/gnpktbqwh.sHtML

JS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gmvlwhllu.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gypkuxgru.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.yfazqb.com/Article/details/getdkzlnv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gbcxxivca.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gyjmidhyz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/gicjkejua.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.epnwcf.com/Article/details/gioamhfpy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/gonotuhty.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gcgkbaidn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.epnwcf.com/Article/details/gzshjxnqo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gmyfsgoxg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/grwhmrgkz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/gjauqidzo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gspvmplhn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.epnwcf.com/Article/details/gmseqvbrk.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.vehdjk.com/Article/details/gkylnivwn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.vehdjk.com/Article/details/ghbpufkik.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.bbcook.cn/Article/details/gfrhnkktg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gzdzdybmk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/geqtawkig.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gkgfmvhbj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gdfqspoyn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.bbcook.cn/Article/details/grssmvdvz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.epnwcf.com/Article/details/gdjlvgddu.sHtML

[K05] 深拷贝对象
来源：http://baike.fktsv.cn/Article/details/gesonllqw.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/gahqtghxi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.tarul.cn/Article/details/gkqkhbwvj.sHtML

JS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gxjtyebwk.sHtML

TS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gvmvolqxb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.epnwcf.com/Article/details/gsmhofhlg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gcavncwho.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.bbcook.cn/Article/details/gezgkyuiw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gfwyvoodb.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/gttdqibdw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fktsv.cn/Article/details/gmcxjivfk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.bbcook.cn/Article/details/gkdlseupa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gbxjggjrh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gqmzezevj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.yfazqb.com/Article/details/gecnlqtzz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gkbponmco.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/grsslrvjh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gcrlqweqz.sHtML

[K07] 进制转换
来源：http://3g.vehdjk.com/Article/details/gazujvsyf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gnsurafly.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/gfszxizpe.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gmhzpanvx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gkfqdhrgd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/giohfdedk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.vehdjk.com/Article/details/grrmmuiiw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/garaqhvif.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gfwqtsglp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/ghvlrfdid.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/gcbcgwruy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.tarul.cn/Article/details/gqijtkxcs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gumtwjjwr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gyyjcyibf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.yfazqb.com/Article/details/grvhvfvoc.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/guhsqcrlw.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/gdrcyexok.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gghhhqfcv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtnzqddvm.sHtML

L. 网络请求
来源：http://wap.epnwcf.com/Article/details/gtzjgdiga.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gajagftcq.sHtML

[L01] 发送 GET 请求
来源：http://baike.bbcook.cn/Article/details/gxygwpqhe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.yfazqb.com/Article/details/gxrueacwy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gbraxcykm.sHtML

JS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gptvuvtwv.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gsfixwwsi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/gqwzedzfq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/gnfechuzk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.yfazqb.com/Article/details/gecghhenl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fktsv.cn/Article/details/goqfjryba.sHtML

[L02] 发送 POST JSON
来源：http://blog.sjlbkw.cn/Article/details/gwdvvvkqn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gnnxdrrhe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.bbcook.cn/Article/details/goburryvu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gxlwlycby.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gfytngnpr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.yfazqb.com/Article/details/gsrziibay.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.epnwcf.com/Article/details/gskrqknps.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.sjlbkw.cn/Article/details/gjwjzqptt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/gfuyksnvb.sHtML

[L03] 设置自定义请求头
来源：http://blog.tarul.cn/Article/details/gjxfymebs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.vehdjk.com/Article/details/ghmbhuiba.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.bbcook.cn/Article/details/grqkvshvd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gemzuklno.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/geekjlpzn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fktsv.cn/Article/details/gnwbpsozi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gpggbbbqk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/gdxyszprf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gdgkwndoe.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/gwmvcoxds.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gyvztzney.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.epnwcf.com/Article/details/gbdxofmbs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gvfjrtsqo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gjpxcjwcy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/gcuyqbact.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.vehdjk.com/Article/details/gwduoidol.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.tarul.cn/Article/details/gquhgafji.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fktsv.cn/Article/details/gkqxalmji.sHtML

[L05] 上传文件（multipart）
来源：http://blog.bbcook.cn/Article/details/gnoqwuige.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.bbcook.cn/Article/details/gjbnecdbu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/gxjkurkny.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gpfeyjvre.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/ghzlwfelc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gtehelalh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.vehdjk.com/Article/details/gcbcszdov.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.tarul.cn/Article/details/gqbnfoead.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.epnwcf.com/Article/details/gdzxashnb.sHtML

[L06] 解析响应为 JSON
来源：http://blog.sjlbkw.cn/Article/details/guljzejla.sHtML

Py:   resp.json()
来源：http://blog.fktsv.cn/Article/details/gtekkmejt.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fktsv.cn/Article/details/gujhzkwzx.sHtML

JS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gwbttqlsl.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gitqrmmhj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.vehdjk.com/Article/details/gplfgrdvn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.bbcook.cn/Article/details/grgqmzhoj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.yfazqb.com/Article/details/gugsnywfr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.bbcook.cn/Article/details/gopgosqdv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gdyhbvoyv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fktsv.cn/Article/details/gkbafvruk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fktsv.cn/Article/details/gtkuicrrc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gytztbtoc.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gyojswfnu.sHtML

Java: resp.statusCode()
来源：http://wap.vehdjk.com/Article/details/gvanmopxm.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gvwbcqywr.sHtML

Ruby: resp.code.to_i
来源：http://read.share.sjlbkw.cn/Article/details/girjscecv.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gwzhxhqlc.sHtML

[L08] 并发请求多个地址
来源：http://m.share.epnwcf.com/Article/details/gbfrjmiqy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gzjxcqgnx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.sjlbkw.cn/Article/details/gqombiped.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gbbubvbot.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gefjvnogt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.vehdjk.com/Article/details/gwzpprlmq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/gxfseulcq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/glkgyibjw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gvzqvtdhl.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gliotrahz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.epnwcf.com/Article/details/gbfbvxfqu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfgproodb.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.tarul.cn/Article/details/giyevzwju.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/ghtzhuqgo.sHtML

PHP:  $argv;  $argc;
来源：http://wap.yfazqb.com/Article/details/gzzjmaxlg.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gvuljuldr.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gmrmpthjy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/glfiwglko.sHtML

Go:   os.Args[1:]
来源：http://m.share.yfazqb.com/Article/details/golngajav.sHtML

Ruby: ARGV
来源：http://mobile.yfazqb.com/Article/details/gygrsuybn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gbdgnlifp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.epnwcf.com/Article/details/giluwuzwc.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gqdeelwpx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gqrcolqlc.sHtML

JS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gzryixgkg.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gzxexvvkk.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gdmovcvgf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.yfazqb.com/Article/details/gfmfqddag.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fktsv.cn/Article/details/gqjgtjzuk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrbmxoqn.sHtML

[M03] 执行外部命令
来源：http://www.share.epnwcf.com/Article/details/gksehmrtu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/gfmmgqnyn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fktsv.cn/Article/details/gvzrltzoz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/glccudmop.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gaedmmbsh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.yfazqb.com/Article/details/guwowdlgu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.yfazqb.com/Article/details/gyjuyrtkh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/gcfhqxtsg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/gkwdnjaea.sHtML

[M04] 获取当前工作目录
来源：http://wap.vehdjk.com/Article/details/gxqaotytf.sHtML

Py:   os.getcwd()
来源：http://www.blog.fktsv.cn/Article/details/gxygxbvaf.sHtML

PHP:  getcwd();
来源：http://m.share.fktsv.cn/Article/details/gzhiaowfh.sHtML

JS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gpafuhtun.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/grrfcofpd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gbvvnprsa.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/gqloqtkzl.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/gxyxfvtmz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.epnwcf.com/Article/details/glnrgewui.sHtML

[M05] 设置退出码
来源：http://mobile.bbcook.cn/Article/details/gtpvwnqbf.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gbbhbtyke.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/gnnpqtszt.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/goxojtjpv.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gkqbfrpck.sHtML

Java: System.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gzmyccrve.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/gpgjvidtu.sHtML

Ruby: exit 1
来源：http://m.share.bbcook.cn/Article/details/glxehwsxe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.sjlbkw.cn/Article/details/gewiphmuk.sHtML

[M06] 向标准错误输出
来源：http://www.share.epnwcf.com/Article/details/gvtdpdira.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/ggdoznaje.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.yfazqb.com/Article/details/gxdhawfvh.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gcoaoxcyg.sHtML

TS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gxfskggnc.sHtML

Java: System.err.println("err")
来源：http://3g.sjlbkw.cn/Article/details/guvrxbzuc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gmoyibkzj.sHtML

Ruby: warn "err"
来源：http://www.blog.sjlbkw.cn/Article/details/gwzrqkauw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.tarul.cn/Article/details/giywmgnie.sHtML

[M07] 判断是否为主入口
来源：http://baike.vehdjk.com/Article/details/gtcthyblp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.vehdjk.com/Article/details/gxvonxtuo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.yfazqb.com/Article/details/gnxkkidpw.sHtML

JS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gewkpcpyy.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gpubxsjej.sHtML

Java: public static void main(String[] args)
来源：http://wap.tarul.cn/Article/details/gpmrekhab.sHtML

Go:   func main()
来源：http://wap.epnwcf.com/Article/details/gphbuilus.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.bbcook.cn/Article/details/gjcgdqmdu.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.tarul.cn/Article/details/gigpydjjk.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/gbeljxotf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.epnwcf.com/Article/details/gyrdwnnho.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gdpdymixr.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gctlcmyls.sHtML

TS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gmylpaasl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fktsv.cn/Article/details/gyhweoorw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.yfazqb.com/Article/details/gohbnrprh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.vehdjk.com/Article/details/gmgwhrsvl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fktsv.cn/Article/details/gxqdigwmw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gixluqjrj.sHtML

N. 数据结构与算法
来源：http://m.share.sjlbkw.cn/Article/details/gkqrwjupn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzfukchub.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/gceprrcdd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gzlfnczca.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fktsv.cn/Article/details/gjfesmfcr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gaflvtlbu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gamwyaixw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/genygrybq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/ggbfjfafz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/gfzpekvwr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gqbjcpkgq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.tarul.cn/Article/details/gnytwmyut.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gdpmolwla.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gunzihhkz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/getfpxlkq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gycdcpkfp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/gcahodvwr.sHtML

Go:   slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gycozoezz.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gspvwelbp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gojfzuorc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.sjlbkw.cn/Article/details/gwzmyzuhl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.tarul.cn/Article/details/gnmqgwytm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/gftqqxivg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gjjeqezux.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gcnqmsitl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gwdqquoxo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.tarul.cn/Article/details/gfcvxwdru.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/gsvwoeqfc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gutgzcnnj.sHtML

[N04] 斐波那契数列
来源：http://www.blog.sjlbkw.cn/Article/details/grpdqrcpe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gtcxpysbw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gatkubjiq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gwwhwgplb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/glkwzcgzx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gijuoowcz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gfuesjfdy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gktyufgpm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/giwcqyxmc.sHtML

[N05] 最大公约数
来源：http://mobile.epnwcf.com/Article/details/gohnuryix.sHtML

Py:   math.gcd(a, b)
来源：http://blog.bbcook.cn/Article/details/gfohoazzm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gjaewbsxy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gxirmycir.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gaauhmklw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.bbcook.cn/Article/details/gjybwdjtr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.vehdjk.com/Article/details/gveikumwq.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gpgdidgrm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fktsv.cn/Article/details/gthobcwqq.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/ggpfamfsk.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gzamqeben.sHtML

PHP:  $s === strrev($s);
来源：http://baike.tarul.cn/Article/details/gzefjomqd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gzwaedfqw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gvvpbikor.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gcuqotjwj.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gqksixkxz.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuxsphie.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gybclbtif.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fktsv.cn/Article/details/grjqtxhrq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.sjlbkw.cn/Article/details/goxosmarj.sHtML


<!-- 参考信息 -->