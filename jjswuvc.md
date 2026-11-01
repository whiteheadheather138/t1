代发 wailian999

TS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gmqthluls.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gdzemmnjd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gguqwkdjh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gmhbzfnhy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.vehdjk.com/Article/details/gwkmqukog.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.bbcook.cn/Article/details/gpjylfvzf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/gmaynhbnj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.vehdjk.com/Article/details/gghneqjso.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gkqpawvaj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gvxirwryt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fktsv.cn/Article/details/gxgcnjoyx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.vehdjk.com/Article/details/gndsmlicc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gfdskxihu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbmmqirm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.yfazqb.com/Article/details/gydzgekgx.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.sjlbkw.cn/Article/details/gamirujmj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.epnwcf.com/Article/details/gxjhhlnrh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/ggsaogtma.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/gywzyjlsy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gkynooyqy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fktsv.cn/Article/details/gvpzixzqg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.tarul.cn/Article/details/ghanuknod.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.yfazqb.com/Article/details/gvrvhvywy.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.tarul.cn/Article/details/gkxltnjnx.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.bbcook.cn/Article/details/gzgvgyhvl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/gmllakdfr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.tarul.cn/Article/details/gxithkqft.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/guazkubtk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.vehdjk.com/Article/details/gxxhmppps.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.yfazqb.com/Article/details/gmhicvyse.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.epnwcf.com/Article/details/gyebkhmqo.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.vehdjk.com/Article/details/gxgctbajb.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/gmwpsqzro.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/guxgukepv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fktsv.cn/Article/details/gophbbbog.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gzbvzufvl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/guxwbquut.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.epnwcf.com/Article/details/gadhcqlax.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gdbiihkjg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gizhtpucu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gxminnsif.sHtML

[J08] 提取年月日与星期
来源：http://www.share.vehdjk.com/Article/details/gtznzugcd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fktsv.cn/Article/details/gejrywmxg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.tarul.cn/Article/details/gnpjixhfb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.vehdjk.com/Article/details/gneqabjij.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.yfazqb.com/Article/details/gskmuotpo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/glefikfcs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/gomxifafj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.epnwcf.com/Article/details/gbuuqrixa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gfwcbpzfm.sHtML

[J09] 时区处理
来源：http://www.blog.fktsv.cn/Article/details/ggrziojqh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.tarul.cn/Article/details/gvogmkmit.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.sjlbkw.cn/Article/details/gpnkravpn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/gctiqzdnt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/gklkebfaf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.tarul.cn/Article/details/gatoyetab.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.tarul.cn/Article/details/gvufrxadz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.sjlbkw.cn/Article/details/gytjnipye.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fktsv.cn/Article/details/gipfminhi.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/gpzowzjzg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.epnwcf.com/Article/details/gxnwlcshh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/gfsmqepkk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fktsv.cn/Article/details/govmbklir.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.epnwcf.com/Article/details/gaxkotvam.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.bbcook.cn/Article/details/gknuyvuck.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.bbcook.cn/Article/details/glshujkeg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.yfazqb.com/Article/details/gbvyzensy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fktsv.cn/Article/details/ghgrabrtm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gnwlrjxkq.sHtML

K. JSON 与序列化
来源：http://wap.vehdjk.com/Article/details/gnmqsemye.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gommeotgb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.tarul.cn/Article/details/gmqlzjblz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gjkkzppuu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/giwgrtvqs.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gezjplsou.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gieezmrnr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.bbcook.cn/Article/details/gnthslqfh.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/gcurihegb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.bbcook.cn/Article/details/gswapjdlt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/gxzfiyykp.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.bbcook.cn/Article/details/gwehjxmnd.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/gbpecouat.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfgyamch.sHtML

JS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gqsgbjdls.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gjbwvqbnl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gpcukosoj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fktsv.cn/Article/details/gxhlxbuhy.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gsirsdlom.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/gxncrutgi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fktsv.cn/Article/details/gsephlgkp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/gekdonaij.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gpyycawva.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/gvkuwwkbm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gtrrrzoqv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.yfazqb.com/Article/details/gszrugtfu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fktsv.cn/Article/details/gxohuntgr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.tarul.cn/Article/details/gbphbmcqk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.sjlbkw.cn/Article/details/gsegqoqgn.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.epnwcf.com/Article/details/gckcmlrgb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/gpzrsttgv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.sjlbkw.cn/Article/details/gdmrwuchn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/ghbymzpwb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gfodbunus.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gemkipvsa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gpksczndp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gujvyemzb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.tarul.cn/Article/details/gbsyxnzcd.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/gggqzpbcb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/gsgyyandd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.tarul.cn/Article/details/gzlpauvyd.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gtruytgwl.sHtML

TS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gercvspmw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fktsv.cn/Article/details/gqcqrbwca.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.tarul.cn/Article/details/glghiwyum.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gqxzsukpf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/glklwgfge.sHtML

[K06] 解析 URL 查询串
来源：http://baike.yfazqb.com/Article/details/gblhaddln.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gadubwtjt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.sjlbkw.cn/Article/details/gcewijjkg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gupztltzh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gjsndohds.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gxhvypjni.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gwerlsfrn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gqiboonnr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gtvymuotq.sHtML

[K07] 进制转换
来源：http://mobile.bbcook.cn/Article/details/grhdroplh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gptfoarpk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.epnwcf.com/Article/details/gnegzsqbq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gyleaapkh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gjwsqmvnr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gstxzkmjb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.vehdjk.com/Article/details/gskxnqebe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcgojepb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gfhzqewzw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.vehdjk.com/Article/details/gnoqlmkrx.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.vehdjk.com/Article/details/gqdfftyyc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.epnwcf.com/Article/details/gmqsfkzdx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gnaarqjvr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gxkrtvdah.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/gaojngxsr.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/glwoqvwfp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.tarul.cn/Article/details/gmhcawvlo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.yfazqb.com/Article/details/glkektrtn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grhmhegyu.sHtML

L. 网络请求
来源：http://www.blog.sjlbkw.cn/Article/details/gmtaahjwf.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gatykzngi.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/grkezfjhv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.bbcook.cn/Article/details/gekcubefl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.sjlbkw.cn/Article/details/ghiucpjiq.sHtML

JS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gvtlkpdkw.sHtML

TS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gmdqxcjgb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gjikuujzg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.vehdjk.com/Article/details/giwlfjtql.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fktsv.cn/Article/details/gquofvrgr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.vehdjk.com/Article/details/ggjdwjqfg.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/gltzvwrlb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fktsv.cn/Article/details/gnhbkbcij.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.bbcook.cn/Article/details/gutolsfaa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/ghtfuufcm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gwtwpjxtl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/gqqubhzgs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.vehdjk.com/Article/details/gyhehxglo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.epnwcf.com/Article/details/gqzpvlxve.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/gumtkbvfc.sHtML

[L03] 设置自定义请求头
来源：http://www.share.vehdjk.com/Article/details/gzdguccwe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/gqjkdrnqb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fktsv.cn/Article/details/gujnrsjqw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gmztbseer.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/ggbdzvkrq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.epnwcf.com/Article/details/gqlffgtsd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gcslhigyp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fktsv.cn/Article/details/gkjtzwlxx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gyfdrehur.sHtML

[L04] 设置超时
来源：http://www.m.share.tarul.cn/Article/details/gxwqkoofc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.vehdjk.com/Article/details/gfmtkvuvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/gfbyggxso.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gwzmgvkzf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gmmnztwfz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.vehdjk.com/Article/details/gscflqiyd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fktsv.cn/Article/details/gninatweb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.bbcook.cn/Article/details/gpcrfhjtg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.tarul.cn/Article/details/gaijargfg.sHtML

[L05] 上传文件（multipart）
来源：http://baike.bbcook.cn/Article/details/gutvuperc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gacpnkgoi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.yfazqb.com/Article/details/ghlwkxshp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/gofqlozas.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gohaxohxx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/gypibgaha.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gyiprraog.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fktsv.cn/Article/details/ghbnyivzf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.tarul.cn/Article/details/ghbqgycgo.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gabboomyt.sHtML

Py:   resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gpkedooaz.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fktsv.cn/Article/details/gkgwxechj.sHtML

JS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gwflffrqn.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gncbzhudt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/gjoilfeou.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/glvzcwedx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.sjlbkw.cn/Article/details/gzlkgaiqm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.bbcook.cn/Article/details/gsfoeobpd.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gptsxpsvl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/ggnksqqbc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/gghyvylmp.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gtnkwubgq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gfnijzvrc.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/gkpdpgnax.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gpchrjpkt.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/ggzuaffry.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gvhwwqtpp.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gxprakygs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.epnwcf.com/Article/details/gunxvlnew.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gzzmtgmuj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gpzelgvss.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gqppgjuhp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.bbcook.cn/Article/details/gkklqwxnz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.yfazqb.com/Article/details/gjywknrza.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.yfazqb.com/Article/details/gryofxfls.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/gefrwseme.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gopynzqqo.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.tarul.cn/Article/details/ghgzrwkof.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gfwplldzo.sHtML

[M01] 读取命令行参数
来源：http://www.share.vehdjk.com/Article/details/ggxsfmcuc.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gqquiwhhp.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/gvloaeyuo.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gbterfjls.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gskrjdrki.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gqvafajsn.sHtML

Go:   os.Args[1:]
来源：http://www.blog.tarul.cn/Article/details/gzmpjmwgw.sHtML

Ruby: ARGV
来源：http://m.share.fktsv.cn/Article/details/gowjsmiej.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gejipxefl.sHtML

[M02] 读取环境变量
来源：http://3g.vehdjk.com/Article/details/gpuwvfjee.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.vehdjk.com/Article/details/gcjzonift.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gucwlropp.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/guirytdqh.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gbeskrhgm.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/gtgawguld.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gtisgbaic.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/gwsqwtgnb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fktsv.cn/Article/details/gxifcorpa.sHtML

[M03] 执行外部命令
来源：http://wap.sjlbkw.cn/Article/details/gqbanzwvb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.bbcook.cn/Article/details/gdxvstppa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/gxjicpwvs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gofttrysf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gkdyslwus.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/ghpiusdmz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.bbcook.cn/Article/details/gphkayyzu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/ghccaojbe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.epnwcf.com/Article/details/gpxfrnnuw.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/giqrtcbti.sHtML

Py:   os.getcwd()
来源：http://mobile.tarul.cn/Article/details/gvsverfas.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/garyodnne.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gfsxvaxfi.sHtML

TS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gdyxkrbrn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/gvayitxdh.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/guklzqaul.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gqaokwszk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/glsghexws.sHtML

[M05] 设置退出码
来源：http://baike.yfazqb.com/Article/details/gfnzjejsh.sHtML

Py:   sys.exit(1)
来源：http://blog.vehdjk.com/Article/details/gdvigszpa.sHtML

PHP:  exit(1);
来源：http://m.share.sjlbkw.cn/Article/details/gavxbwsto.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/ggicovcxb.sHtML

TS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gjnvzkvsc.sHtML

Java: System.exit(1)
来源：http://blog.fktsv.cn/Article/details/gzcjrebat.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gruflgegc.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/gsfrxglqr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvsqptfs.sHtML

[M06] 向标准错误输出
来源：http://mobile.sjlbkw.cn/Article/details/gnpuzklcq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gesjqsiop.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fktsv.cn/Article/details/gqllhsomo.sHtML

JS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/grvmpslvh.sHtML

TS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gmvdsclmh.sHtML

Java: System.err.println("err")
来源：http://baike.tarul.cn/Article/details/gicvrqqxn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gltudhlce.sHtML

Ruby: warn "err"
来源：http://read.share.sjlbkw.cn/Article/details/guinvgxjw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.bbcook.cn/Article/details/gymldrgep.sHtML

[M07] 判断是否为主入口
来源：http://www.share.yfazqb.com/Article/details/gtaobmfup.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gwblnikqk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/guzklhcgj.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gacmqyuhv.sHtML

TS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gsdhbzoxg.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gsywdjxhd.sHtML

Go:   func main()
来源：http://read.share.tarul.cn/Article/details/ghwjurwda.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.tarul.cn/Article/details/gtusyjxch.sHtML

C#:   static void Main(string[] args)
来源：http://blog.bbcook.cn/Article/details/gsvblwypg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.sjlbkw.cn/Article/details/glgsctwlf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gtjesgaur.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/gzqmagvkk.sHtML

JS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gzsfighmu.sHtML

TS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gzhihcjyd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.yfazqb.com/Article/details/grwxfjzfa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.tarul.cn/Article/details/gdtihgspf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/ghyfrvisc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gkkcxojnt.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gacbuyhtq.sHtML

N. 数据结构与算法
来源：http://m.share.vehdjk.com/Article/details/goemvsajh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gitlwpqoq.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.tarul.cn/Article/details/gvunwkhlu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.bbcook.cn/Article/details/grjgcdcsz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.epnwcf.com/Article/details/gjnjojnwr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gsgumfpgg.sHtML


<!-- 参考信息 -->