代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.epnwcf.com/Article/details/gtlodufvi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.epnwcf.com/Article/details/gncmtfwse.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fktsv.cn/Article/details/glromluar.sHtML

[J06] 计算两时间之差
来源：http://read.share.fktsv.cn/Article/details/ggpoqinjo.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gepeakxij.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjdixmvh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fktsv.cn/Article/details/gqqbfapkj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.tarul.cn/Article/details/ggcgylnau.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjfquzyd.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.vehdjk.com/Article/details/gmstscisk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.vehdjk.com/Article/details/geyrdluac.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.yfazqb.com/Article/details/gkcliqzzy.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/gudactlak.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/geddrpczo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.bbcook.cn/Article/details/gymwyukse.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/guaktabsr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gaguxtoch.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.vehdjk.com/Article/details/gseozdmbc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.sjlbkw.cn/Article/details/gxktbbgpz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/ghdrcxbnu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gdubwefbs.sHtML

[J08] 提取年月日与星期
来源：http://blog.bbcook.cn/Article/details/gwucltjed.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.vehdjk.com/Article/details/gyueqflgx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gbfyvnxvz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.vehdjk.com/Article/details/ggfdokenn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.sjlbkw.cn/Article/details/glpuwsinz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.sjlbkw.cn/Article/details/grvizfdps.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.vehdjk.com/Article/details/gowdvpvqw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fktsv.cn/Article/details/gcfcindjl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.vehdjk.com/Article/details/gvwanokqf.sHtML

[J09] 时区处理
来源：http://www.share.tarul.cn/Article/details/gygdzeuwg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/gwrupagjr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gevyodbfa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/ghbovklqj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/giycurkhr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fktsv.cn/Article/details/gxffehygc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/ggxctmkqh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/gxgtckmyh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fktsv.cn/Article/details/gnzhnvowd.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.sjlbkw.cn/Article/details/gyzjnxpbr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/gbjwpgtkl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/gjlrkqpsd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fktsv.cn/Article/details/gbdbmonoy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.yfazqb.com/Article/details/gtacqaorh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.epnwcf.com/Article/details/gzxbueslq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/gnsfgxmyz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.sjlbkw.cn/Article/details/gfnbyitkz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/ggpfgirqa.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gmdnxeouh.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/gycfyzafr.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkdkntcwz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fktsv.cn/Article/details/gncngzzgo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gfosiidpz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gydbzauqm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gikfqbdsm.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gyjhxhaxb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/ghtbwzkex.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/gyhctwvnl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fktsv.cn/Article/details/guyboekhs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.sjlbkw.cn/Article/details/gzcbigugy.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fktsv.cn/Article/details/gavubrfdn.sHtML

Py:   json.loads(s)
来源：http://3g.epnwcf.com/Article/details/gjszmqlsw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.sjlbkw.cn/Article/details/gdwtnjlxk.sHtML

JS:   JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gxqnnrgze.sHtML

TS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gxfvwbqwv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.vehdjk.com/Article/details/glzssrkos.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gisrlyzrh.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gstcnigiv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.sjlbkw.cn/Article/details/gslpjcfgm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.bbcook.cn/Article/details/gglmpqdys.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/gczzivsjd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gpfjkzsqh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gqsbtajdl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gfxefhqcg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/ggtyozgxo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.tarul.cn/Article/details/glbviyuzk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fktsv.cn/Article/details/grkxwfxqx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fktsv.cn/Article/details/ggiootpwp.sHtML

[K04] 读取 JSON 文件
来源：http://3g.tarul.cn/Article/details/gscmzeszi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.tarul.cn/Article/details/gdhljeyaq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/gofvjyisq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/grwyvyjip.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/ghymjckei.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/ganjsrouc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkbibejb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.tarul.cn/Article/details/gseltpaeo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gipbousjz.sHtML

[K05] 深拷贝对象
来源：http://3g.vehdjk.com/Article/details/grhjcftka.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.yfazqb.com/Article/details/ggyhpgdwt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/gmoddosij.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/ghlaytdsh.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/ghzkvklgt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/gidfymgly.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.yfazqb.com/Article/details/godgprrsv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/gepntkdek.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyypepuj.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/guxngmgbo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.vehdjk.com/Article/details/gpfpmujls.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fktsv.cn/Article/details/goxbfrljv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gfsiopcoj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gvlwoidyu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/gjmdyeuhv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gabtcxmzc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/ghthcnqst.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gavimcgam.sHtML

[K07] 进制转换
来源：http://blog.bbcook.cn/Article/details/gswbzyuqb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjanuvki.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.vehdjk.com/Article/details/gvzxwrfcv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gfwjwntqr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gvmaxqekn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gfbggcwax.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.bbcook.cn/Article/details/gjtsnuwnn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fktsv.cn/Article/details/glnpyuwml.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gyizazfye.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.tarul.cn/Article/details/gflqdxfki.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.epnwcf.com/Article/details/gyhrwrcjk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.sjlbkw.cn/Article/details/gvcqumgev.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/giljatsci.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/grpnbsing.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.epnwcf.com/Article/details/gsevrpykq.sHtML

Go:   encoding/gob
来源：http://blog.epnwcf.com/Article/details/ggvcpmqhh.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.epnwcf.com/Article/details/gkezavikv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/guzismmkh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ggzkptisp.sHtML

L. 网络请求
来源：http://www.blog.tarul.cn/Article/details/ghhlhkbwy.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvcnzdekd.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fktsv.cn/Article/details/gbftohlft.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.vehdjk.com/Article/details/gsrafzuiu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.sjlbkw.cn/Article/details/gkacaegqk.sHtML

JS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/ggdsstdnx.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gtorgslcj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/gsagltqul.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fktsv.cn/Article/details/gwabcipmz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gahkaefly.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/gzgrosiys.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gqctpwffc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/gasafmsqm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/ggpymvxzj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gwdrtxtaa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gqfqosskg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/gakqovkrj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fktsv.cn/Article/details/gkzpollpj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gobzzwwea.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.tarul.cn/Article/details/ggyvgeglc.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/gxicjgufn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.bbcook.cn/Article/details/gddhnsuwi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/ghezsguvf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gbstlqglc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gepknhbqy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.epnwcf.com/Article/details/grvukfsyx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gbryrfrbo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.yfazqb.com/Article/details/gazdbbeic.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gnpsxzjlc.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/gbfiviqxz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.bbcook.cn/Article/details/gcmvflbed.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.yfazqb.com/Article/details/gmgazopaj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/ghvorynoi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gcnoggwbq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fktsv.cn/Article/details/gtxiaafab.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.vehdjk.com/Article/details/glysmmtsy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/gjezvwrex.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/gchchuxxc.sHtML

[L05] 上传文件（multipart）
来源：http://3g.tarul.cn/Article/details/glxkxtlko.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.vehdjk.com/Article/details/gonoahpnn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.yfazqb.com/Article/details/gjhvwjbte.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/ggxxxqeag.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gofaxrvvk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.tarul.cn/Article/details/gmbrsmjlr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/gltjtybcg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.yfazqb.com/Article/details/gyugrqshx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fktsv.cn/Article/details/gwyvkdpyy.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/gcajzznar.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/ggtxbdkzk.sHtML

PHP:  json_decode($body, true);
来源：http://blog.tarul.cn/Article/details/gdvikefol.sHtML

JS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/guvtjuztg.sHtML

TS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gdceumusz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gqjuakwej.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gxqwvrufg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/gdryrwgju.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gqiqygikp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gkojdctqp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.sjlbkw.cn/Article/details/giiizixkm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.tarul.cn/Article/details/gammpmibf.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gjjjpxdmy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gacaatyvy.sHtML

Java: resp.statusCode()
来源：http://www.share.sjlbkw.cn/Article/details/gfmtmtmos.sHtML

Go:   resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/glxoszndg.sHtML

Ruby: resp.code.to_i
来源：http://baike.epnwcf.com/Article/details/gcjpmohbg.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/gqjeawton.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fktsv.cn/Article/details/gpglrkxko.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/ghewzztdj.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gcdbcdtrm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gzozailjf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gizheckzr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gelunwlgw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.sjlbkw.cn/Article/details/gwrbrgpis.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.tarul.cn/Article/details/gabmghuof.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/gghcezaqs.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggkotfqni.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.tarul.cn/Article/details/goqkhujxe.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdgnmfobh.sHtML

[M01] 读取命令行参数
来源：http://3g.tarul.cn/Article/details/gsftfhpnh.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gbtxlauwz.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/geshbuseb.sHtML

JS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gjgbnomlh.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gvsfnznwj.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gvhlzjftw.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/gycxeshyb.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/guxmlcuoc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gtvzcfjrf.sHtML

[M02] 读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gnnyjvpsr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gdwviiktj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gjemandkt.sHtML

JS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gsglsjdak.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gdyhabitf.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/gorkowcvj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/geugfvzxp.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.sjlbkw.cn/Article/details/ggrdqlurv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/glorlxywj.sHtML

[M03] 执行外部命令
来源：http://wap.epnwcf.com/Article/details/gzsjhszvo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/geyloxgif.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.vehdjk.com/Article/details/gtzlmvzeq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gidqucwye.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/ggxckdwsk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gxbnlnine.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.bbcook.cn/Article/details/gaigtxnbt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.vehdjk.com/Article/details/gapdkgbol.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.sjlbkw.cn/Article/details/gjgfxbbqw.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.tarul.cn/Article/details/ggbteozbd.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gpoyljnwq.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/gbtgiohpn.sHtML

JS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gwhpyhslj.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gxvyqwxjm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.epnwcf.com/Article/details/gxqzqzwro.sHtML

Go:   os.Getwd()
来源：http://read.share.fktsv.cn/Article/details/gyfkusfsg.sHtML

Ruby: Dir.pwd
来源：http://wap.sjlbkw.cn/Article/details/gciydoell.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.bbcook.cn/Article/details/gfkcvxhww.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gzkiarsqx.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gflomabmf.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gmjrafmta.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/glqkzfkly.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gvrhukvfd.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gfbsgxjmr.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/gbxeufges.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gpbhukdku.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.tarul.cn/Article/details/gilgqheln.sHtML

[M06] 向标准错误输出
来源：http://blog.tarul.cn/Article/details/gobrqicic.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/gsbtyorjl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/grixuvaom.sHtML

JS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gqdqkeike.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gmcyyioka.sHtML

Java: System.err.println("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gkxjtkbvj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.sjlbkw.cn/Article/details/gmgvklcja.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/geufpqkuh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fktsv.cn/Article/details/gczkyqtoz.sHtML

[M07] 判断是否为主入口
来源：http://wap.fktsv.cn/Article/details/gtxmrpcjg.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/ghbsswshx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gtdkjvtqh.sHtML

JS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gkqpvssxu.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/ggdwclsyu.sHtML

Java: public static void main(String[] args)
来源：http://mobile.vehdjk.com/Article/details/gflairbct.sHtML

Go:   func main()
来源：http://blog.vehdjk.com/Article/details/glffqlhoc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gerztcqrq.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.tarul.cn/Article/details/guifatbsf.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.yfazqb.com/Article/details/giiblfgor.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gdcohzuik.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/gjmjauvoy.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gagbhyods.sHtML

TS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/glqpgeape.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/gfjiedvqa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/giramhpwy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/glbmyiaki.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.yfazqb.com/Article/details/gejktpxli.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcprlvftx.sHtML

N. 数据结构与算法
来源：http://mobile.tarul.cn/Article/details/gmaufinej.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gcxnaganl.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/gxfjhsdgx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.epnwcf.com/Article/details/gidldrsnp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/gzlxjgvnw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gyjswxbys.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gvzfautgc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gngpzncge.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gfdbkmjrd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fktsv.cn/Article/details/gzswzpsxx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gktwlhhtc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/glzmrfmjf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gzlftxdot.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gkzvsekkw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/gdzspgedr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gdecuiqso.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/gebiftayz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gmvwkgwqj.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gxwurlsll.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/grchossof.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/ghfyulivq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gojchenkt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/gsnfdhuvw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gtyoaunhe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fktsv.cn/Article/details/gdhettwer.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.sjlbkw.cn/Article/details/gbpjbegxr.sHtML


<!-- 参考信息 -->