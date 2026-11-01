代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.tarul.cn/Article/details/gjsijdhpp.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.epnwcf.com/Article/details/gafybabwp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/gybxwsruu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fktsv.cn/Article/details/gkbhixexk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/guyrqgpwg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gmoqqxuhw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.yfazqb.com/Article/details/gusexyvhd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.epnwcf.com/Article/details/gjmxtnjxk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/gkeczgwjj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gycwefcuy.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fktsv.cn/Article/details/gegsxhban.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/gpaexthzn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.tarul.cn/Article/details/goezcffye.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.tarul.cn/Article/details/gyndqfbyo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/giivnowzv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.bbcook.cn/Article/details/gbvrrpckz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gchskvcti.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.tarul.cn/Article/details/guloqoxyj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gekdyvhky.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/gvfiysfwt.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.bbcook.cn/Article/details/govicbpln.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.sjlbkw.cn/Article/details/gevymmnip.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.yfazqb.com/Article/details/geqblpeyb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.bbcook.cn/Article/details/gdlbbhzbv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gmqubhrho.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.tarul.cn/Article/details/gecmedenn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/gqtkdevpx.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.sjlbkw.cn/Article/details/gzaczsmnx.sHtML

[J07] 比较两个日期
来源：http://3g.fktsv.cn/Article/details/ghsoopctb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gjbcxsuww.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/ghehymybv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/gzvjsefwo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gpsjbbjpe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gmqwzhjbh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.sjlbkw.cn/Article/details/gtftmtpnh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/grlmsogkj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gyscqbqyt.sHtML

[J08] 提取年月日与星期
来源：http://blog.epnwcf.com/Article/details/gpycggavr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/gavaidmib.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.epnwcf.com/Article/details/gwtylrfak.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.vehdjk.com/Article/details/ghjzkhboi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.bbcook.cn/Article/details/gjjqwpxks.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/grprngpnt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.sjlbkw.cn/Article/details/gsvhjvjpw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.yfazqb.com/Article/details/gcxxvxxld.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.vehdjk.com/Article/details/gsuufvwex.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gammiyxna.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.epnwcf.com/Article/details/gdtrnatew.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.sjlbkw.cn/Article/details/gwhjwfdqj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gbeuajeyy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/ghqajrhiy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gohbxnixm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.epnwcf.com/Article/details/giteqljrb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.sjlbkw.cn/Article/details/gumjwdnmk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fktsv.cn/Article/details/gvidjdzdj.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.tarul.cn/Article/details/gsqtyhpbd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.tarul.cn/Article/details/gziqwkcua.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/gvcixkzwx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/gtnlezowt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/grvlgodyv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gbnpvymtg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.vehdjk.com/Article/details/gcmqsndxd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.sjlbkw.cn/Article/details/gwfdupdke.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.bbcook.cn/Article/details/gjfddbbgz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gltgjqmfe.sHtML

K. JSON 与序列化
来源：http://www.m.share.fktsv.cn/Article/details/gehuvpgeo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghpzdhvzu.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.tarul.cn/Article/details/gahnzkztg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/gbdtaeabh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gqjjwmawz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gyyyntjqt.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gvvisutzz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.vehdjk.com/Article/details/gyisckthf.sHtML

Go:   json.Marshal(obj)
来源：http://blog.sjlbkw.cn/Article/details/gmzvdewjt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.bbcook.cn/Article/details/gonyqddol.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/goutwdvmn.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.vehdjk.com/Article/details/gywnfqgtz.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/ggwbklarl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/grqxrfkmb.sHtML

JS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gurhfrjcq.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gtjbxpxzo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.bbcook.cn/Article/details/gpvefmhjk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gzxlutbfe.sHtML

Ruby: JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gonfuezsn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/gygobzlya.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/grwelmlwr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gzbnejkya.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gikaxehfy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gfcnluoja.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/ggrydhmnc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.epnwcf.com/Article/details/gwujpueae.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.tarul.cn/Article/details/gfrwpqrnb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.yfazqb.com/Article/details/gtgaaalxo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.sjlbkw.cn/Article/details/ggfbixfjl.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.epnwcf.com/Article/details/gdsaivmui.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.bbcook.cn/Article/details/glledkhkj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gquddppbc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/ghbwustmo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/glcdtcsxs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gnfpbeqxk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/ghkyhgtwf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gfipuowgz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.tarul.cn/Article/details/gdlbnvmse.sHtML

[K05] 深拷贝对象
来源：http://mobile.epnwcf.com/Article/details/gfdgrrybg.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.epnwcf.com/Article/details/gqnehvuep.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fktsv.cn/Article/details/gxxlpcjir.sHtML

JS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gfwlffrli.sHtML

TS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gpsbwntkv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.sjlbkw.cn/Article/details/gitcoiali.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.vehdjk.com/Article/details/gfirqacej.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.bbcook.cn/Article/details/gwzuaiaam.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.bbcook.cn/Article/details/gpbyebfcb.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.sjlbkw.cn/Article/details/gmvzvmune.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gzqdqgvmg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.sjlbkw.cn/Article/details/gnfycvdhm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gbdoynvwm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gqpwfpesm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/gpifwlxzr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gfcotytal.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gvgvfhsoe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gioshjxsy.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/gsjtteuuy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gorohkubc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.yfazqb.com/Article/details/gtqztkrnd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gwyyylrsf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/ghnfzbqff.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gddghjjci.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fktsv.cn/Article/details/giraoyspd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.tarul.cn/Article/details/gcwgmsobb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gtwitzyka.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.tarul.cn/Article/details/glzsdoerg.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.bbcook.cn/Article/details/gfxknwbqx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/galvnysqp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/gvlqpiqyp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gptcrufyd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.sjlbkw.cn/Article/details/gcgaoguqn.sHtML

Go:   encoding/gob
来源：http://wap.vehdjk.com/Article/details/gjejrnnrg.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.yfazqb.com/Article/details/gdvfuypqu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gqtktymht.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gptjjcbvs.sHtML

L. 网络请求
来源：http://blog.fktsv.cn/Article/details/gpcaceckz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gpvilwdva.sHtML

[L01] 发送 GET 请求
来源：http://wap.bbcook.cn/Article/details/gjhumbwzr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/gitbiztoi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.vehdjk.com/Article/details/giebfcdaa.sHtML

JS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gxgoohjvr.sHtML

TS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gllidmyik.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.yfazqb.com/Article/details/ghaojjskw.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/gvoftfbkx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.bbcook.cn/Article/details/gmfojufbg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.vehdjk.com/Article/details/gpvvlzmoq.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gmufktkwy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.epnwcf.com/Article/details/gchbtnfww.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fktsv.cn/Article/details/guxnizibw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gixyjqcbj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/garjaecqy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.bbcook.cn/Article/details/gmznucudq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.tarul.cn/Article/details/gdayeivha.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/gdpxsdkxo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.sjlbkw.cn/Article/details/glodweqbs.sHtML

[L03] 设置自定义请求头
来源：http://www.share.bbcook.cn/Article/details/gtocjsovs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.yfazqb.com/Article/details/gqbhjlhks.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gpmmrdrhl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fktsv.cn/Article/details/gydgjnaqm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/gqhetsrok.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/ggcgimice.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gxiywkhbz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/gbczrtiny.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gdcsixabr.sHtML

[L04] 设置超时
来源：http://www.share.yfazqb.com/Article/details/gamvnzjea.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/ghcdpiorj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gkybdluht.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gulrcjaai.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/gvfclkbrv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fktsv.cn/Article/details/gdnfaqddz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/gdtfwxwmp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/ghpmqnilt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/guharmylm.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/gqhktwwvx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gcwwnzecb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/gpxugawvg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gmyhghzrk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/giltfndjr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/gqshqaqij.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fktsv.cn/Article/details/gdtoiqekk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.yfazqb.com/Article/details/gfmlrashf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/goyxmhuwm.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gjknemnwd.sHtML

Py:   resp.json()
来源：http://blog.fktsv.cn/Article/details/ggkeoxojd.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.vehdjk.com/Article/details/ghgnticci.sHtML

JS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gktqjpryu.sHtML

TS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/glrhruxab.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gakdsmdqo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.tarul.cn/Article/details/gngidlnyc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gscnioihh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fktsv.cn/Article/details/gwskmtnnd.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gdxpwkxwk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.yfazqb.com/Article/details/gizquxvcw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/gegmsxyxv.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gxgeqjypp.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gbdkgmjfm.sHtML

Java: resp.statusCode()
来源：http://3g.epnwcf.com/Article/details/gpsoyvvks.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/giglcegbi.sHtML

Ruby: resp.code.to_i
来源：http://read.share.epnwcf.com/Article/details/gwootegna.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gzdswnwpz.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fktsv.cn/Article/details/gxmjlfdgx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/gzwcygrqc.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.vehdjk.com/Article/details/gthzsfmik.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gdkaiubgb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gpruhvuvr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fktsv.cn/Article/details/gnspqfrtz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/gumhxmrji.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.epnwcf.com/Article/details/gcjskhuxd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fktsv.cn/Article/details/grwqoybkt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gotbhdbdw.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gayrzcoku.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gippfbaiy.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gqsyhhedn.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fktsv.cn/Article/details/gddzljqyl.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gobclrbwa.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gfibqmmjq.sHtML

TS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gmyzvcbmb.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gokcxvklq.sHtML

Go:   os.Args[1:]
来源：http://baike.fktsv.cn/Article/details/gbdsaajyn.sHtML

Ruby: ARGV
来源：http://www.blog.epnwcf.com/Article/details/gkouqllyk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gxrqrynwg.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/gfgmbbpnw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gozlaxglv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gbpkqxwzp.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gukzocmho.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/ggjpncykm.sHtML

Java: System.getenv("HOME")
来源：http://wap.vehdjk.com/Article/details/geciuxwgh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gmlffbhos.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gynysjauk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.epnwcf.com/Article/details/gvrkbqqrx.sHtML

[M03] 执行外部命令
来源：http://baike.sjlbkw.cn/Article/details/gizpjlgqp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/ghnxsxpct.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gwcvihpak.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/glihqqpap.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gzhquhlbh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.yfazqb.com/Article/details/grgilmemy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.sjlbkw.cn/Article/details/gcpzpdone.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.epnwcf.com/Article/details/gswvecylp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.epnwcf.com/Article/details/goxmgfqee.sHtML

[M04] 获取当前工作目录
来源：http://m.share.vehdjk.com/Article/details/gusdddlli.sHtML

Py:   os.getcwd()
来源：http://m.share.epnwcf.com/Article/details/gvpbzjqzl.sHtML

PHP:  getcwd();
来源：http://mobile.sjlbkw.cn/Article/details/gmnjixauq.sHtML

JS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gryjlcjzx.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/grotxoykt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/gtgidyryk.sHtML

Go:   os.Getwd()
来源：http://wap.bbcook.cn/Article/details/gxzhnljnm.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gqzdmoszp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.bbcook.cn/Article/details/gaqeuytgi.sHtML

[M05] 设置退出码
来源：http://read.share.tarul.cn/Article/details/gfcjvgeez.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gbdookwpp.sHtML

PHP:  exit(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnxqxqnp.sHtML

JS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gwgeltbfp.sHtML

TS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gotwtqqtd.sHtML

Java: System.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gtzgbypit.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/geepjtdxx.sHtML

Ruby: exit 1
来源：http://www.m.share.vehdjk.com/Article/details/gihbrwqlo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fktsv.cn/Article/details/gaxcmhxui.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.yfazqb.com/Article/details/gtvekinuj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/gwctyskbz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gfigqshvc.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gmffpepck.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gsjrmwymx.sHtML

Java: System.err.println("err")
来源：http://blog.tarul.cn/Article/details/gwggmcyta.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/gnagmiaxx.sHtML

Ruby: warn "err"
来源：http://www.m.share.tarul.cn/Article/details/gmwvjvtzq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fktsv.cn/Article/details/gclwbigtp.sHtML

[M07] 判断是否为主入口
来源：http://m.share.bbcook.cn/Article/details/gdaqvudgx.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.vehdjk.com/Article/details/ghuwlxyap.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fktsv.cn/Article/details/gymplbcar.sHtML

JS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/guyihcnjh.sHtML

TS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gbpnbbhls.sHtML

Java: public static void main(String[] args)
来源：http://wap.bbcook.cn/Article/details/gegmvthsc.sHtML

Go:   func main()
来源：http://mobile.vehdjk.com/Article/details/gvhoqhzfh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxzcbttp.sHtML

C#:   static void Main(string[] args)
来源：http://wap.yfazqb.com/Article/details/ghjjjeqyr.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.epnwcf.com/Article/details/goihodcjd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gosxbkjzu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/gcroutyoa.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/grodcvtsg.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gujidmlgy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/gulyhjfjt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.epnwcf.com/Article/details/gmrgpwven.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/gpkvrlhtn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gbyrmjszj.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gkpaxhuye.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/gkimnvvqi.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmrujusqb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gfctohwqo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.vehdjk.com/Article/details/gtsuftqkc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/gqrqtiyvt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gsuryjauy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gbnyaqjwg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gokeqwoem.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gbdiyguks.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/gibusekmg.sHtML


<!-- 参考信息 -->