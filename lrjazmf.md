代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://wap.bbcook.cn/Article/details/gdsodgowg.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.tarul.cn/Article/details/gnejlbmpo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.yfazqb.com/Article/details/gzzherrfg.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.tarul.cn/Article/details/gxqjkouse.sHtML

[J07] 比较两个日期
来源：http://mobile.yfazqb.com/Article/details/gtjbwmvus.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gfckkybfb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.tarul.cn/Article/details/gwntoniin.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gcnsqcygo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gpaxtsqxe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gppqzzjit.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gqmztiokj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gbfzrrlju.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gjnjevesv.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.vehdjk.com/Article/details/gfqekydzu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.vehdjk.com/Article/details/gzvbvseaj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/gauhvjeky.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.epnwcf.com/Article/details/gctmtirht.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.yfazqb.com/Article/details/gwdmkvpot.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fktsv.cn/Article/details/gsphswchg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fktsv.cn/Article/details/glgemvbsf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/gvbtpqvuz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.vehdjk.com/Article/details/gohszplpa.sHtML

[J09] 时区处理
来源：http://blog.epnwcf.com/Article/details/gwzfdbkzm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.vehdjk.com/Article/details/gowagkiet.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.tarul.cn/Article/details/gajlfpxlk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gqjyffkmj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gksbebtow.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.tarul.cn/Article/details/gwnckdlif.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.bbcook.cn/Article/details/gouhobrog.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.bbcook.cn/Article/details/gnhbgxyvb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.epnwcf.com/Article/details/gndwzbkqd.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.bbcook.cn/Article/details/gzprlxtyd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.yfazqb.com/Article/details/ghstgkiaq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.bbcook.cn/Article/details/gqikvunxn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.epnwcf.com/Article/details/gnbhemkew.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gdmckuxxq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/gonscsvzm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.yfazqb.com/Article/details/gbytsumqz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.bbcook.cn/Article/details/gxulrsdrz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gxwrnndxe.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtnvkhqfz.sHtML

K. JSON 与序列化
来源：http://baike.bbcook.cn/Article/details/gzbutqbtz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtplquyqy.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.bbcook.cn/Article/details/gxfocplas.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/gbroyevzv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gchnsywpi.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gmljvcyvl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/grgyfqhim.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.tarul.cn/Article/details/gwyysssml.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fktsv.cn/Article/details/gbgfnimap.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.sjlbkw.cn/Article/details/gprjfefkb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gqbaxyypc.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fktsv.cn/Article/details/ginrrcyuk.sHtML

Py:   json.loads(s)
来源：http://wap.yfazqb.com/Article/details/gywlbmmkr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.tarul.cn/Article/details/ggvijddhm.sHtML

JS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/glfkllqdp.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gcgyircdu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.vehdjk.com/Article/details/gcgumiivk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gtidvsfro.sHtML

Ruby: JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gananrnia.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.bbcook.cn/Article/details/gyjxarwub.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.vehdjk.com/Article/details/ggwzgrtlv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gvrkdfwhd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gpmepozup.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gvvchgmnx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gndkqlqbw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.yfazqb.com/Article/details/gqtxjgbyx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gmuktsfaw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.epnwcf.com/Article/details/gitnzibvo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.vehdjk.com/Article/details/gakkgbqtb.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.vehdjk.com/Article/details/gkndmrety.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.epnwcf.com/Article/details/gwourtyph.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlsslewu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gfnybodaj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gejtwhlfu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gondzzaxn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/gmqetbmwh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/ggsxksdqa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.yfazqb.com/Article/details/ghvkjhjpp.sHtML

[K05] 深拷贝对象
来源：http://wap.tarul.cn/Article/details/gjmfkszit.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gdvbaoftz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/gneqsvmok.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gljbpoqgo.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gxsgunkyt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.epnwcf.com/Article/details/gofttvtra.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.yfazqb.com/Article/details/gykehwohd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.tarul.cn/Article/details/gbgurndpx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.vehdjk.com/Article/details/glmcmmbxn.sHtML

[K06] 解析 URL 查询串
来源：http://3g.yfazqb.com/Article/details/gmhalrflc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gpvbmjaua.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.sjlbkw.cn/Article/details/gauohqbtf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/giybhtugr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gwoprzrbo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.bbcook.cn/Article/details/grsbideqn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gjbufsuwm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gctijhvao.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gmioetqlr.sHtML

[K07] 进制转换
来源：http://www.m.share.vehdjk.com/Article/details/gndeokuxj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/grcprtvyy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/gfuxybszr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gtohvpihk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gbxlqhuds.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gjukzsmgu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gjmwxydyv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.yfazqb.com/Article/details/glnmwnryx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/ggsnxtiyc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpgnowkn.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.vehdjk.com/Article/details/giwntlhlb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/golheaqdd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gcthcttgq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gojqeaeey.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/ggqspzsqn.sHtML

Go:   encoding/gob
来源：http://m.share.sjlbkw.cn/Article/details/gudwhtqhi.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gfdopsbvm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gnvuxaygy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/goyalwcyk.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/gtxvvfddl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrtxqhsf.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fktsv.cn/Article/details/gjujmlaym.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fktsv.cn/Article/details/gjihaleef.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.epnwcf.com/Article/details/goiswutfv.sHtML

JS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/glhypfzvt.sHtML

TS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gtewepqew.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gmwfrkoqy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.sjlbkw.cn/Article/details/gzdxpvjti.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fktsv.cn/Article/details/gvcjdxzwq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.epnwcf.com/Article/details/gglkbzybi.sHtML

[L02] 发送 POST JSON
来源：http://www.share.tarul.cn/Article/details/gmnphgcjw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.vehdjk.com/Article/details/grjjxhvlj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.bbcook.cn/Article/details/gdzptqpop.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gfnkbnrfs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gbobbmrhd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/gmevyxfvf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.tarul.cn/Article/details/gclhzyawc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gxzmuvbcc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fktsv.cn/Article/details/gwgbenluw.sHtML

[L03] 设置自定义请求头
来源：http://baike.fktsv.cn/Article/details/gdwscpkcn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/gjkwxnijh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fktsv.cn/Article/details/gkwmlabog.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gbesbqrod.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/groilijjx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.bbcook.cn/Article/details/gdafyqkoe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/glnvhdumn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.epnwcf.com/Article/details/gratjkfft.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gnqbjnylo.sHtML

[L04] 设置超时
来源：http://www.blog.vehdjk.com/Article/details/gheptoizc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.sjlbkw.cn/Article/details/gqyeufqgb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gzxczdxxu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gqprbmwfe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gkuzhsgid.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fktsv.cn/Article/details/gdkmmtpak.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.epnwcf.com/Article/details/ggqslpvjl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gklbiwjcm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.bbcook.cn/Article/details/gguivvpbh.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.sjlbkw.cn/Article/details/goliznxrv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.yfazqb.com/Article/details/gvibhvygs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/gxdvcnsqy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/garndflqj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gbkdmmpoe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/ggwqwaald.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/grjgfexgn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/gaazjlpuy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/gizkvdiln.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.sjlbkw.cn/Article/details/ghbgunxpr.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/goqteylpy.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fktsv.cn/Article/details/gumovwoxx.sHtML

JS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gujezaxhr.sHtML

TS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gqjzrjpoi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gsjnkmazg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.epnwcf.com/Article/details/gbhuirmyd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.yfazqb.com/Article/details/gjigibyxt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.vehdjk.com/Article/details/gfikrtfve.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/gsbvdfmyx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gnboxoptd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.vehdjk.com/Article/details/guujrilms.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gitouekjy.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gmuxowwok.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/grneutgwf.sHtML

Go:   resp.StatusCode
来源：http://3g.fktsv.cn/Article/details/gcexibgck.sHtML

Ruby: resp.code.to_i
来源：http://www.share.sjlbkw.cn/Article/details/gdbbikdlf.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gupkkwjih.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/guwhfcjfr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/gtkdshcun.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fktsv.cn/Article/details/gkilcapgj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gvoqmarib.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gpvdempfh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gkirmimud.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.vehdjk.com/Article/details/ghpdbemmw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.epnwcf.com/Article/details/gnkqgvtcn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.sjlbkw.cn/Article/details/glajbqmqt.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbkmdqdfy.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gnieixxld.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdylmhfkf.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gigdnkorq.sHtML

Py:   sys.argv[1:]
来源：http://3g.sjlbkw.cn/Article/details/gpudzlndi.sHtML

PHP:  $argv;  $argc;
来源：http://baike.vehdjk.com/Article/details/gpvqagugm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/ggvasmbbu.sHtML

TS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gsbrjjgii.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gtsrzrqwb.sHtML

Go:   os.Args[1:]
来源：http://3g.fktsv.cn/Article/details/gyeyhufvg.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gmoztsyfy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/garrhjspf.sHtML

[M02] 读取环境变量
来源：http://blog.epnwcf.com/Article/details/gsjutypqq.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fktsv.cn/Article/details/gfwbgmjjb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gnsjqldjn.sHtML

JS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gyycridnh.sHtML

TS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/ggmuppbuy.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gozmqwzju.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/guztdhjgz.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.yfazqb.com/Article/details/ghntrbzzz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/gnkwoqhlp.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/gpwpbxsab.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.sjlbkw.cn/Article/details/grktfribk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.bbcook.cn/Article/details/girwmdblh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gqslbnhqy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gettpmbjg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gutulfmel.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/ghfqksgyu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gxjyiqsrc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.epnwcf.com/Article/details/gtcyoluvc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.epnwcf.com/Article/details/gjesuzgbo.sHtML

Py:   os.getcwd()
来源：http://www.share.yfazqb.com/Article/details/gyyeylgwf.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/gbkovamba.sHtML

JS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/guexfpidy.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/guzomkvyp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gveugjktp.sHtML

Go:   os.Getwd()
来源：http://read.share.vehdjk.com/Article/details/gpnuknzfd.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/gwhezueen.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gwphpcmpo.sHtML

[M05] 设置退出码
来源：http://www.share.fktsv.cn/Article/details/gbmqlrzmr.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gxqazvtxw.sHtML

PHP:  exit(1);
来源：http://baike.sjlbkw.cn/Article/details/gpvaintjn.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/grwlracbp.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggkknjzoq.sHtML

Java: System.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gngxangtj.sHtML

Go:   os.Exit(1)
来源：http://mobile.yfazqb.com/Article/details/gtsfycgna.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gyzhbcvvh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gwwqfmysv.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gnqmexwob.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gtjdpiuyq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/gfxzsqvnt.sHtML

JS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gjbqnhuwc.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gigguwqrl.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gdncxvukp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/gizycmtsg.sHtML

Ruby: warn "err"
来源：http://read.share.epnwcf.com/Article/details/goleixcav.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.tarul.cn/Article/details/giinuhexw.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/ggqtuclpp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.vehdjk.com/Article/details/gjpchdvcg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gaktrvkor.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gmhqjfvvq.sHtML

TS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/gxsgxsevp.sHtML

Java: public static void main(String[] args)
来源：http://www.share.epnwcf.com/Article/details/gmnovquaq.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gtbmngvss.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/gwaaerhtw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gjqgsbszz.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.epnwcf.com/Article/details/glvdxiejj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.epnwcf.com/Article/details/grllzisnz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/ggqjmzpjx.sHtML

JS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gbymswylt.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gxidjdvpg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/gopjwyabk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/ggscumthp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gqhebvamn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.sjlbkw.cn/Article/details/geyfltcya.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnbrqvqvq.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/ggadizcmv.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfbcemvng.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.epnwcf.com/Article/details/glnreqraf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gsntbtrsv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/gwukilnia.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gngdfuuoc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gjegaychg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gozgfwszi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gvhaolejm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gjpbhqpct.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gqbzyadwb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.bbcook.cn/Article/details/gawdppbbh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/ghtbijlpg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.epnwcf.com/Article/details/gznojlklf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/guzwvsgzb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gqlwvjfum.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fktsv.cn/Article/details/gritluyki.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/ggovehxas.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/groafayha.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/gurcxcfye.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/gaqdcmtpv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.bbcook.cn/Article/details/gjkcevjuf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fktsv.cn/Article/details/gsztbzooj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/giagxbnsx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/grgucwuea.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fktsv.cn/Article/details/gjqvocvup.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gkxihahnk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.sjlbkw.cn/Article/details/gvwgevymw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.yfazqb.com/Article/details/glchhlcti.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.bbcook.cn/Article/details/grdddcxyr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/geecprtud.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gcmmfjcpl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gildkezfk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gmrowbdzj.sHtML


<!-- 参考信息 -->