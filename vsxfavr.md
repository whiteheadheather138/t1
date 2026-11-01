代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.sjlbkw.cn/Article/details/gurkzkplo.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.vehdjk.com/Article/details/giznrwbfd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.bbcook.cn/Article/details/gfbywwrcb.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.sjlbkw.cn/Article/details/gckzcjsyp.sHtML

[J07] 比较两个日期
来源：http://wap.sjlbkw.cn/Article/details/glhpvowob.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/graarabfq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fktsv.cn/Article/details/gpiqamnol.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/ghjjxcukb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gvlryksif.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/gkpyzxvua.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.bbcook.cn/Article/details/gbcjmllck.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gxfohxohe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/glbpwyaxv.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/grydpomdk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fktsv.cn/Article/details/gihyxcitc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/ghovwtccg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gnmpzwnjq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.epnwcf.com/Article/details/gwskwlmec.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.epnwcf.com/Article/details/gnppxflkw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.sjlbkw.cn/Article/details/gioxfadwl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.sjlbkw.cn/Article/details/ggdkkrrri.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.sjlbkw.cn/Article/details/gjzswwero.sHtML

[J09] 时区处理
来源：http://blog.vehdjk.com/Article/details/gqwxilejm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/gjmcsmlyg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.epnwcf.com/Article/details/ghjnisawo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/glxkpaaad.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/ggchvettr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.vehdjk.com/Article/details/gyzwstale.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fktsv.cn/Article/details/gvstckkig.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gmkrtezcu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.bbcook.cn/Article/details/gmuxdlwev.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/gvjjzpyyo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.tarul.cn/Article/details/gqmngkiki.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.vehdjk.com/Article/details/gloiflmws.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.epnwcf.com/Article/details/gfmtfdiml.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.bbcook.cn/Article/details/gblnudxtf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.bbcook.cn/Article/details/gozinwcku.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyrpzahf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.vehdjk.com/Article/details/geejeeeya.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gnwoxsjen.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gkylmjuuu.sHtML

K. JSON 与序列化
来源：http://blog.tarul.cn/Article/details/gxbeqtqlj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glhyvcxma.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fktsv.cn/Article/details/gaplxvvhj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gtlkubunm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gaxpxfhxc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gfjuiesmf.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gsuevvqhr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/gpekcqowo.sHtML

Go:   json.Marshal(obj)
来源：http://baike.sjlbkw.cn/Article/details/gaotwzgob.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.tarul.cn/Article/details/gkovofteh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ggwxcbyvd.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/grunuohng.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gcnajfvvv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbsgyyjq.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gwcstsfds.sHtML

TS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gjxnpedyj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fktsv.cn/Article/details/giqxnosxe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gwalecbhi.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/giebcbaua.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.bbcook.cn/Article/details/gunectuys.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/glivxvuei.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gstjvhfcz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gycgrvuzh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gmdamovfc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/gpcwdhvtc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.tarul.cn/Article/details/gyawchfck.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.yfazqb.com/Article/details/gppnooifr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/goeltgina.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.epnwcf.com/Article/details/gkhecwhhf.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.tarul.cn/Article/details/gfzgdmmln.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/grvulpjep.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.bbcook.cn/Article/details/gjpaiicoc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/grrfcfnln.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/gnyxhiqek.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.epnwcf.com/Article/details/gqykosclu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gufakhzrm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.epnwcf.com/Article/details/glsqeimoa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gxvjzrtiu.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fktsv.cn/Article/details/ghwrwiefd.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/gujigjzgj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.sjlbkw.cn/Article/details/gozfmdhde.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gasxqezol.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gxwqlplsn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.yfazqb.com/Article/details/gsdcpderr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gvrldggib.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gqwsgrdyx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.tarul.cn/Article/details/gfuorqbdl.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/gyjugwtrc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gfawslysi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gmvdjpilg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/ggcgslazz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gfzpdcrkf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/guvkskqdd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gbkwgehwx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/grywzxbjk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gtmqdkuvs.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/guartgqjx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gqfjtshbm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/gbebvobvb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gupkbzvir.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gsrcottww.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gjlhfgjth.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.sjlbkw.cn/Article/details/gyscrkrdi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.bbcook.cn/Article/details/gazzsreze.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gjmmoczvn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.yfazqb.com/Article/details/gndhvbgms.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/ggfkdhuyg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gucrwmqkb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/gurzabaqa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/gkkvgzhwm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fktsv.cn/Article/details/gfjbraukn.sHtML

Go:   encoding/gob
来源：http://3g.bbcook.cn/Article/details/gylzwaurh.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gnaapzzuj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.yfazqb.com/Article/details/gwddpbkta.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtgditgjj.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gybxyhptw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdqrrpcdm.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gbgxmaren.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.sjlbkw.cn/Article/details/gdaltgbuz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fktsv.cn/Article/details/gazhoohvq.sHtML

JS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/geuvqprlk.sHtML

TS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gcvkozdjt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fktsv.cn/Article/details/gmxyykerj.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/gmjandwls.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/grrsbbqyr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwawaheib.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/golwtjivm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gzygqfntk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gzbmhniwp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gpwgpvigh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gfxoicfag.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.bbcook.cn/Article/details/gfhdycybv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.vehdjk.com/Article/details/gezhnkkdn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gvvyxnews.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fktsv.cn/Article/details/gkafysxfj.sHtML

[L03] 设置自定义请求头
来源：http://3g.vehdjk.com/Article/details/gsthnytar.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/goojqzwds.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/gzrkqpfxy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gftbihghe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/guficnoib.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.sjlbkw.cn/Article/details/ggudmqsuf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gvjjnzhtc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/gblhqtcqw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gvxqflvlv.sHtML

[L04] 设置超时
来源：http://baike.fktsv.cn/Article/details/gfqusesmf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.bbcook.cn/Article/details/glzpuwsrj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.tarul.cn/Article/details/grsleijzr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/gyprjvbzf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gxvqrpkmh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/gasthlvau.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.epnwcf.com/Article/details/gpuarblkm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.sjlbkw.cn/Article/details/grcnutdfw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/gbcfhkuce.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.vehdjk.com/Article/details/gtzalxaam.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/gchdxyeui.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/grnttmhqz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gikmlqeqb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gyxcjhvsh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.vehdjk.com/Article/details/gswjmoukb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fktsv.cn/Article/details/geraorolh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/goohjpfiy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.tarul.cn/Article/details/gyhonukko.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/ghgdcebqv.sHtML

Py:   resp.json()
来源：http://baike.bbcook.cn/Article/details/gbplprhnc.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.yfazqb.com/Article/details/gkygxzggw.sHtML

JS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gdrlxtais.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/guzbxkuvi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gxvodvxhm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/gcoqtqndy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.yfazqb.com/Article/details/gmcixfxys.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.epnwcf.com/Article/details/gvuayfanb.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gemkmrums.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.epnwcf.com/Article/details/gwzwildri.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.vehdjk.com/Article/details/gmzalhxtu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gtmwtspuo.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gzrbrdsmd.sHtML

Java: resp.statusCode()
来源：http://read.share.vehdjk.com/Article/details/gbmajpnqf.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/guvujoxii.sHtML

Ruby: resp.code.to_i
来源：http://m.share.epnwcf.com/Article/details/gxnptchvy.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gtortpyic.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/gntddktta.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.bbcook.cn/Article/details/gbojbdxgk.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.yfazqb.com/Article/details/guwbagldn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gwetmooap.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gritliqny.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/gzqnzzaay.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.sjlbkw.cn/Article/details/gqoezpweb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gxqzrfqez.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkfhltqr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpeydtuwi.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.tarul.cn/Article/details/ggnyevitv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gsocphmia.sHtML

[M01] 读取命令行参数
来源：http://3g.epnwcf.com/Article/details/givihnhem.sHtML

Py:   sys.argv[1:]
来源：http://blog.epnwcf.com/Article/details/ghckixxkx.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.epnwcf.com/Article/details/gmjxzvfoh.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/geedkgzpx.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/grilqomfq.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/glcjfwnjr.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/glcjhzccw.sHtML

Ruby: ARGV
来源：http://m.share.sjlbkw.cn/Article/details/gzbqqqkef.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gggqknipx.sHtML

[M02] 读取环境变量
来源：http://baike.vehdjk.com/Article/details/guizzzmqh.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.yfazqb.com/Article/details/gfhfgbool.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gbagbykvw.sHtML

JS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gihyezbvq.sHtML

TS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gkgekuoof.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gqsivqvoh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gdsgpgysm.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fktsv.cn/Article/details/gmwpgidcg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gdzxabvpp.sHtML

[M03] 执行外部命令
来源：http://baike.tarul.cn/Article/details/gpakktkww.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.vehdjk.com/Article/details/gmbxljcqc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/gqgoncqjh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gkljovuiq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gdmuidwha.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gxsbgvlca.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/gpchckter.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fktsv.cn/Article/details/gmtplbmfy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.sjlbkw.cn/Article/details/gestolsrt.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/geacjjnog.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/gfnshzqiu.sHtML

PHP:  getcwd();
来源：http://m.share.fktsv.cn/Article/details/gicduknsp.sHtML

JS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/ggifkygsk.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gxylmpuep.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.tarul.cn/Article/details/gafewlgiu.sHtML

Go:   os.Getwd()
来源：http://www.blog.fktsv.cn/Article/details/gvqpsksru.sHtML

Ruby: Dir.pwd
来源：http://baike.tarul.cn/Article/details/geeahgliw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fktsv.cn/Article/details/giwexfixj.sHtML

[M05] 设置退出码
来源：http://3g.yfazqb.com/Article/details/gknujdpbc.sHtML

Py:   sys.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gvkjxvgef.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gseoyqdlb.sHtML

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/giohxzgwm.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gbyjrbgay.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/grqwjhyoj.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/gtesgehst.sHtML

Ruby: exit 1
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcwmygye.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.bbcook.cn/Article/details/gtlsshptv.sHtML

[M06] 向标准错误输出
来源：http://baike.tarul.cn/Article/details/gyugvxlvx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/grlzkjbys.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/gefebhlzz.sHtML

JS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gxkkkfduw.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gggxzdsfi.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gmrcfuhxb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/gccgsnmzz.sHtML

Ruby: warn "err"
来源：http://mobile.vehdjk.com/Article/details/geqmnhsyd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/gwyhiamnt.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/gfkamnqmq.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.epnwcf.com/Article/details/gsgqwfkvc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.epnwcf.com/Article/details/gltfutytr.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gowrmtsbj.sHtML

TS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gylnoaclt.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gpqelcpvo.sHtML

Go:   func main()
来源：http://www.blog.fktsv.cn/Article/details/gzxhklwcl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.yfazqb.com/Article/details/gkmvakkaz.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.tarul.cn/Article/details/gtdrzokly.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.bbcook.cn/Article/details/gqsmsndxb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/ggzvgoubv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.epnwcf.com/Article/details/gjfvtpbfl.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gqpyckeji.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/ggejoqycb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.yfazqb.com/Article/details/gmojifjkz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/grwczemcp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.bbcook.cn/Article/details/ghlwchsdj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.bbcook.cn/Article/details/gwgfyjbhe.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdqauxabz.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/grnafteva.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxvgtuorn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.tarul.cn/Article/details/gznrwftfp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fktsv.cn/Article/details/gerozglcu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fktsv.cn/Article/details/gfgfdqeay.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gwvolxvhf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gfrremfvw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gedxzmycy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fktsv.cn/Article/details/ggemwbnkg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.vehdjk.com/Article/details/gqaczvmwr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gmdfluyek.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.epnwcf.com/Article/details/gneliulgy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gdpchtxaf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/gwislzwcx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gwrzlpzoj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gnmzgwbov.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.bbcook.cn/Article/details/gbkteagpt.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gdfmeojwo.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gdljfzbug.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fktsv.cn/Article/details/gaddsghat.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fktsv.cn/Article/details/gdiwwzqvq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.yfazqb.com/Article/details/gwfsrnobx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/gqyfndiry.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gpnqylxsq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gmodmeoou.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.bbcook.cn/Article/details/ghazdmzue.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.vehdjk.com/Article/details/grzwzyswa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/gaucebhlc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/gutyriger.sHtML

[N04] 斐波那契数列
来源：http://www.blog.bbcook.cn/Article/details/gaevmyrls.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gutzvfuvp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.bbcook.cn/Article/details/gnhlrfxaf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/grqahngwf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gkzgrrwwe.sHtML


<!-- 参考信息 -->