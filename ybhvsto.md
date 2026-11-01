代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.sjlbkw.cn/Article/details/gurfmulrs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fktsv.cn/Article/details/gyhabepst.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.epnwcf.com/Article/details/gombfrndd.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/gwpdvcpqu.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/gtqnttvut.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.yfazqb.com/Article/details/gzqmostxp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.yfazqb.com/Article/details/gisdnfpjx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.bbcook.cn/Article/details/gidjtcxjh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/gdoagfnhf.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.epnwcf.com/Article/details/gztrlcpbr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.tarul.cn/Article/details/gwchcsfii.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.yfazqb.com/Article/details/gbrqyzfpl.sHtML

[J07] 比较两个日期
来源：http://blog.fktsv.cn/Article/details/gyxdyzryq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/getofpmfa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.tarul.cn/Article/details/goccjzhbv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gfwgrqjie.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/gqpqvvrla.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fktsv.cn/Article/details/gqbbpzrte.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fktsv.cn/Article/details/gazvrohbk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/ghjsqvyah.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gfutwltwk.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fktsv.cn/Article/details/gelbyzrtr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.bbcook.cn/Article/details/gooabcpjo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.epnwcf.com/Article/details/gtxfaonmy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.bbcook.cn/Article/details/gmcftksqi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.vehdjk.com/Article/details/gwslruxry.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/gzvuxglkj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.vehdjk.com/Article/details/gdalpxqzt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.epnwcf.com/Article/details/gdxaqsvhi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.vehdjk.com/Article/details/glhpqjqtn.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/gaonfwafj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.sjlbkw.cn/Article/details/girrfahtd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.vehdjk.com/Article/details/gaqsqrzer.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/ganuxzimd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gbjlylyji.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/gdlzciqix.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fktsv.cn/Article/details/girmrpcyb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.epnwcf.com/Article/details/gahxhpujl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fktsv.cn/Article/details/gllernczk.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.yfazqb.com/Article/details/gsrmfccop.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fktsv.cn/Article/details/geaiaitxw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.yfazqb.com/Article/details/grkagbxpg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/gkhiwwkbq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.sjlbkw.cn/Article/details/goirqdzzx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.yfazqb.com/Article/details/ghjpkeqij.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.epnwcf.com/Article/details/gmqdaafda.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fktsv.cn/Article/details/gbbiwtgsi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.vehdjk.com/Article/details/gwttxtnxo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnwscenau.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/gzrgrikwn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gobxfyhkg.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fktsv.cn/Article/details/gfpvlpkht.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gopryrjgy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/glfuyouat.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/gvfqhhzva.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gefkbyxaw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fktsv.cn/Article/details/gdlulbfyk.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.bbcook.cn/Article/details/gstfgktgv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.yfazqb.com/Article/details/grrjmqhup.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.epnwcf.com/Article/details/gsrsknxmd.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fktsv.cn/Article/details/gsemkegid.sHtML

Py:   json.loads(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfipgkmwa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gietwaddq.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gxijwdtbv.sHtML

TS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gayvqarch.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gdigfujka.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gpkcewqmp.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gitczrphc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.epnwcf.com/Article/details/gkuohwcgh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.vehdjk.com/Article/details/girdfichl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gkigocyar.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/gebljarmj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/ghhsxiztf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gdweneepn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.bbcook.cn/Article/details/gupywyiim.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fktsv.cn/Article/details/gnbimtphe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/grcicfrca.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.tarul.cn/Article/details/ggrbswkgr.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.epnwcf.com/Article/details/gbopxgcii.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/gsmpltbny.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fktsv.cn/Article/details/gcluueocv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.tarul.cn/Article/details/griteescx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gpgvdsonu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gviuarmmk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gkdlcebkl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.epnwcf.com/Article/details/gtujrzsip.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/ggbgmxxda.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.yfazqb.com/Article/details/gzsfslgmg.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.tarul.cn/Article/details/grtlbjcce.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gfgbgnrpy.sHtML

JS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gpbxcpbll.sHtML

TS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gtfuynqqz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.tarul.cn/Article/details/gmswrhiae.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.vehdjk.com/Article/details/gsdwgsvkw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gzwlxsxbn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gnsfvqtks.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.vehdjk.com/Article/details/gbmuzqsmu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gzrtmnkgl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.epnwcf.com/Article/details/gkwdhvrmk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/ggntvhysk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/gezjdgfbp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gqmxfpgmm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gfpiapocv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/grtdyuetu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gfxkojwhc.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/gsrpezeli.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gfzzfayai.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.bbcook.cn/Article/details/grvyrsjut.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gpisyofwc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gstkmchqw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gaaisftqt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/gcyyjldfo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.vehdjk.com/Article/details/gikcaxkjz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gmqkngskf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/gtnlolfap.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/gsxsgakhu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.yfazqb.com/Article/details/ghhenyfji.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gtlhezyfu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/goxfrulvo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.yfazqb.com/Article/details/grywsxqvt.sHtML

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/gksgjptnk.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.epnwcf.com/Article/details/gnfhtmbro.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.bbcook.cn/Article/details/grruyofva.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjvugxgom.sHtML

L. 网络请求
来源：http://www.share.vehdjk.com/Article/details/gxwxnwgrl.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfxaaibzv.sHtML

[L01] 发送 GET 请求
来源：http://blog.epnwcf.com/Article/details/gbkuwgbnd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.epnwcf.com/Article/details/gfdtrcidk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.vehdjk.com/Article/details/gfowjoafh.sHtML

JS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gdaxixydz.sHtML

TS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gavyevcpg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/gdmbsmyao.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/gmvtkwnxf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/gbbgqahba.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/gisqznflo.sHtML

[L02] 发送 POST JSON
来源：http://www.share.yfazqb.com/Article/details/gytyxdnnv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gislahyun.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gsfemqswe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gnusvtfgd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gcinqxduf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/gdojbrevm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.bbcook.cn/Article/details/gbrkodeya.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.tarul.cn/Article/details/gtelszlyw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/geiowgcqj.sHtML

[L03] 设置自定义请求头
来源：http://3g.bbcook.cn/Article/details/gyrdhvutw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.yfazqb.com/Article/details/gdzrynvep.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gglzqktan.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/guaikvigb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/grluppolx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fktsv.cn/Article/details/gmtyofzff.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gpgfnvjjw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/gmmbpfusn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gcxroljge.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/geyierfqx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.yfazqb.com/Article/details/gofghslqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.vehdjk.com/Article/details/gkhvqchvv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gocukozul.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/geqnopuhc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.vehdjk.com/Article/details/ggylztbvc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gwvirfacq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.tarul.cn/Article/details/greipgqrp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/gxmmsnimm.sHtML

[L05] 上传文件（multipart）
来源：http://baike.epnwcf.com/Article/details/gaqqvuuvi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/gvfwoclqv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.vehdjk.com/Article/details/gbeodlynx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gxruqzbgw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/gwdyyzfhu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.sjlbkw.cn/Article/details/gwakwefth.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gcigggecq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/gdtcrvktp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fktsv.cn/Article/details/gwkcwgczc.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.bbcook.cn/Article/details/gplluhbme.sHtML

Py:   resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gmjenrbjh.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/gdrtnlzyx.sHtML

JS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gtyjoncee.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gnxotkywy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.yfazqb.com/Article/details/gttkobzuu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.yfazqb.com/Article/details/gonpnzyom.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.epnwcf.com/Article/details/gujlwbdfz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/grpjpcfhx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gzigeikcr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/ggevrnvpw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.bbcook.cn/Article/details/gdbrafgen.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gjicvrbwl.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/gjeyztkik.sHtML

Java: resp.statusCode()
来源：http://baike.bbcook.cn/Article/details/gvmnvnvud.sHtML

Go:   resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gkjihplen.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gibmutxzw.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/giuiqibqx.sHtML

[L08] 并发请求多个地址
来源：http://mobile.vehdjk.com/Article/details/ghbjsmdcx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.epnwcf.com/Article/details/gnhszchqf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/ggruxgfiy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gauikamfj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gfinobkmj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gqjpgohng.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/ghhbnfmhk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/gxlbknvwk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gtogjkcxd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjqinoahe.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.tarul.cn/Article/details/gofrpvhjl.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gewmxxyqb.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fktsv.cn/Article/details/ggeelalql.sHtML

Py:   sys.argv[1:]
来源：http://wap.yfazqb.com/Article/details/gbfqrmsak.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gezlojlko.sHtML

JS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gpzlqahtp.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gvdvuzzxr.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gtgnvnyru.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/grkrzwwfs.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gypjirkxr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gfphtagii.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gwwmqwsgj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gvkhdkady.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gvezqqymd.sHtML

JS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gommmnjuf.sHtML

TS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gouxghngg.sHtML

Java: System.getenv("HOME")
来源：http://blog.bbcook.cn/Article/details/gagmofmit.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gzhvcfwfs.sHtML

Ruby: ENV["HOME"]
来源：http://wap.tarul.cn/Article/details/gbttzuxka.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gxgjgwcla.sHtML

[M03] 执行外部命令
来源：http://3g.sjlbkw.cn/Article/details/glikeztdm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/ggqmkumyp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/gdtilzmjq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gujaciugp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gkdpmnwgf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.vehdjk.com/Article/details/gawifsxuo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/gustzrlyp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.yfazqb.com/Article/details/gmkvdggwk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.sjlbkw.cn/Article/details/gciseplrr.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.tarul.cn/Article/details/gbbazgnqx.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/guqqaxryc.sHtML

PHP:  getcwd();
来源：http://blog.tarul.cn/Article/details/givlqdzif.sHtML

JS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/ghdukfjxs.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/grmiabrew.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.sjlbkw.cn/Article/details/ghckxhlnp.sHtML

Go:   os.Getwd()
来源：http://baike.sjlbkw.cn/Article/details/gnqtfyobg.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/gdzqrzfru.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.tarul.cn/Article/details/glyngshxo.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/gxqatxwnu.sHtML

Py:   sys.exit(1)
来源：http://baike.vehdjk.com/Article/details/galqtpnnz.sHtML

PHP:  exit(1);
来源：http://blog.vehdjk.com/Article/details/grlglkowt.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/ggdvasjlw.sHtML

TS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/guxgzzrht.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gnzyvzasw.sHtML

Go:   os.Exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gkbtjzppm.sHtML

Ruby: exit 1
来源：http://www.blog.fktsv.cn/Article/details/gkdfilqrd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gmflbjfwt.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/gitkybkcc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gfbilkypj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gvajqfkvy.sHtML

JS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/gktydrcdo.sHtML

TS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gqkrmhxiq.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gvfqrotyo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fktsv.cn/Article/details/gspromewf.sHtML

Ruby: warn "err"
来源：http://m.share.bbcook.cn/Article/details/gtttutsqu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/gbcdubbbu.sHtML

[M07] 判断是否为主入口
来源：http://blog.yfazqb.com/Article/details/ggiqozkyw.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/gsnhgfyfq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.yfazqb.com/Article/details/gjmkunsal.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/geaukkmqo.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gfomnpksh.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gihqbmwqr.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/gcotavtcj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.yfazqb.com/Article/details/gdavohzai.sHtML

C#:   static void Main(string[] args)
来源：http://blog.bbcook.cn/Article/details/gylfakdqp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/gtsxkqacv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/grvamrwdk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.sjlbkw.cn/Article/details/gjitcsoot.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gviqryktj.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gevgckybq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.sjlbkw.cn/Article/details/gxsgjaknq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gonyotzew.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/gzhleowfs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gzbxgqjez.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/giuhzrzmi.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/ggmgzbslc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdnujihsa.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/gntixmdrf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gykhphglt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.tarul.cn/Article/details/goezzxvkt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gajcbykqf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gmgoivqrh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gfzpucykh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gwtvoxydh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.bbcook.cn/Article/details/gdkgrbpxt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gmngkptzg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/gvjstietw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gesphcpwm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gkgjfxipd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gqbxdcihl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/gvwpctadw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/gqkzvdxcl.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gdcbzdhzr.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gjqpzsceb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.vehdjk.com/Article/details/gwlqmoybu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.epnwcf.com/Article/details/gkfimkcsi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/groncjliz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fktsv.cn/Article/details/gntivizzp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gmsfbiicy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gciwkyrao.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.bbcook.cn/Article/details/gwljorbbt.sHtML


<!-- 参考信息 -->