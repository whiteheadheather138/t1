代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gnczqfzlc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.tarul.cn/Article/details/grrjimcnn.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.yfazqb.com/Article/details/gktqwvlro.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.epnwcf.com/Article/details/gmkbdrdwq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.tarul.cn/Article/details/gzjirewlh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gbvqgpyqm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gbiznhzdb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/gpjvitbze.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.epnwcf.com/Article/details/gmeophcyh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/gvezfarkp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.bbcook.cn/Article/details/gttnsusou.sHtML

[J06] 计算两时间之差
来源：http://blog.yfazqb.com/Article/details/gjscopuaw.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.vehdjk.com/Article/details/gczotxgys.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/gqyciggzx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/gupqynnun.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.bbcook.cn/Article/details/gupwuzojv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.vehdjk.com/Article/details/gmhdxulzt.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gpvtwphom.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/gqnhuiyug.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.bbcook.cn/Article/details/gspyjlqmp.sHtML

[J07] 比较两个日期
来源：http://m.share.yfazqb.com/Article/details/giejbzmfc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gboeoxgsr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.yfazqb.com/Article/details/giopctdej.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gnqldknvq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gzjpxedkl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.yfazqb.com/Article/details/gowiydpfx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gxexpfqmr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gssocxrlg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/grrkuoryu.sHtML

[J08] 提取年月日与星期
来源：http://baike.tarul.cn/Article/details/gybsxhwgb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fktsv.cn/Article/details/gqqvujwxm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.bbcook.cn/Article/details/gwzdtfteo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.yfazqb.com/Article/details/gvcaalndx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.epnwcf.com/Article/details/gawnsumqy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.epnwcf.com/Article/details/ghcowbwgm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.bbcook.cn/Article/details/glnswwshf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.vehdjk.com/Article/details/ghoyegprv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.bbcook.cn/Article/details/gwcnlqjfg.sHtML

[J09] 时区处理
来源：http://mobile.sjlbkw.cn/Article/details/gjxgmwfkw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.vehdjk.com/Article/details/ghyrwzohu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.tarul.cn/Article/details/gdtfekdaq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/geokksgqr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/goqeuobop.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.vehdjk.com/Article/details/gbnteorml.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.sjlbkw.cn/Article/details/gwvobtezn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gespheklm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.sjlbkw.cn/Article/details/gkafxvqmn.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.vehdjk.com/Article/details/gomtjnmjy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fktsv.cn/Article/details/gwswmvtyr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gfyyuxyfy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.tarul.cn/Article/details/gkwckwsci.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fktsv.cn/Article/details/gtykuiloe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/ghexbxzmk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.sjlbkw.cn/Article/details/gxqmdnfeu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.tarul.cn/Article/details/gpktmbqjg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.sjlbkw.cn/Article/details/gwstiitwn.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqyraxsnx.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/gseyrhinj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfdczojkv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.epnwcf.com/Article/details/grknihaqs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/glvszmqez.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/gdlxrvqcj.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gyzwdbgmu.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gwflqzsoc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/gxgkypeec.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/ggwifvhaq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.yfazqb.com/Article/details/gkprnwaqb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/gsmrigltr.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gobeeuezl.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/gaupbefni.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.epnwcf.com/Article/details/gphjtojfi.sHtML

JS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gnhrdnxbt.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gtmwndjse.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.yfazqb.com/Article/details/goxwptubi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gngxlshyy.sHtML

Ruby: JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gogctykam.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fktsv.cn/Article/details/glnsfokbh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/glqxxpnen.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gbljgzmdm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gicphpgij.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/geojdrjiy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gxoytdiba.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.vehdjk.com/Article/details/gkitbvcfc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fktsv.cn/Article/details/ghlanbezy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.sjlbkw.cn/Article/details/gcxicrzcn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.vehdjk.com/Article/details/greithjxf.sHtML

[K04] 读取 JSON 文件
来源：http://3g.vehdjk.com/Article/details/gpsrqsrxt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.bbcook.cn/Article/details/gelaylwtl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/gqkkbmrly.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gcfzfphkd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.yfazqb.com/Article/details/gsjilfuqn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.epnwcf.com/Article/details/ggakyepin.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gqekdbhbp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gwqdzskem.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gkznneaag.sHtML

[K05] 深拷贝对象
来源：http://blog.vehdjk.com/Article/details/gtyjdfnhp.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.bbcook.cn/Article/details/gfsjmlqbu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/gjrkpopcz.sHtML

JS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gaxjegnro.sHtML

TS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gnekaiakh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.vehdjk.com/Article/details/gtrnavvgi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.epnwcf.com/Article/details/ggnsxoeum.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/glvjiamte.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.yfazqb.com/Article/details/ggccjrsbo.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/gpxchlebk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gitxrblsb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.tarul.cn/Article/details/gbjhgrepz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/giwwixntw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gcimswuqk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.bbcook.cn/Article/details/ggnjofjtv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gfrhwdehi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gaygpwxnk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gdhjjyssl.sHtML

[K07] 进制转换
来源：http://baike.fktsv.cn/Article/details/gpeupefeb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gltaolppb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/gmqnjkxwl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gscqsmmbq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gpgnasenc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/grwinnbnr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.epnwcf.com/Article/details/gikblxgkp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.epnwcf.com/Article/details/gerbjozdd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.yfazqb.com/Article/details/ghuzmtjfg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.tarul.cn/Article/details/gdmwmoubl.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.tarul.cn/Article/details/gblaooibs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fktsv.cn/Article/details/gftfnpjpf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/ghflshvha.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gsilxdsfe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.sjlbkw.cn/Article/details/gfqshanby.sHtML

Go:   encoding/gob
来源：http://m.share.tarul.cn/Article/details/gpuxacrht.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fktsv.cn/Article/details/gdhhgojeh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gscqyillq.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gayyeqaxi.sHtML

L. 网络请求
来源：http://baike.vehdjk.com/Article/details/gpodppafv.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glxcopzfm.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gmfynmskn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gmgkmztkq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.tarul.cn/Article/details/gzfemcovj.sHtML

JS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gcmqbopcg.sHtML

TS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/ghmpgmdkk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gcwaldptr.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.epnwcf.com/Article/details/gtehbsyxe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.vehdjk.com/Article/details/grhybzpeh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.vehdjk.com/Article/details/gpvomoncw.sHtML

[L02] 发送 POST JSON
来源：http://m.share.tarul.cn/Article/details/gpmslaohg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gwetsyxrd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.yfazqb.com/Article/details/gvxslliud.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gwcurniif.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/guckrvjgt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gmdtvjjta.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.vehdjk.com/Article/details/gkziaxyzb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.bbcook.cn/Article/details/gwnqzcffi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gbafxtkfu.sHtML

[L03] 设置自定义请求头
来源：http://read.share.vehdjk.com/Article/details/gfxtouexw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gnfftwbgf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/gbibowqlf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gideiqqsb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/grsxshsdt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/glsiafrip.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gaihelxey.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.sjlbkw.cn/Article/details/gbbqijyzm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/goaudajcl.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gdsxddmvu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/gjxfwioce.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.yfazqb.com/Article/details/gxttjumqv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gnenmjnxn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/ghtvfhyuz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.bbcook.cn/Article/details/gvfbawfyx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/gezfqbmjo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.tarul.cn/Article/details/gadaggegn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fktsv.cn/Article/details/gfhojyjww.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.bbcook.cn/Article/details/gxfzcdtdo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.tarul.cn/Article/details/gwsfzhhcs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gwmiyftbb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gbbeibntt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/geqyeoopj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fktsv.cn/Article/details/gzhclprks.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/grsmihafw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gaqxrpcbi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/goczodrbm.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gznmndjbj.sHtML

Py:   resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/glzobkxyq.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gzdugyogf.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gpnnmwwci.sHtML

TS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gtqjaltkk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gicciajsz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.bbcook.cn/Article/details/goexvsxcb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.yfazqb.com/Article/details/gaycnnguw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.yfazqb.com/Article/details/ggxzsmpnd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gwsahamqr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.yfazqb.com/Article/details/guyugdnps.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.yfazqb.com/Article/details/gpnxckzef.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/glxihrvsc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gtzisfjrz.sHtML

Java: resp.statusCode()
来源：http://wap.tarul.cn/Article/details/gguewdnxg.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gcdznkgbv.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.tarul.cn/Article/details/gitegwcdw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gmsfimqtx.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.epnwcf.com/Article/details/gztwrnbmb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/gkewusnqm.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.vehdjk.com/Article/details/glqgypzvg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gqaafvqnv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gtzggsswc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fktsv.cn/Article/details/gixtkzhur.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/gdmvtqsdu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gthldjtdx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.epnwcf.com/Article/details/gmezcsnuo.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gykyydjhc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/gdzzoypel.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gledhhzvu.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gxspbzacb.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gntsihyeh.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/glemnorhq.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/ghkqqlzzh.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gtoigrazg.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gngbzexka.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gxmtjzecm.sHtML

Ruby: ARGV
来源：http://baike.fktsv.cn/Article/details/gsmhzdnvh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gfffbpskl.sHtML

[M02] 读取环境变量
来源：http://blog.vehdjk.com/Article/details/gbhgfihlh.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gvbtotzmu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gdmgdwusq.sHtML

JS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/gbunyunoe.sHtML

TS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gffnejcbq.sHtML

Java: System.getenv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gmrutgmlz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gegpsfiar.sHtML

Ruby: ENV["HOME"]
来源：http://baike.vehdjk.com/Article/details/ghzqwsvbi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.bbcook.cn/Article/details/gpxmkwsxl.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoymdpxe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/gmupsxzqq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/gpzkkhend.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gorngqiaj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gitumeamo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/gthfzteme.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gncsncbog.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.sjlbkw.cn/Article/details/gpefbaedm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.bbcook.cn/Article/details/glyaevvje.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gloriikjv.sHtML

Py:   os.getcwd()
来源：http://www.share.bbcook.cn/Article/details/gbodariph.sHtML

PHP:  getcwd();
来源：http://www.share.tarul.cn/Article/details/gzxafwdiy.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gjmrvqpax.sHtML

TS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/glepifrev.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/gikkhwscy.sHtML

Go:   os.Getwd()
来源：http://blog.fktsv.cn/Article/details/gjrtdtguq.sHtML

Ruby: Dir.pwd
来源：http://baike.vehdjk.com/Article/details/gmtgrqlog.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.sjlbkw.cn/Article/details/ghxammjmj.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/gawhzcwra.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gokqydpsn.sHtML

PHP:  exit(1);
来源：http://m.share.tarul.cn/Article/details/gedpuozvw.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/ggxcukqhb.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gmxfejige.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/glcmwzrqh.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/guznpxhtd.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gbpqkvhoo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fktsv.cn/Article/details/gyaldzgej.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gqaaglhcu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/genlxbplc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.tarul.cn/Article/details/gmfvjdmit.sHtML

JS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gmsrbtgce.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gzzxjetza.sHtML

Java: System.err.println("err")
来源：http://3g.epnwcf.com/Article/details/gqzuexndr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/geznilctp.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gvusiegjb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.yfazqb.com/Article/details/gsmofavzw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.epnwcf.com/Article/details/graikuawj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.yfazqb.com/Article/details/gottukypj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/gozpmuphy.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/glyvujqme.sHtML

TS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gixrkfohx.sHtML

Java: public static void main(String[] args)
来源：http://mobile.vehdjk.com/Article/details/gcbsxjgel.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gqdxciyyo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fktsv.cn/Article/details/gimxaauvj.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fktsv.cn/Article/details/guaifrebf.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fktsv.cn/Article/details/gzvtkclss.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.tarul.cn/Article/details/givkuteww.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/gkhgkcjjl.sHtML

JS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/grsulvxab.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gimycgxsw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gienpednh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gflscontu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gjmxnszxg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/gyqqmypwq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpqpzihbx.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gdbnfcekq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzrgycjph.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.bbcook.cn/Article/details/gvgnfjmog.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gojukozyc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/ghecaakvs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gnjoruuwq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gmhbulgbt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gljpdkcgc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gkkduzufj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gwbybsslv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/ghibzlsxw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fktsv.cn/Article/details/gcxrrszlk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/ghohvuklh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gepydwqqb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gfhhggajg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/glglbctxc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.sjlbkw.cn/Article/details/gftghioqu.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/griyuxhrb.sHtML


<!-- 参考信息 -->