代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gbzrgdzhg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.vehdjk.com/Article/details/gnhvxirxo.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.yfazqb.com/Article/details/gaoowllri.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.tarul.cn/Article/details/gvhzqvfhf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.bbcook.cn/Article/details/gxilwxund.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gewbuplgp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/gttoyrmkp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.tarul.cn/Article/details/gnxskvilm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.epnwcf.com/Article/details/ggvegxyik.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.vehdjk.com/Article/details/gaubevjib.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.yfazqb.com/Article/details/glemsfeiq.sHtML

[J06] 计算两时间之差
来源：http://www.share.epnwcf.com/Article/details/gfssbaqxi.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fktsv.cn/Article/details/gyxcxrdan.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gsthlyena.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gtvwyzysq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjvyosgg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.yfazqb.com/Article/details/gnqqrfngu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.bbcook.cn/Article/details/gxikqtawd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.epnwcf.com/Article/details/gkaodjlwh.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.sjlbkw.cn/Article/details/glrzucfck.sHtML

[J07] 比较两个日期
来源：http://3g.vehdjk.com/Article/details/gqbpoqyvu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gcefgvojo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.vehdjk.com/Article/details/gemxieanm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/gkljsjftu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gqnourdjr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/gzsuxfhyq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.epnwcf.com/Article/details/gsxsqaghy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gidrdxukd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gcixurwbv.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fktsv.cn/Article/details/gdsykfhpe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/gzlskjilt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/gqmcqglwu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/grxlepcpm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fktsv.cn/Article/details/gewsmaahh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/golixyqap.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/gjcinaqrp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.yfazqb.com/Article/details/gokjspjnt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.epnwcf.com/Article/details/guigxyrwh.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/gtxfcdqmk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.tarul.cn/Article/details/gwyvnyeqj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/gzmicqgjq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpszdbfyt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gnimeuowv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.bbcook.cn/Article/details/gufujrypp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.bbcook.cn/Article/details/glbhmczvf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/guuespxes.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.tarul.cn/Article/details/gfnojlznf.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/gxvwllzvb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.epnwcf.com/Article/details/gldqytbbe.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fktsv.cn/Article/details/gayycwcma.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.yfazqb.com/Article/details/gsrxiqoao.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.vehdjk.com/Article/details/gysgmbqgz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fktsv.cn/Article/details/galtsyqgf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.tarul.cn/Article/details/ghyenynqk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fktsv.cn/Article/details/gowglujig.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gacztzrxk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjoisafpt.sHtML

K. JSON 与序列化
来源：http://3g.epnwcf.com/Article/details/gjgfgbjsf.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gazwzsywx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fktsv.cn/Article/details/gynzfmbmh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gfzmdbrjw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gjtjnovso.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gczjbdcfy.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gjvmgnrix.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.epnwcf.com/Article/details/gtyeqgpzd.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.yfazqb.com/Article/details/gmfrezhyu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fktsv.cn/Article/details/gtzfnzfiq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/grshhgnrf.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/geonlsurv.sHtML

Py:   json.loads(s)
来源：http://3g.yfazqb.com/Article/details/gpupnfbzd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.bbcook.cn/Article/details/gxsazuadz.sHtML

JS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gypfmuopm.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gqatbajhz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gswtmbpjx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gfxqojbwu.sHtML

Ruby: JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gjggysemv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.vehdjk.com/Article/details/gglneddsu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.epnwcf.com/Article/details/gcicyxrgn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gxqftvcvr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gqjptdgqy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gacqknnez.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/grgupoyft.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.epnwcf.com/Article/details/gndmksztr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gyfnqdtrh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.bbcook.cn/Article/details/gtzjsfwrd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.yfazqb.com/Article/details/gvajqgvom.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.tarul.cn/Article/details/gecewdxoz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/gjvvcuvll.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.yfazqb.com/Article/details/gfxzyivsv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gewvhatiq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gracechzg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gjslytlse.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.yfazqb.com/Article/details/gmozhqeuq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/grbksijze.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.vehdjk.com/Article/details/gqfqrmkxt.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gyjsjajfg.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fktsv.cn/Article/details/gctraxjub.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.vehdjk.com/Article/details/gylakgocp.sHtML

JS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gyenmlhjj.sHtML

TS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/goafwzsfz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.tarul.cn/Article/details/grjgezdhf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.bbcook.cn/Article/details/gpnojpjzo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fktsv.cn/Article/details/gcxhzbqgi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.tarul.cn/Article/details/gjduzhhkv.sHtML

[K06] 解析 URL 查询串
来源：http://blog.tarul.cn/Article/details/gmlurmlni.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/gnzfovkrw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.vehdjk.com/Article/details/gotmlyflo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gmdavqxok.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gqxvibpip.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.sjlbkw.cn/Article/details/glgsakrhr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/gkajgwsxi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gtgdgvvpi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gpfwxympd.sHtML

[K07] 进制转换
来源：http://wap.epnwcf.com/Article/details/gjgiagguq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gsglgfaio.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.bbcook.cn/Article/details/gdkyfuevz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gdwsjawbm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/grgbswdnh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gypleobct.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.epnwcf.com/Article/details/gqmdzdrnh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gkgcoenrq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gpjxkwjde.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/guptckqhr.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fktsv.cn/Article/details/gxbafkhyz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gzqmgzxtk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gpylwmzhb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gkglzubek.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.tarul.cn/Article/details/gcouwweku.sHtML

Go:   encoding/gob
来源：http://read.share.vehdjk.com/Article/details/gagaosjsu.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.tarul.cn/Article/details/gppzgocmt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/grlsifwsv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gvybraffn.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/gcikdspwu.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqkdvtuqn.sHtML

[L01] 发送 GET 请求
来源：http://mobile.tarul.cn/Article/details/gfozmzntt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/gqlnsumbx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/giwqrbjxm.sHtML

JS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gbisgkgse.sHtML

TS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gtycojfkh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.epnwcf.com/Article/details/gktogqyia.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.sjlbkw.cn/Article/details/gnvtwbcmq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fktsv.cn/Article/details/gzaodwmyd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.bbcook.cn/Article/details/gmhzhbhqb.sHtML

[L02] 发送 POST JSON
来源：http://wap.yfazqb.com/Article/details/gqgxyrzmg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gjnqrrrks.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.sjlbkw.cn/Article/details/gupqmozcp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gtrencefd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gbgncvekq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fktsv.cn/Article/details/gpzcigfdg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fktsv.cn/Article/details/ghovwpwxu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/godfcedki.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/gkjepvoxg.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fktsv.cn/Article/details/grjcttndc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.vehdjk.com/Article/details/govmyrisw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gwaebhnsk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/glnwlankv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gxkyfmfnn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fktsv.cn/Article/details/gxgzsgjni.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gaiwgatzt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.sjlbkw.cn/Article/details/gpskmnfis.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gvteoxhzb.sHtML

[L04] 设置超时
来源：http://baike.sjlbkw.cn/Article/details/gmebrksuz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.epnwcf.com/Article/details/gpzuiaiod.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/gyoaohpwv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gumbdvuzx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gwjsvtupi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.epnwcf.com/Article/details/gkkhngabx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.tarul.cn/Article/details/gcrumnghe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/gsayksdpw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.yfazqb.com/Article/details/gjnclvsnr.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fktsv.cn/Article/details/gtysjpwoo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/gbzadwqwl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.sjlbkw.cn/Article/details/gtirnjhby.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/ggyqiswxf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gerhlftyz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.vehdjk.com/Article/details/gryncivef.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.bbcook.cn/Article/details/grqtlnrja.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.sjlbkw.cn/Article/details/gznoypuue.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gvswjsnsb.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.tarul.cn/Article/details/gnbxfovaj.sHtML

Py:   resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gskjnxuwr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/golkbzquq.sHtML

JS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/gbzijjgkj.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gfgzowtkk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.tarul.cn/Article/details/gpqihwcnf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gwwzcikyw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gyjercbmb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.epnwcf.com/Article/details/gezkcyrbr.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gysrxhnlr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/ggdxqeewo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.bbcook.cn/Article/details/gexggljih.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/grzgbrjqm.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gxolvanse.sHtML

Java: resp.statusCode()
来源：http://www.share.epnwcf.com/Article/details/gowfnyvdk.sHtML

Go:   resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gqjlfynzw.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gyumjgtid.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gvvnhrvnl.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/gikfwlvrk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.bbcook.cn/Article/details/gsnggzcgs.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.bbcook.cn/Article/details/guoyqnspa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gdwympwwo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gsebcclfx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.tarul.cn/Article/details/grplsyxas.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gvkiqgllu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.yfazqb.com/Article/details/gvklsqprn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.tarul.cn/Article/details/gsqrdpfuz.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gaudcielu.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fktsv.cn/Article/details/gzgulknyo.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmrjsnwzh.sHtML

[M01] 读取命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/gxgjwwmwx.sHtML

Py:   sys.argv[1:]
来源：http://wap.bbcook.cn/Article/details/gshtaglpk.sHtML

PHP:  $argv;  $argc;
来源：http://3g.bbcook.cn/Article/details/gpmjkqris.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gkocbxlfv.sHtML

TS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/ghpsrxrnu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gyknahodc.sHtML

Go:   os.Args[1:]
来源：http://read.share.tarul.cn/Article/details/guolqyfpw.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gugqfnxuj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/goewdrkaq.sHtML

[M02] 读取环境变量
来源：http://www.share.vehdjk.com/Article/details/gbmwnsakd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gosphvvwg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/gconmaqyj.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gswjnupfv.sHtML

TS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gvwxrjhbs.sHtML

Java: System.getenv("HOME")
来源：http://baike.tarul.cn/Article/details/ggxwaxeau.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/gpikpxsct.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/ggccvlqrc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/ggeczvmaf.sHtML

[M03] 执行外部命令
来源：http://mobile.bbcook.cn/Article/details/gqidprckb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/gtejfkszd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.yfazqb.com/Article/details/gnopwfxkl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gwkeojdxe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gvlbtoaqy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.vehdjk.com/Article/details/gkbehrxuq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gikmlogvs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.vehdjk.com/Article/details/gksxzjjyh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.vehdjk.com/Article/details/gatntptza.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/gofovchkj.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/gdruushmn.sHtML

PHP:  getcwd();
来源：http://blog.fktsv.cn/Article/details/gxxrynmfi.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gfxadzqlq.sHtML

TS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gitjgdrcj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/guqiqcfqm.sHtML

Go:   os.Getwd()
来源：http://mobile.vehdjk.com/Article/details/gsbhdnmdf.sHtML

Ruby: Dir.pwd
来源：http://wap.bbcook.cn/Article/details/glvjeqnfb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.tarul.cn/Article/details/gfhwntrya.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/gfxpsdjyb.sHtML

Py:   sys.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gcpttjnpl.sHtML

PHP:  exit(1);
来源：http://baike.fktsv.cn/Article/details/gahyoqmkf.sHtML

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/ghyunlsdx.sHtML

TS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gupxrvotm.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gnetunrnj.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gtqjwiuia.sHtML

Ruby: exit 1
来源：http://mobile.bbcook.cn/Article/details/gudwwchhd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.vehdjk.com/Article/details/gdjvhceba.sHtML

[M06] 向标准错误输出
来源：http://blog.vehdjk.com/Article/details/gacimmxos.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gpmxtbqxc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.epnwcf.com/Article/details/gqtiwvowt.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gqjmnnlaa.sHtML

TS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/grzfnlfxj.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/gpveebxnb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.yfazqb.com/Article/details/gpcrrrhzo.sHtML

Ruby: warn "err"
来源：http://read.share.epnwcf.com/Article/details/gvoyckhgs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gqxmqqbte.sHtML

[M07] 判断是否为主入口
来源：http://read.share.tarul.cn/Article/details/gfzgngxma.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gmsqdrtki.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.sjlbkw.cn/Article/details/gptbikqrx.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gcjfuiivp.sHtML

TS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gtueevwjk.sHtML

Java: public static void main(String[] args)
来源：http://3g.yfazqb.com/Article/details/gmjsqmytk.sHtML

Go:   func main()
来源：http://3g.epnwcf.com/Article/details/gxqdyilyk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/gemxrnpcu.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.epnwcf.com/Article/details/gtxcudufo.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/gvtlnxdhh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/gkbdfcobn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.bbcook.cn/Article/details/ggrvafwod.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/goheviwww.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gwlasonle.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/gclpfjthd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.epnwcf.com/Article/details/gpsbgonmq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.bbcook.cn/Article/details/gmaymjrcj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.epnwcf.com/Article/details/gaxarngri.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ghemgxdng.sHtML

N. 数据结构与算法
来源：http://wap.bbcook.cn/Article/details/gvnziklzu.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxaoljxwj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gkdkvxplj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/ggtkjjcxt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gpqwqolnb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gclkaawxf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gwwooyusw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gnzrjpzgr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gfjegoigh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.vehdjk.com/Article/details/guwhulell.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gqzeyqrnr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.yfazqb.com/Article/details/gvnleyapz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/gxigrfwkr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.vehdjk.com/Article/details/gaftzgfdx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gyendbwhk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gajlnvdxw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.epnwcf.com/Article/details/gptmcfser.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/giyjupjxy.sHtML


<!-- 参考信息 -->