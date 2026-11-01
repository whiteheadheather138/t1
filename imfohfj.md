代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gsxukdatr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.bbcook.cn/Article/details/gztlrujai.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.bbcook.cn/Article/details/gofbpmegn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gykylkvmm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gpkpicftp.sHtML

[J08] 提取年月日与星期
来源：http://m.share.epnwcf.com/Article/details/glkvjpppq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.vehdjk.com/Article/details/gzmyfwkdz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.yfazqb.com/Article/details/gfthjdebf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fktsv.cn/Article/details/gfegftjxh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.epnwcf.com/Article/details/gibtzzgre.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.tarul.cn/Article/details/gnpphcpfy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.sjlbkw.cn/Article/details/guyiyadgi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.tarul.cn/Article/details/gbjxiwuft.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/gngnwflgn.sHtML

[J09] 时区处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkhnmxva.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.yfazqb.com/Article/details/gepvvertz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/gmgvhnfie.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/grotuagzj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/gdfoeomkg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.sjlbkw.cn/Article/details/guytdazgq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.vehdjk.com/Article/details/gfjbzcqrk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fktsv.cn/Article/details/gthmqrjyt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.tarul.cn/Article/details/gvtfabmwc.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.bbcook.cn/Article/details/gbivlpzdd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.yfazqb.com/Article/details/gvyiehsaw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.epnwcf.com/Article/details/gwywtdknn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fktsv.cn/Article/details/glwalxubn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.vehdjk.com/Article/details/gzjqdqujh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/gtxhgujes.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.bbcook.cn/Article/details/gckeioymu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.bbcook.cn/Article/details/gxaftnege.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fktsv.cn/Article/details/gjzfvnent.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/giccrzeep.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gfoyjldjl.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjebsagjq.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.bbcook.cn/Article/details/gbptabdxq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/gzbwxvlfu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gakzhzasd.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gtmqgkfyj.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gaaufnyxq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fktsv.cn/Article/details/giovupzbn.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/grspfhcyi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.sjlbkw.cn/Article/details/gcqgsxgpd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.yfazqb.com/Article/details/gyuwnazdh.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fktsv.cn/Article/details/gtttqlwuw.sHtML

Py:   json.loads(s)
来源：http://m.share.vehdjk.com/Article/details/gpwazrnyg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fktsv.cn/Article/details/gteqseobl.sHtML

JS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/grrlhfeuo.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gpmgpixct.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/gtckivcil.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.tarul.cn/Article/details/gsjtdbfwh.sHtML

Ruby: JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/giptsohpz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.yfazqb.com/Article/details/gmggmitis.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gcqaljpfi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gptvxiotn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gwcfifmzt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/gcinmisql.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gcymsorme.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gewgoingt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fktsv.cn/Article/details/geutbnojn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.tarul.cn/Article/details/ggidftecm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.tarul.cn/Article/details/gfzqmafoc.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.yfazqb.com/Article/details/gcgykeuvq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gjknrwtqo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gogdejhma.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/glucyjkba.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gwjlczyxo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fktsv.cn/Article/details/grluudwec.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gxrkhnvle.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.vehdjk.com/Article/details/gcosjdnlj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gulapcebd.sHtML

[K05] 深拷贝对象
来源：http://read.share.fktsv.cn/Article/details/gpirrqvqz.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.epnwcf.com/Article/details/gwfjrvxkd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/gpvspuelj.sHtML

JS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/ghuerclfb.sHtML

TS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gguszloms.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/gfpokijka.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.tarul.cn/Article/details/glwiuqkah.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fktsv.cn/Article/details/giwavbkus.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fktsv.cn/Article/details/gpoxcyfkg.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.bbcook.cn/Article/details/glitoyodz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/ghkebrivo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.tarul.cn/Article/details/gfdsneglx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gesbndmor.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gheqznjug.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.epnwcf.com/Article/details/gukwoqgqm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gnwcdqebs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gysgkylkn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gpoqfueld.sHtML

[K07] 进制转换
来源：http://www.share.yfazqb.com/Article/details/gqoiixxdo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.tarul.cn/Article/details/gkbimvgst.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/gjvyspejj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gljtwmfvx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gkeuqwvyt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gxejtpxcc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.sjlbkw.cn/Article/details/gagsscakh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fktsv.cn/Article/details/grcrzqnez.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gosgwaond.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/ghdhynnvf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gakihgode.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.tarul.cn/Article/details/gkcrvtrfy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gvhojngyn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/ggqegygwr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/gimnugsta.sHtML

Go:   encoding/gob
来源：http://blog.yfazqb.com/Article/details/gqffblsxu.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fktsv.cn/Article/details/gnoznxzvo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gcdvyjdqb.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzqfkaumb.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/gicqujepz.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gsxtudlje.sHtML

[L01] 发送 GET 请求
来源：http://read.share.vehdjk.com/Article/details/gjnsjpkmn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.yfazqb.com/Article/details/gmazmrlfe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.epnwcf.com/Article/details/ggvibnxlv.sHtML

JS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gevvxuxzn.sHtML

TS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/grypewgoo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.sjlbkw.cn/Article/details/gayndhglm.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/gulabypbk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gayyeapip.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.tarul.cn/Article/details/ghnwmvnoj.sHtML

[L02] 发送 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gorwlnswv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.vehdjk.com/Article/details/gjooyfvfs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/gvxbrwiuv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gaqczdmvx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/grkxpydot.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/grfyhrcfp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/gfgqystxs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fktsv.cn/Article/details/gnnefhphr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.epnwcf.com/Article/details/gnpnrjnbi.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/ghebputhk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.sjlbkw.cn/Article/details/gkdphsryo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gricgncva.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fktsv.cn/Article/details/gzzysyrhm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gqvvnqibw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.tarul.cn/Article/details/gugdsnxwn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gdqfdgzim.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/gzxxooekd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gcucsmkeo.sHtML

[L04] 设置超时
来源：http://read.share.tarul.cn/Article/details/gcyecjsrm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.yfazqb.com/Article/details/gokpmxlho.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/gvisssecj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/goeqgeess.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/ggedjdezt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.vehdjk.com/Article/details/glgjmewrn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.bbcook.cn/Article/details/gyusukcqq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.epnwcf.com/Article/details/gbzyacwyq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.yfazqb.com/Article/details/gambugtyn.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.yfazqb.com/Article/details/ggqmofhhn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.bbcook.cn/Article/details/gwdlhpaqh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.tarul.cn/Article/details/gaoqwowsh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gpbshmmbn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gwvqhlqys.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/gzbldevos.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.tarul.cn/Article/details/ghgxxjeqo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/gxxvhxtmu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.yfazqb.com/Article/details/gruwgmomc.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gkofdwzwt.sHtML

Py:   resp.json()
来源：http://www.blog.yfazqb.com/Article/details/glxcogtjg.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.tarul.cn/Article/details/gkkqfwzrd.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gjzelzaae.sHtML

TS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gdklhghej.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.bbcook.cn/Article/details/grjfyzxpa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.tarul.cn/Article/details/gxsyvskzc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.epnwcf.com/Article/details/glsaberjb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.yfazqb.com/Article/details/gxsnnrxio.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gvmcbbmha.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.vehdjk.com/Article/details/glbvkmxqk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.vehdjk.com/Article/details/gowsxhvrd.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gvxjnnprp.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gyhgrssiq.sHtML

Java: resp.statusCode()
来源：http://blog.sjlbkw.cn/Article/details/gvbkvzrwx.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gvqojqdsa.sHtML

Ruby: resp.code.to_i
来源：http://baike.epnwcf.com/Article/details/gcavszems.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gbomfyxsa.sHtML

[L08] 并发请求多个地址
来源：http://m.share.sjlbkw.cn/Article/details/gyjgtgffr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.yfazqb.com/Article/details/givjychzj.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/gsmsidshu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gjzkkrlvl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gjgydhpgd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.vehdjk.com/Article/details/gqrnqagyv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fktsv.cn/Article/details/gridfyuzr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/ghivstnni.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/golwwlehe.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggughorpn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.bbcook.cn/Article/details/gemsxyaqn.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnhcbkgxy.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gdbrokvbt.sHtML

Py:   sys.argv[1:]
来源：http://read.share.epnwcf.com/Article/details/gmfxwqtpd.sHtML

PHP:  $argv;  $argc;
来源：http://wap.vehdjk.com/Article/details/gmskqtbpc.sHtML

JS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/gvpuuliay.sHtML

TS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gescmwfaw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/ggvrpgony.sHtML

Go:   os.Args[1:]
来源：http://m.share.epnwcf.com/Article/details/gqhnyxgbg.sHtML

Ruby: ARGV
来源：http://read.share.epnwcf.com/Article/details/glllpzddf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gskudlsvu.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gunchmdcr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.bbcook.cn/Article/details/ghriibgga.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gnrsmadxe.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/ghzdrvotl.sHtML

TS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gxabcmszo.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gfkjqssyz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/gdfbnladb.sHtML

Ruby: ENV["HOME"]
来源：http://baike.vehdjk.com/Article/details/gwoubxihj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.tarul.cn/Article/details/gdqggmgyd.sHtML

[M03] 执行外部命令
来源：http://baike.bbcook.cn/Article/details/gxidzegte.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.tarul.cn/Article/details/gzxfbxhjg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/glqnwscye.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/grgomrdvu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gfacvhmaq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gwrlqqgam.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.tarul.cn/Article/details/gevmmhhru.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.epnwcf.com/Article/details/gxbditcue.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gbsjducyl.sHtML

[M04] 获取当前工作目录
来源：http://blog.sjlbkw.cn/Article/details/gakxhkpul.sHtML

Py:   os.getcwd()
来源：http://www.m.share.bbcook.cn/Article/details/geaxflkfb.sHtML

PHP:  getcwd();
来源：http://blog.tarul.cn/Article/details/gxoowvapn.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gpamalelr.sHtML

TS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gqldogeau.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/glpaoaook.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/gqybbpgfp.sHtML

Ruby: Dir.pwd
来源：http://baike.fktsv.cn/Article/details/gpkpdznwg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.yfazqb.com/Article/details/gnvxscaut.sHtML

[M05] 设置退出码
来源：http://www.m.share.fktsv.cn/Article/details/gsbetfslm.sHtML

Py:   sys.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gjklgljre.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/gswiojhrb.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gzfafcrdi.sHtML

TS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gjzdqhdkh.sHtML

Java: System.exit(1)
来源：http://wap.vehdjk.com/Article/details/gutybbzbi.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/gqfgzzcxd.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/ghzeluwzz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.yfazqb.com/Article/details/gonmupqgh.sHtML

[M06] 向标准错误输出
来源：http://mobile.tarul.cn/Article/details/gmnobcqge.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/gncckoumz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.tarul.cn/Article/details/gdbzmdooz.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/glwievytz.sHtML

TS:   console.error("err")
来源：http://3g.tarul.cn/Article/details/gohxzpyfy.sHtML

Java: System.err.println("err")
来源：http://m.share.epnwcf.com/Article/details/gssupcikg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.yfazqb.com/Article/details/grwdfhdct.sHtML

Ruby: warn "err"
来源：http://www.m.share.vehdjk.com/Article/details/glbpkppjc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/grgxctxvw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.bbcook.cn/Article/details/gwqwgwcjm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.vehdjk.com/Article/details/gmukgkozp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/gzlgmhjaj.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gcwgeiqwv.sHtML

TS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/grfattbbp.sHtML

Java: public static void main(String[] args)
来源：http://baike.yfazqb.com/Article/details/gthztftyf.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/gfwbzyzhs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gnznrvydh.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fktsv.cn/Article/details/gfycmtdmc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gbgaukvfb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.vehdjk.com/Article/details/gckbrmwcz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/glnngdipf.sHtML

JS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gmfynxgnj.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gvhvfmegd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/grqbunzch.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.epnwcf.com/Article/details/gbtkxnswr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.sjlbkw.cn/Article/details/gvoilsexa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.sjlbkw.cn/Article/details/gseobhnjf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdfgzomts.sHtML

N. 数据结构与算法
来源：http://baike.vehdjk.com/Article/details/gomkpmuaj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gzzzckswm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fktsv.cn/Article/details/gsomhrvaq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gapmdluwc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.vehdjk.com/Article/details/gwdpayxsx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gzvsgrwur.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gxojmuyko.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gjjuoqdea.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gltaogful.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.sjlbkw.cn/Article/details/gpnnncdxi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gvspcqmho.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.yfazqb.com/Article/details/gnnglyrtk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gtdyvntuh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/gdpmeygsz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/ghyqzptlu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gpjdyrwyy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gtuwvpbhz.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gfvbofomd.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/guaaobmoq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/gfmnwaovk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/gqyqqnyjj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fktsv.cn/Article/details/gcpdmhnbu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.epnwcf.com/Article/details/gtmzrfkgj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gvfzerlhd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gixqisxhc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gwrkfeirz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/gdhlfaite.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.yfazqb.com/Article/details/gwefadkoa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/gxtxpgflm.sHtML

[N04] 斐波那契数列
来源：http://www.share.bbcook.cn/Article/details/gfchfziee.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gxlphogso.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.vehdjk.com/Article/details/gnxhjtdti.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/grmcmbclb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/goitvkllo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gtsqtsfbc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.yfazqb.com/Article/details/gfmpldwvj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gfmaahoyi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gikfvetfw.sHtML

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/galsjligs.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fktsv.cn/Article/details/gtvrlgbpl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gdeglhjnb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gsaemjesn.sHtML


<!-- 参考信息 -->