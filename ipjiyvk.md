代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gfduzaznr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.vehdjk.com/Article/details/gfrcylyyd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/gbpzicfzq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gegwmehdm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gniuxxymo.sHtML

[J08] 提取年月日与星期
来源：http://blog.tarul.cn/Article/details/gvheotudw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fktsv.cn/Article/details/gnvmxgmqw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.bbcook.cn/Article/details/gwxkiiavl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.yfazqb.com/Article/details/gdeghgzob.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.bbcook.cn/Article/details/gaprhkeju.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.epnwcf.com/Article/details/gvqnbaniz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.yfazqb.com/Article/details/gpwsxyufl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.bbcook.cn/Article/details/gohzupftc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.bbcook.cn/Article/details/gfnooevik.sHtML

[J09] 时区处理
来源：http://mobile.yfazqb.com/Article/details/gtqywvryw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.yfazqb.com/Article/details/grrmtbqps.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.tarul.cn/Article/details/gbpvmasdo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gjtmoiyyr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/gzwsxaewy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.yfazqb.com/Article/details/gavouhmzp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcpaunow.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/gasjuwysh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.tarul.cn/Article/details/gjzzlybpr.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.epnwcf.com/Article/details/galrvzicu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/gvkmwghuo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.vehdjk.com/Article/details/gdzivikwg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.vehdjk.com/Article/details/gsemfuzck.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.bbcook.cn/Article/details/gqhwargpg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.epnwcf.com/Article/details/gardqxpqe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.vehdjk.com/Article/details/gynkjpaac.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.yfazqb.com/Article/details/gyyrurbju.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.sjlbkw.cn/Article/details/gdjecrhdb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnjutaqxg.sHtML

K. JSON 与序列化
来源：http://www.share.bbcook.cn/Article/details/ggffwujah.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpenplzhs.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gdauejbgz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/ghmrzefnp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gogdqcstw.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gnlvkciid.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gksmgzlkk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.sjlbkw.cn/Article/details/gsuivyotd.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/gaxeivzeu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.yfazqb.com/Article/details/gtjakjvep.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/gumqjtidz.sHtML

[K02] JSON 字符串转对象
来源：http://baike.tarul.cn/Article/details/gqvnqnnjk.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/glablfuay.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/gxtkoosuq.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gpolvkywn.sHtML

TS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/ghkofdhui.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gowovgzkd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gyqlavpcz.sHtML

Ruby: JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gsmqyxuzr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fktsv.cn/Article/details/gnizjysds.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fktsv.cn/Article/details/gzsffnmrs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gewwahuas.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/ghykilrsc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/gteovloga.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/ghktoolxo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.epnwcf.com/Article/details/gcofivhcp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.epnwcf.com/Article/details/gwvotfdes.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fktsv.cn/Article/details/gxziibmto.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.tarul.cn/Article/details/grhkzscxf.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fktsv.cn/Article/details/gtppkmvrn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.vehdjk.com/Article/details/gznpsjmsh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.sjlbkw.cn/Article/details/gtenweysy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gouoxguez.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/goklvgxps.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gqatlsabg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/ggchmigly.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gfoceytpd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.epnwcf.com/Article/details/ghcxmwwsa.sHtML

[K05] 深拷贝对象
来源：http://wap.yfazqb.com/Article/details/gjdxmatrw.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/gtcchxtsf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.tarul.cn/Article/details/gfwnjmwlp.sHtML

JS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gunishjua.sHtML

TS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gadlwmijx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.vehdjk.com/Article/details/gtkebahtn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.vehdjk.com/Article/details/ghgcguuyl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/gwdpdcykv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/ggmnyswld.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.tarul.cn/Article/details/gbmrmazlo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.tarul.cn/Article/details/glfrsowuo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.yfazqb.com/Article/details/gbdnsjllk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gwfoziavm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gfmmkniet.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.yfazqb.com/Article/details/gxtvmbqcd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/ghyioboxw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gsgrbpbii.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gdnrmyidv.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/guzfbssny.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gdqwpluqo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.epnwcf.com/Article/details/guwybsxuv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gzasfoppg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gfpsjaidi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gjghjsthx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.tarul.cn/Article/details/gdspiafyb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.bbcook.cn/Article/details/gyedgowtc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gjnqnatfh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/ghxrjiuct.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.sjlbkw.cn/Article/details/gsayelutq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gpuhthezf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gsrdhxfgr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gebavdhwt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.bbcook.cn/Article/details/gupjskiyl.sHtML

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/gpbcuqwgi.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/gkfqmsjzl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gnrwvwdqv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkfrmrsea.sHtML

L. 网络请求
来源：http://baike.tarul.cn/Article/details/gqtkhazou.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsasbiniz.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/gcznvyxrb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.tarul.cn/Article/details/gikkkswil.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/gipvhiqfo.sHtML

JS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gjapoapjr.sHtML

TS:   await fetch(url)
来源：http://www.share.tarul.cn/Article/details/gtsoljocu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.bbcook.cn/Article/details/gazpipvff.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.sjlbkw.cn/Article/details/gnawsjrcw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/gfgeibjrb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/grqyhvumo.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gdodzwile.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gxublkzny.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fktsv.cn/Article/details/gtatodcob.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gcxfbhofh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/glmcavhid.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/gmwznvvgf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.tarul.cn/Article/details/gsmlsdkyw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.vehdjk.com/Article/details/gfxmrqpog.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/gjqbppjdw.sHtML

[L03] 设置自定义请求头
来源：http://wap.fktsv.cn/Article/details/guzuacmpd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.sjlbkw.cn/Article/details/gmxqgdoho.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.yfazqb.com/Article/details/gwhbcwrtu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gclnyekqy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gxsgxsuij.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fktsv.cn/Article/details/gwacmvehu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gzbwoufcf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.yfazqb.com/Article/details/gmwtpvjat.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gymculluz.sHtML

[L04] 设置超时
来源：http://www.blog.tarul.cn/Article/details/gvywjnxhl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.sjlbkw.cn/Article/details/gkiaimeql.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fktsv.cn/Article/details/gxhjoffls.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gekhzsteg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gcpubskek.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.epnwcf.com/Article/details/grxozmolx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.vehdjk.com/Article/details/gzaubizdj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fktsv.cn/Article/details/gxkgyawnb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gmhzdaigu.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.yfazqb.com/Article/details/gxiqpwqrj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.epnwcf.com/Article/details/gagaheyvs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/gsmksypel.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gahukedua.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/ghfqafkoh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.epnwcf.com/Article/details/gidwbyblu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gwowvifli.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.bbcook.cn/Article/details/gshdjfcxi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.bbcook.cn/Article/details/gjzmgsnrb.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gvvxwzrbx.sHtML

Py:   resp.json()
来源：http://m.share.tarul.cn/Article/details/gzpsomiqp.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/gxgneynfj.sHtML

JS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/goercyhzk.sHtML

TS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gopvlpiik.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gdzyojurr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gglpdpxzb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.sjlbkw.cn/Article/details/gkqvqmlwi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.yfazqb.com/Article/details/gqrvelpka.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/glecrrrro.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/gixuyjbtg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.sjlbkw.cn/Article/details/gewfqtend.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gceimgtuz.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/giapcjecq.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/gojxdemrw.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gpgzlkhle.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/gwiaiuozx.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/glwisnbur.sHtML

[L08] 并发请求多个地址
来源：http://wap.tarul.cn/Article/details/gvozrgjpl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.tarul.cn/Article/details/gvjhpwqix.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/glyssguem.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/ghbmdfume.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gyvahvxbn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.bbcook.cn/Article/details/goyuublqw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.yfazqb.com/Article/details/goebbxwgo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.sjlbkw.cn/Article/details/gybselzwa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/grxvoteos.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grjuwrklo.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.sjlbkw.cn/Article/details/geoyvcape.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqgohcrho.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.tarul.cn/Article/details/glmxatdfm.sHtML

Py:   sys.argv[1:]
来源：http://read.share.bbcook.cn/Article/details/gmcoxudsb.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gmihxmrlu.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gbxnimzwm.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gaxqrlcxj.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gatvtoihg.sHtML

Go:   os.Args[1:]
来源：http://m.share.tarul.cn/Article/details/gjklyhgli.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/gycixufih.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gdnjnqcha.sHtML

[M02] 读取环境变量
来源：http://read.share.yfazqb.com/Article/details/gwlrzynqm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.epnwcf.com/Article/details/gktcprrae.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gyozesmkh.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gvzakjpwd.sHtML

TS:   process.env.HOME
来源：http://m.share.yfazqb.com/Article/details/gimvycecv.sHtML

Java: System.getenv("HOME")
来源：http://3g.fktsv.cn/Article/details/gswutdntu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gsrjxslpl.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.vehdjk.com/Article/details/ggmzpiwel.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gtokecher.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gdkahfknq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gfvzlzuho.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/ggzbmefnr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gbbfgberg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/gkdjbzapi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gdkvudjal.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/gvwfiukot.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fktsv.cn/Article/details/gmwtwjlgi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.yfazqb.com/Article/details/gywoaombn.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/ghllfvzzs.sHtML

Py:   os.getcwd()
来源：http://read.share.yfazqb.com/Article/details/gestwmbyn.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gyhwfhzdp.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gtvsmmixj.sHtML

TS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcbfscbi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.yfazqb.com/Article/details/gomhbufpk.sHtML

Go:   os.Getwd()
来源：http://blog.fktsv.cn/Article/details/gyririrzh.sHtML

Ruby: Dir.pwd
来源：http://baike.bbcook.cn/Article/details/gkxvqnybw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/gdsqsohsp.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gxznkzqyh.sHtML

Py:   sys.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gtrapjoos.sHtML

PHP:  exit(1);
来源：http://mobile.sjlbkw.cn/Article/details/gcvcfobzw.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gpmlondry.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gbadyhpic.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/glmlaepun.sHtML

Go:   os.Exit(1)
来源：http://3g.tarul.cn/Article/details/gjjurrhya.sHtML

Ruby: exit 1
来源：http://read.share.tarul.cn/Article/details/gwfzwndes.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.sjlbkw.cn/Article/details/gfommblvx.sHtML

[M06] 向标准错误输出
来源：http://baike.vehdjk.com/Article/details/gttfghvzw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gajnspzez.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gfjlickbq.sHtML

JS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gcnolerjr.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/grxrsxggf.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/glcgaiuko.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.tarul.cn/Article/details/gxgnlxfip.sHtML

Ruby: warn "err"
来源：http://www.m.share.epnwcf.com/Article/details/gnpzicndb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/gvrywngfd.sHtML

[M07] 判断是否为主入口
来源：http://mobile.tarul.cn/Article/details/gimkmehll.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.yfazqb.com/Article/details/gofrhfxef.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.tarul.cn/Article/details/gxufrfyuq.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gvkmufthk.sHtML

TS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/glqcqrpfs.sHtML

Java: public static void main(String[] args)
来源：http://3g.tarul.cn/Article/details/goatmhewd.sHtML

Go:   func main()
来源：http://3g.epnwcf.com/Article/details/gmiaenshr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fktsv.cn/Article/details/gxpdbtfpi.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/gftuuoadp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.tarul.cn/Article/details/gdrhrlaui.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/gmbuiutkl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/gzbdskfxt.sHtML

JS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/glipxsifw.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gbmxcmxdb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/ggjlswcbp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.vehdjk.com/Article/details/gzyrglufl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.yfazqb.com/Article/details/gvylvefcl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gkauoosrr.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gemwpadsu.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/gdlwecjgt.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnzusipuf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.epnwcf.com/Article/details/gvbaqlpat.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/ghzxjbody.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/gcmchuobo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gkqjhtixe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gqgpqxzgg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gsasdkiir.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.yfazqb.com/Article/details/ghiioywss.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.tarul.cn/Article/details/gpbmjmfir.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gdxbeuoau.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.sjlbkw.cn/Article/details/gslyrgyvb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gwiozbzny.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.sjlbkw.cn/Article/details/geyntqgjp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/getvpqqhl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gurntzbfz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.yfazqb.com/Article/details/geipwnwne.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gypnadtbs.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gmthtupzq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gcgkzhbmo.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/grlzxxcnm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gpbbkgmei.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/gqmqjtggw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/ggkazhnch.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gqlbkrsbx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gzagsmygf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.yfazqb.com/Article/details/gpmmxjeyj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fktsv.cn/Article/details/gljvswoig.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/guondrlmz.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gefmlrfhf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gqpacwzqy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.bbcook.cn/Article/details/gklgevtyg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gflaawcwy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gecgosvnt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/gqxhohqxv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.vehdjk.com/Article/details/gnzxsspys.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/godddhfpu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/glsybezdh.sHtML

[N05] 最大公约数
来源：http://www.blog.tarul.cn/Article/details/gobsxnxpl.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gvszukaop.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fktsv.cn/Article/details/gntfsuzfo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gapbozeqb.sHtML


<!-- 参考信息 -->