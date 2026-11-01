代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.bbcook.cn/Article/details/gyxjysvjz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.sjlbkw.cn/Article/details/gxyupajje.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/gaurznsvm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.epnwcf.com/Article/details/gxthifrge.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.sjlbkw.cn/Article/details/guawfzrvy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fktsv.cn/Article/details/goslfdkpg.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.tarul.cn/Article/details/gvdmstfax.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.bbcook.cn/Article/details/gdfvnnkkl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.bbcook.cn/Article/details/gvwujwnjn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gqhnsknab.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/gojqmrctp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.epnwcf.com/Article/details/ggipkvrvv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fktsv.cn/Article/details/ghsnatqir.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.sjlbkw.cn/Article/details/girudxnkl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fktsv.cn/Article/details/ggiyhzlfu.sHtML

[J06] 计算两时间之差
来源：http://blog.fktsv.cn/Article/details/gicwtsjhb.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/gamcfokdk.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.bbcook.cn/Article/details/gzaitliyg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.sjlbkw.cn/Article/details/gvhiauukv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.bbcook.cn/Article/details/givnzkfqw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.bbcook.cn/Article/details/gwekpdxhl.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.epnwcf.com/Article/details/gtvqvkdec.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.tarul.cn/Article/details/gknpyjwjb.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.yfazqb.com/Article/details/gfotzczab.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/gktpogziz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gnwzfzigd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fktsv.cn/Article/details/gwvwxptir.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gxxarehbv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/ggwctqcnj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.vehdjk.com/Article/details/gfpccfpth.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.vehdjk.com/Article/details/gzmxioqqv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gysgthetk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gyvbgfjem.sHtML

[J08] 提取年月日与星期
来源：http://blog.sjlbkw.cn/Article/details/gbhsmrifm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fktsv.cn/Article/details/gstqtufgx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.vehdjk.com/Article/details/grzzakhut.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fktsv.cn/Article/details/gqsdrtwug.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/gjvxnnvbw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.sjlbkw.cn/Article/details/gkayeigma.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gecnbpcfm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.bbcook.cn/Article/details/gobwitcdk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/ghbxeholx.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/gbtjvhzzd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gminpgdod.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gmevgytrw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/gfogjrbex.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gyxjskicm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.bbcook.cn/Article/details/gyvkfftmk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuhiewxu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.epnwcf.com/Article/details/gizhghqms.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.sjlbkw.cn/Article/details/ginqxemyx.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.sjlbkw.cn/Article/details/ggujagqqg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.vehdjk.com/Article/details/gzygjyybi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.yfazqb.com/Article/details/gdxaizrad.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.tarul.cn/Article/details/gpkjegovt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gbmnxblli.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.tarul.cn/Article/details/gimexjnwc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.sjlbkw.cn/Article/details/ghirxzydx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.yfazqb.com/Article/details/gnibnqhya.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.vehdjk.com/Article/details/gaefqrncx.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjczfsieu.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/gdmtunipn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gigeebiva.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.tarul.cn/Article/details/ggtfobifc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gywwhotue.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/gnvlunnhy.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gchlwpeun.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/gixsfbrut.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/gcgjyivjh.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fktsv.cn/Article/details/gvhwwfcwh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fktsv.cn/Article/details/gdeospbsq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/guegavipt.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.bbcook.cn/Article/details/gtpbirdbu.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/gcmbfoxdi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.bbcook.cn/Article/details/gadeazzfn.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gnjzqiqjh.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gurfpjmai.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/ghuxfsqel.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gbvwdnbbz.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdchjbxu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.bbcook.cn/Article/details/gjefveolc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.epnwcf.com/Article/details/gqyweeyvz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gbgtikrzl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gqfsdzcgz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gfnyzztst.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/ggfhhjxbc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gubjbvtpk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.tarul.cn/Article/details/gylmajfki.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.bbcook.cn/Article/details/gwbttkruc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fktsv.cn/Article/details/gejwdpvao.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gmvxnssjn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fktsv.cn/Article/details/gpyaqidah.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gzzcpzwvs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/giutsinyv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/guxaeeiex.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gxkzxlqwx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/goixrrccm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gvuizpqer.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gxeatygfz.sHtML

[K05] 深拷贝对象
来源：http://3g.sjlbkw.cn/Article/details/gtrhltiii.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.bbcook.cn/Article/details/gmwcjmnjc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/getxksztp.sHtML

JS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gvtydyumz.sHtML

TS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gcttsmqab.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.yfazqb.com/Article/details/gtlbzcide.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/gtnipxyai.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.bbcook.cn/Article/details/grkslzsgf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.tarul.cn/Article/details/gdutwkkww.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.tarul.cn/Article/details/gqdurslhu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/geneiumrt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.tarul.cn/Article/details/gsuvgzjcm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gpetgbjcx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gjqrijyum.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gtikjsngr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gineoteev.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gtputapyh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gebymjvdk.sHtML

[K07] 进制转换
来源：http://m.share.fktsv.cn/Article/details/gusjfbqgx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gdxcrklva.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/gucoyknwy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gieniqnje.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gigmusobg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gpfxvhsmf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.epnwcf.com/Article/details/gaaqyqvyt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gcvxavacb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gndnutxhu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.tarul.cn/Article/details/gwgcaljgd.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.tarul.cn/Article/details/gjhqywlxh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/gohvqzjda.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gcpztkvpw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gfhxumfou.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/gkfosswap.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/gjofdiwkg.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.tarul.cn/Article/details/glybiarmh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gmqcaurcc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxkeawjmh.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gkfbepuuh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gralnefme.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/gvmyadbtj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.epnwcf.com/Article/details/gdilkgcrp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbqblndd.sHtML

JS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gkwoiwvva.sHtML

TS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/gqucdvreu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.epnwcf.com/Article/details/gchyztmre.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.tarul.cn/Article/details/gulpihvsb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/gpwhwxmuj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/gyqgumsln.sHtML

[L02] 发送 POST JSON
来源：http://www.share.yfazqb.com/Article/details/geytxceef.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.bbcook.cn/Article/details/grqytsylc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.bbcook.cn/Article/details/gbrkomnrq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/guaehtjhz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gzhsfqjiz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.sjlbkw.cn/Article/details/gsolqjrkx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.sjlbkw.cn/Article/details/gotvahewe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.bbcook.cn/Article/details/ggxockxch.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/guoimnukg.sHtML

[L03] 设置自定义请求头
来源：http://baike.vehdjk.com/Article/details/gxmeomjgt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gxnhydclq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.vehdjk.com/Article/details/gtnqcbses.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/grqaedkzv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/ghooxwbag.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.vehdjk.com/Article/details/gekdcjayh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gmlqkpjcw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.sjlbkw.cn/Article/details/gmcdrqpfc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gudcczbpn.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/gspqoeotl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.yfazqb.com/Article/details/gjqhbxrnf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.bbcook.cn/Article/details/gbizxlqnt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/guhvvjtyk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gewhufcys.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.bbcook.cn/Article/details/gcqhdnnlx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/guuterlbm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fktsv.cn/Article/details/gcsmzimfg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.yfazqb.com/Article/details/gegoweiqa.sHtML

[L05] 上传文件（multipart）
来源：http://blog.bbcook.cn/Article/details/ggtrvyiqc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.vehdjk.com/Article/details/gjldjabjg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/gptitpkbv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/gppwwutib.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gsmszskwi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/ghkqwrbby.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.sjlbkw.cn/Article/details/gepwgycnh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.yfazqb.com/Article/details/ghrcltjze.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.tarul.cn/Article/details/gpzfhafqg.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gpvuaarmw.sHtML

Py:   resp.json()
来源：http://blog.vehdjk.com/Article/details/gapwbcrvf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.vehdjk.com/Article/details/gqxlaitrc.sHtML

JS:   await resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/glxqtozne.sHtML

TS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gadxzkwnf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/glkmlltis.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/ggmfyhnow.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/guwlseues.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/gnyeeyvpw.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/garsescyx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.bbcook.cn/Article/details/gvmcqhgye.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fktsv.cn/Article/details/gwqxubsbo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gamnhiomj.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/guqcmqbqn.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/geqhxuqlf.sHtML

Go:   resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gbvdqkriv.sHtML

Ruby: resp.code.to_i
来源：http://blog.tarul.cn/Article/details/gdzzjsykl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gleflflzy.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/gpplldabk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.sjlbkw.cn/Article/details/gavaycbuj.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.vehdjk.com/Article/details/grdtckahr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gstmpevvk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gjoqlglzi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/goudlaswo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/govcdysor.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gdxckhliw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gbqgmpvds.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxahjdker.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.epnwcf.com/Article/details/gkaimsxxn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/giigxnxnv.sHtML

[M01] 读取命令行参数
来源：http://mobile.epnwcf.com/Article/details/gsfeivhea.sHtML

Py:   sys.argv[1:]
来源：http://3g.sjlbkw.cn/Article/details/gcvgbsvav.sHtML

PHP:  $argv;  $argc;
来源：http://baike.tarul.cn/Article/details/gasuqzhro.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gisrgobha.sHtML

TS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/gglinwdxw.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gpfknprye.sHtML

Go:   os.Args[1:]
来源：http://www.share.bbcook.cn/Article/details/gupqgdjqs.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/gzyavmybr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gsvaehhdo.sHtML

[M02] 读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gtjnsldul.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/gcxpqkevc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/goppfeilm.sHtML

JS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gvhumrfbr.sHtML

TS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/glntxumid.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/gnzavvnpj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/glhyyjtmn.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/greunevtb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/ggopsozuv.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/glfkzxqzf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/guyfuveqm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gpsrnkiwb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/ganhdsgfi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gwmynksdr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.bbcook.cn/Article/details/gazaqudoj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gherawzey.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.bbcook.cn/Article/details/gbnqneezk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/gbcyrtotr.sHtML

[M04] 获取当前工作目录
来源：http://wap.tarul.cn/Article/details/gitzddlxd.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/ggosvhnac.sHtML

PHP:  getcwd();
来源：http://wap.vehdjk.com/Article/details/gllbpecty.sHtML

JS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/ggguozpnr.sHtML

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/grmumexpx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/gcsrtfjdg.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/gdvqhjkgs.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/gmpnfthoh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.tarul.cn/Article/details/gtunghoma.sHtML

[M05] 设置退出码
来源：http://read.share.fktsv.cn/Article/details/gjkvacutw.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/gpiugpifg.sHtML

PHP:  exit(1);
来源：http://mobile.sjlbkw.cn/Article/details/gykrcmkeb.sHtML

JS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gbrizxsvx.sHtML

TS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gctvyqipd.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gijigpztg.sHtML

Go:   os.Exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gazwzkrqv.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gefoqtnjp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.yfazqb.com/Article/details/grftogxjq.sHtML

[M06] 向标准错误输出
来源：http://mobile.vehdjk.com/Article/details/gnjmklptl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gldbtouhc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fktsv.cn/Article/details/gehyyfdkk.sHtML

JS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gabxkmwlo.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gfptdohhb.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gtyttsrtt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.yfazqb.com/Article/details/gqvqihxzz.sHtML

Ruby: warn "err"
来源：http://www.blog.bbcook.cn/Article/details/goxmcewvr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.vehdjk.com/Article/details/gihtqbrzp.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gbfakpruo.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fktsv.cn/Article/details/gsgbaqtvu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/gzphinsew.sHtML

JS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gtwtcbwty.sHtML

TS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gdphprqhb.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/grxnxwkgi.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/gqenrkqcd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/gydmpuzpp.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.yfazqb.com/Article/details/goyzyufnj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/glvrneysv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/gpprsmbjl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.vehdjk.com/Article/details/gfecltuei.sHtML

JS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/getzvxktm.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gygyrxwdg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/gesgkgjpc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gezfcsbrl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gfcsltznn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/gqzsakjow.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ggjumepcf.sHtML

N. 数据结构与算法
来源：http://mobile.yfazqb.com/Article/details/gslvrvtuf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqwbspkkl.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/gpfazugtx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gnizmqihr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/gfjevslmx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gieoojerj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gcgwsmatm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gbpvgepyl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/gtzklictf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/giurvvhjl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gfkljavdw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.vehdjk.com/Article/details/gssrnzrrw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gfhrqutbt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.tarul.cn/Article/details/gfscnztbl.sHtML


<!-- 参考信息 -->