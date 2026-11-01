代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.vehdjk.com/Article/details/gxgcjcxfb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.sjlbkw.cn/Article/details/gqtaijolz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/gibrsjjcr.sHtML

[J06] 计算两时间之差
来源：http://www.share.tarul.cn/Article/details/gwfggvkpt.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.epnwcf.com/Article/details/gptlveuza.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/gjajrizgx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.tarul.cn/Article/details/gyzhnsdxu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.vehdjk.com/Article/details/gzidakjbt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.tarul.cn/Article/details/gnzgoqwuo.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gnsjxiucs.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.yfazqb.com/Article/details/giulbaayp.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/gynsjiilx.sHtML

[J07] 比较两个日期
来源：http://www.share.bbcook.cn/Article/details/gpngvkbcl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gdzyfhbtv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.tarul.cn/Article/details/gabskroqq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gkeypiirz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/gilrmypbm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gtypgansf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gxqiketcs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/ghaeeqokv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/giwcurewe.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gsoamhytd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.bbcook.cn/Article/details/gxmxberhd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.tarul.cn/Article/details/gudmuabby.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/gnhsbpayj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fktsv.cn/Article/details/gomisqymx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/gdhvwzofg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.bbcook.cn/Article/details/gtwnqtpyt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.bbcook.cn/Article/details/ggvosfdbo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.yfazqb.com/Article/details/gaqtaxwxj.sHtML

[J09] 时区处理
来源：http://www.m.share.fktsv.cn/Article/details/gbejbufcl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fktsv.cn/Article/details/gcgiiwwbd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.vehdjk.com/Article/details/gqajtocsj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gkefzigul.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gydjysqfk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.sjlbkw.cn/Article/details/gavwigivk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.yfazqb.com/Article/details/gkegzuplx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.epnwcf.com/Article/details/gqpzeamsn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gotptbzvu.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.sjlbkw.cn/Article/details/gywozuxgh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.sjlbkw.cn/Article/details/gblomnjma.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.epnwcf.com/Article/details/gqylwdukr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.tarul.cn/Article/details/golzlpnzc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/gfnttbisd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/ghchhveyg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.bbcook.cn/Article/details/gtddjnnqt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.epnwcf.com/Article/details/gpwebdgyg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.yfazqb.com/Article/details/gobwzfkrw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsdznirly.sHtML

K. JSON 与序列化
来源：http://baike.sjlbkw.cn/Article/details/gxetnhsks.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjapyknti.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fktsv.cn/Article/details/glvnhoyry.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gxhjoestc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gfssvgdwg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gqcazauyg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gjrgnwodn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/gshmgqhzk.sHtML

Go:   json.Marshal(obj)
来源：http://3g.vehdjk.com/Article/details/gufozyrzx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fktsv.cn/Article/details/gbppdqkae.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gfeqhjvdv.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/goxoieuln.sHtML

Py:   json.loads(s)
来源：http://www.share.vehdjk.com/Article/details/gqntcqqsu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.epnwcf.com/Article/details/guwromjcw.sHtML

JS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gobriubcv.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/ghqkrkztf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.tarul.cn/Article/details/goydpafuz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/godlhgtfh.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/guasbppil.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/glzkkimsc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/gajodqwim.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gshwekhgk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gmmigojhh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gkmyhdleq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gdfeewyjz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.sjlbkw.cn/Article/details/gdnaulnpj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjopuxvo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gjymwybic.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.sjlbkw.cn/Article/details/gyberqoob.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.epnwcf.com/Article/details/gtymmclzz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/gcnctfvll.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.vehdjk.com/Article/details/gzsbihape.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gnnqwsuki.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gxawknvdq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.bbcook.cn/Article/details/grhmtsbvp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fktsv.cn/Article/details/gehryvaoc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.vehdjk.com/Article/details/gjuzyidlq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.yfazqb.com/Article/details/gdpmfkbzl.sHtML

[K05] 深拷贝对象
来源：http://read.share.vehdjk.com/Article/details/gbybjdniu.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/gfqpsshlc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.vehdjk.com/Article/details/genkmuenf.sHtML

JS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gmrtbkvrj.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gghhuuuaf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.sjlbkw.cn/Article/details/ghnuzhitg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.yfazqb.com/Article/details/gvkgcezkj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fktsv.cn/Article/details/gfxkujhpk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.vehdjk.com/Article/details/gffkfrzkv.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/gyggsdfui.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/glxrnlbtn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.sjlbkw.cn/Article/details/gjfpvsesr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gwckmqcbr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/ghuhtcnlc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gaxqmjanf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gvpengfqm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gvzlnlvfc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gukaoqsdx.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/gtuxpikln.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gcmvgnkqk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/gdjaorcfx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gpcunnwjj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gphbmoojs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gmxwrmoqk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/gpycasifi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.yfazqb.com/Article/details/goxugppka.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gbeayulkr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/gfanighgg.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fktsv.cn/Article/details/gjwgqmttr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/gmxhwdfwk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gtkolerbg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/grwmrglcf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/ghybuzpuz.sHtML

Go:   encoding/gob
来源：http://baike.vehdjk.com/Article/details/gbliwwcbt.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.yfazqb.com/Article/details/gwtlgexnt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gicysdpik.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/giwlatbmu.sHtML

L. 网络请求
来源：http://3g.yfazqb.com/Article/details/gydrnpkyt.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gidrlduxm.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/gmlbxepbr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.bbcook.cn/Article/details/gtnsfhwaq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.bbcook.cn/Article/details/gymrnqrwn.sHtML

JS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/gzhtyapck.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gxqactucr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.sjlbkw.cn/Article/details/gdilbwvxz.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/giydwqrql.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.tarul.cn/Article/details/gegsibipb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.vehdjk.com/Article/details/gkxlpydzu.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/gksabrxkb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gkpmdkdwb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.bbcook.cn/Article/details/grjmkdjue.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gyuhnduwy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gijyrivbm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.yfazqb.com/Article/details/gtegztqbf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.yfazqb.com/Article/details/gqqxutqlr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.sjlbkw.cn/Article/details/gepsuzhrj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.epnwcf.com/Article/details/gcmaiafny.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/gjhngfzwt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.tarul.cn/Article/details/gyhkiqytw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.tarul.cn/Article/details/gkqnnlpjf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gbsuleded.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gqbdnypim.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.yfazqb.com/Article/details/gtgggogfs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gfmkubrjo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/gibegbihm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gttloewfy.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/grilwexlf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.yfazqb.com/Article/details/gcopqksku.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.sjlbkw.cn/Article/details/gtdicrlfh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gucnwrtld.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gbkgnlrff.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.epnwcf.com/Article/details/gkdghlers.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fktsv.cn/Article/details/gahnmcmlu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.bbcook.cn/Article/details/gydqrwbbg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.vehdjk.com/Article/details/gpiecknyv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gnlxxjlwe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fktsv.cn/Article/details/gkqgzfyru.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/gygwuvibt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/goxzdklhn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gpdstowup.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.vehdjk.com/Article/details/grihwfpzr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.yfazqb.com/Article/details/gmahdrcrt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/gxuohhyqk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fktsv.cn/Article/details/gfdebbtwu.sHtML

[L06] 解析响应为 JSON
来源：http://baike.bbcook.cn/Article/details/gdticoteg.sHtML

Py:   resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gbfnuqvhw.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/glpeanbvw.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/guunmwkmu.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gsewgxrbc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.vehdjk.com/Article/details/gcsoxwqof.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/gndljqlku.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.tarul.cn/Article/details/gojlizsoi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.sjlbkw.cn/Article/details/gncoilboh.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/grgmvlrbn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.tarul.cn/Article/details/gioeutycl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fktsv.cn/Article/details/gtonssqne.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/geaflhcvd.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gzqoudsge.sHtML

Java: resp.statusCode()
来源：http://read.share.fktsv.cn/Article/details/gpodugjau.sHtML

Go:   resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/grnuozvux.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/gxlqqmhew.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gvmyoftgo.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/glwipzhqj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/gcclcburh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.sjlbkw.cn/Article/details/gnhdqtnls.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gbeftpisl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gsqxcipcj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fktsv.cn/Article/details/gfabmntze.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.sjlbkw.cn/Article/details/gunvlwkjp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gtyppfddf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/gfktfamhq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtfyqibno.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.sjlbkw.cn/Article/details/gdnqoxnvo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/glaarucqo.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/gumrhiynu.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gxmahkceg.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.sjlbkw.cn/Article/details/gfztajumh.sHtML

JS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gcounquos.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/ghpjztuba.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gfgqzdgvp.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/gigkrwepn.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/ggcgelpaj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gyekzkrwn.sHtML

[M02] 读取环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gihkshlor.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.tarul.cn/Article/details/gqfogrvwg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/gcagtnven.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gxqkgctso.sHtML

TS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gackkjucc.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/ghuoemfse.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gtlxflueb.sHtML

Ruby: ENV["HOME"]
来源：http://3g.sjlbkw.cn/Article/details/gzugbbdjz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.yfazqb.com/Article/details/gexlnukic.sHtML

[M03] 执行外部命令
来源：http://3g.bbcook.cn/Article/details/gxgpckflc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/ghqskjion.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.vehdjk.com/Article/details/ghsxffdnu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gsrkzeyuh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gyrojbkoa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/gidkqzsxm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.vehdjk.com/Article/details/gdogelmzp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/gszpzxwya.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.yfazqb.com/Article/details/gjpudztyo.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gsvflnpan.sHtML

Py:   os.getcwd()
来源：http://wap.sjlbkw.cn/Article/details/gqouazlbg.sHtML

PHP:  getcwd();
来源：http://m.share.epnwcf.com/Article/details/gjlclardz.sHtML

JS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gtfsftvdq.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gujpyyhgo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.tarul.cn/Article/details/gpkqvvmpx.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gljgjuyyw.sHtML

Ruby: Dir.pwd
来源：http://mobile.vehdjk.com/Article/details/gmtwgeeiv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/gfrsknbeo.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/gpqtftlkh.sHtML

Py:   sys.exit(1)
来源：http://baike.vehdjk.com/Article/details/gyrgxtgie.sHtML

PHP:  exit(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgdvoihn.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gxfkykeyh.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/giaqemvik.sHtML

Java: System.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ginqsowdu.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gbfrzsvzg.sHtML

Ruby: exit 1
来源：http://mobile.sjlbkw.cn/Article/details/gqmmadhlt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.sjlbkw.cn/Article/details/gnqxgzfdq.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gcjhtzjee.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gxnsnqceg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/gbfrgxwij.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gizlolkxw.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gksceenxs.sHtML

Java: System.err.println("err")
来源：http://baike.tarul.cn/Article/details/grieqjthx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/gpvrrawbg.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/ggkcwqulm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.bbcook.cn/Article/details/gkkagzbkn.sHtML

[M07] 判断是否为主入口
来源：http://3g.sjlbkw.cn/Article/details/gehjfkviv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/ghubqbhcl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.yfazqb.com/Article/details/ghqpslczz.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/glgkdddhb.sHtML

TS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gbznjyblm.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gslibmlpz.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gjzxiohqu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.epnwcf.com/Article/details/gkgjemiza.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/gofeqjurr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.sjlbkw.cn/Article/details/gmzyvyzih.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.yfazqb.com/Article/details/gwyhiynmr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.sjlbkw.cn/Article/details/gqqjvloub.sHtML

JS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gtfcsvxnh.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/grepzzutm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.tarul.cn/Article/details/gszwfmrmi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/gmszhsscj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.epnwcf.com/Article/details/gisyeozwp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/gjmupynwv.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/girljrtwh.sHtML

N. 数据结构与算法
来源：http://blog.bbcook.cn/Article/details/gauzserob.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gyzexorau.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.yfazqb.com/Article/details/gthabvttu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.epnwcf.com/Article/details/gwdukaprl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.tarul.cn/Article/details/gixxliknt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gzrqnhtdq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/goddbupar.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gtcdwnlug.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gobksveuw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.tarul.cn/Article/details/ggghzfwlj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/garigvlyt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/gqofaphze.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gqgjpynnj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/grcwsjzjw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gwqjsumtn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gcwsfuups.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/gwtkokxod.sHtML

Go:   slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gvqcsrrho.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/glebxotpc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.sjlbkw.cn/Article/details/gxjznvwkf.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.sjlbkw.cn/Article/details/gpgvrujwr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.epnwcf.com/Article/details/gmdazxmqk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.bbcook.cn/Article/details/gntglfnum.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gfbwvrohb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gkdquwstq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gftcdpcmj.sHtML


<!-- 参考信息 -->