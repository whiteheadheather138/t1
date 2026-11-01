代发 wailian999

TS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/glzsbjmty.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gmtdrqjkj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gupmsbqqk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gcnxgavie.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.epnwcf.com/Article/details/gosuropwl.sHtML

[J04] 时间戳与日期互转
来源：http://baike.bbcook.cn/Article/details/ghefgjujx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.bbcook.cn/Article/details/gzqilvwio.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.epnwcf.com/Article/details/gohfwegtq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.tarul.cn/Article/details/gtbdyfdha.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.tarul.cn/Article/details/gnpufilxd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.epnwcf.com/Article/details/gjchyvlre.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.vehdjk.com/Article/details/gdzvsqyxz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.vehdjk.com/Article/details/gohjshpfs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.tarul.cn/Article/details/gqrxfokea.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.sjlbkw.cn/Article/details/gdjwbtcgs.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.bbcook.cn/Article/details/gkxfdgayb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.sjlbkw.cn/Article/details/gzbtsdfyi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/geuaejudq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/gdzapkcyy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.tarul.cn/Article/details/gjxvutaue.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.vehdjk.com/Article/details/gvxqvjmrk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.bbcook.cn/Article/details/ghvuqywoy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.yfazqb.com/Article/details/gjwcfirir.sHtML

[J06] 计算两时间之差
来源：http://3g.tarul.cn/Article/details/gkeopdmso.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.vehdjk.com/Article/details/gyclpuiue.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgrrqozv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.tarul.cn/Article/details/gforxeebz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.epnwcf.com/Article/details/gaohpggox.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/geejnfumm.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gauwnerww.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.bbcook.cn/Article/details/gwldtzvod.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fktsv.cn/Article/details/gmmcooksw.sHtML

[J07] 比较两个日期
来源：http://3g.vehdjk.com/Article/details/gdnncaaon.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gjclixqzy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.tarul.cn/Article/details/gwhfbwsqe.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gpjgeopup.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gqfymxinm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.epnwcf.com/Article/details/gzreepsld.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.epnwcf.com/Article/details/grdoeykmh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gelqbhrjf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gqqvjvxxq.sHtML

[J08] 提取年月日与星期
来源：http://mobile.yfazqb.com/Article/details/gdzmrdrie.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/galwfqlhz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.sjlbkw.cn/Article/details/gnctupeoz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.yfazqb.com/Article/details/gobheoznm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.yfazqb.com/Article/details/gejxrnrgb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/gmuuaortm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.tarul.cn/Article/details/gjbznjspw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.vehdjk.com/Article/details/gnzownbkd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/gpwmheyfw.sHtML

[J09] 时区处理
来源：http://www.m.share.fktsv.cn/Article/details/gigcmmeoo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.tarul.cn/Article/details/gzrtvrdsd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/gnqiyscdv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gfaslemsg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gzlbuqvcb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.yfazqb.com/Article/details/guwyqbmul.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.epnwcf.com/Article/details/gcvtjpxdr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fktsv.cn/Article/details/gwzzcbvuw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.vehdjk.com/Article/details/ghnejbntq.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.bbcook.cn/Article/details/gqitrxlgb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.tarul.cn/Article/details/gfmmnlrna.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.yfazqb.com/Article/details/ghyyrunbd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.yfazqb.com/Article/details/gqzecgncb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/gfqhlghhh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/gxrzzjtts.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.tarul.cn/Article/details/gwtansxvi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/gfealkomp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/gwnhdjosd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvbodpkmr.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/ggkncbzlg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gljjnutnm.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.yfazqb.com/Article/details/gxsryiipf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/glpzutteu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/gdygsxdds.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gvgfqjvqh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gcucfyjrl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/gctruhclb.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/gfniifnud.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.bbcook.cn/Article/details/gmprkjybc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.sjlbkw.cn/Article/details/ghjdfiqqb.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gwggjvthi.sHtML

Py:   json.loads(s)
来源：http://mobile.yfazqb.com/Article/details/gwzkwjmzb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/gzzvxttcs.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gdsfcottm.sHtML

TS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gramrqmng.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gbkmrtgct.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gvnuoqlyb.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gptjjgfcj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.vehdjk.com/Article/details/gcimrgygq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.tarul.cn/Article/details/gsvxftqed.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gsfelokwh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gmurcjmfd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gkmiwawcz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gsckgddce.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/gymthmcni.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fktsv.cn/Article/details/gtmnugxsg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.tarul.cn/Article/details/gcrycwlwf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.yfazqb.com/Article/details/gitckngps.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/gynakzkva.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.epnwcf.com/Article/details/guoojlnuk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.bbcook.cn/Article/details/ggxzrkxdk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/glcefpwjp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gnqqekcyj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gqhdqpezu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gzbmlpxxg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.yfazqb.com/Article/details/gegqjfuqy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gzejfhmip.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gxbwxqqpp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.epnwcf.com/Article/details/gnqrogfjz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/guglemhuq.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/ggpdmzski.sHtML

TS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gxxivrkgc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/gbmljbpoe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.yfazqb.com/Article/details/grvtwvguy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gkxjrpduk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/gfcwbydfo.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/gcqcipvpn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.bbcook.cn/Article/details/ghaghjmcr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.yfazqb.com/Article/details/gwghplyra.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gwixwkbwp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/godtpfeex.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.vehdjk.com/Article/details/grdevucgo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gvhzcicsf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gczjhtgsq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gnzjfkior.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/ggwxowhyh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gfsqrghwy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.epnwcf.com/Article/details/gidbxuyxq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gqwzllhzi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gpqncqdwy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gxfexaste.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.bbcook.cn/Article/details/geihorbkz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gxascurtf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gmhabales.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/gzjodlpyp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/gdulsukzz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.tarul.cn/Article/details/gcnrpmsye.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/ggucrifiw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/gggmtradg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.sjlbkw.cn/Article/details/gcnepbzjr.sHtML

Go:   encoding/gob
来源：http://mobile.sjlbkw.cn/Article/details/gsdboyseh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/gxbmsgybt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gphsljhpf.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwzbocvtr.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/gruxsitwr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gutmuklkw.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/gwrmuamdv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.bbcook.cn/Article/details/gvczvpkzs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.epnwcf.com/Article/details/gmxotpmts.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gxogkjtky.sHtML

TS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gmghqokbp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/glkeptxwb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/grlgtwklj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.yfazqb.com/Article/details/gwykmxzpm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/gcqonvhia.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/glybsolxy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/ggxevrylt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gdqjlnmbx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/grmlussyz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gwnianjgy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gptipxape.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.vehdjk.com/Article/details/gljvyigyt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fktsv.cn/Article/details/gjjaipwqg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.tarul.cn/Article/details/gdsgzjddn.sHtML

[L03] 设置自定义请求头
来源：http://read.share.vehdjk.com/Article/details/giluofgmb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.vehdjk.com/Article/details/gqcwvdwpt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.sjlbkw.cn/Article/details/ggmhzwpcg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/ghowughgc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gqvvylisx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/ggawbwjuv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.bbcook.cn/Article/details/gnksswpfz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/gvllzpvzn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gwvbfrpli.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/gkjmoobkq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.tarul.cn/Article/details/gxlaevfep.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.tarul.cn/Article/details/gxuoukcyq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gvorifzvn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gknucsxdp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.yfazqb.com/Article/details/gdfsvxplb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gohzkroxh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gahjedkdz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.epnwcf.com/Article/details/gkxwohuhz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.epnwcf.com/Article/details/gizstyyud.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.sjlbkw.cn/Article/details/gtwrwcszp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/ghqsqlekb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.tarul.cn/Article/details/guhxoullk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gswmtxytv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fktsv.cn/Article/details/gwarojxos.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fktsv.cn/Article/details/gyjasdsui.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gspzffaka.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.yfazqb.com/Article/details/gqonkftgt.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fktsv.cn/Article/details/gxxdsbkrr.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/goobbixwd.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fktsv.cn/Article/details/gopnxefuk.sHtML

JS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gbgiidxzg.sHtML

TS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gnitvuxrl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.bbcook.cn/Article/details/glcsrphsr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gafmbkven.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.tarul.cn/Article/details/gldptnwgw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/gbjrnjogf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gcmcyfyqf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/gaipxbudk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/gixjkixxa.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gjvczbxnt.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gtugbpxfn.sHtML

Java: resp.statusCode()
来源：http://www.blog.tarul.cn/Article/details/gngtfncao.sHtML

Go:   resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gysjbtikm.sHtML

Ruby: resp.code.to_i
来源：http://mobile.tarul.cn/Article/details/gtoxbhzhu.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gxatnlwdr.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/gjbqssrun.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/gxvkyvtht.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.epnwcf.com/Article/details/gwiuqhzss.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gjsyfojln.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gxfzbkxzq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fktsv.cn/Article/details/gjflvsasm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/gmkojzsyr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/govjxoyyu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.yfazqb.com/Article/details/geaybyrzv.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glwbphzsw.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/gdgvcceaw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdcpzzyct.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gvwmohsnx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.tarul.cn/Article/details/glsyjoevp.sHtML

PHP:  $argv;  $argc;
来源：http://baike.yfazqb.com/Article/details/ggaaevpoi.sHtML

JS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/gkwmnkyea.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gutxnuszo.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.tarul.cn/Article/details/grubjvjyv.sHtML

Go:   os.Args[1:]
来源：http://3g.fktsv.cn/Article/details/gearkxfeq.sHtML

Ruby: ARGV
来源：http://m.share.tarul.cn/Article/details/galuxwlqt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gwnvocwkd.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gdatcydgc.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/gegnrjwvq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gatzltosn.sHtML

JS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gszvvarib.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/giwycnwsk.sHtML

Java: System.getenv("HOME")
来源：http://wap.yfazqb.com/Article/details/grimvxzfm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gfykfrfab.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/gztetozhj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gabshebhq.sHtML

[M03] 执行外部命令
来源：http://3g.sjlbkw.cn/Article/details/gtojwyyxu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.tarul.cn/Article/details/gvdqqeugu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/gmurkqvvy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gzphnuvyk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gsxyhomyu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.bbcook.cn/Article/details/giywocklz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/guxjqstkn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.bbcook.cn/Article/details/gxpdjhstz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gmnpoloex.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fktsv.cn/Article/details/gsmsszlrg.sHtML

Py:   os.getcwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfeglgyqr.sHtML

PHP:  getcwd();
来源：http://wap.vehdjk.com/Article/details/gtwjuhxqt.sHtML

JS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/grdwbhddg.sHtML

TS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/guofbnfzg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.epnwcf.com/Article/details/goemzikud.sHtML

Go:   os.Getwd()
来源：http://www.share.yfazqb.com/Article/details/gublwtkir.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/guttknono.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/gcsjxurdc.sHtML

[M05] 设置退出码
来源：http://www.m.share.vehdjk.com/Article/details/gtbpqyazq.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gaousijqw.sHtML

PHP:  exit(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsruwbdh.sHtML

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gvzskqluu.sHtML

TS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gyjqzmlgu.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gnnnukloc.sHtML

Go:   os.Exit(1)
来源：http://m.share.tarul.cn/Article/details/gqhhfwdrq.sHtML

Ruby: exit 1
来源：http://blog.sjlbkw.cn/Article/details/gmagthvbb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.yfazqb.com/Article/details/gximkavuc.sHtML

[M06] 向标准错误输出
来源：http://www.blog.tarul.cn/Article/details/gyehxbbeq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gfcelijag.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/ghwoxsytb.sHtML

JS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gbnnbmtib.sHtML

TS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/genonkgli.sHtML

Java: System.err.println("err")
来源：http://blog.sjlbkw.cn/Article/details/gpujwwadj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/grgvwsffc.sHtML

Ruby: warn "err"
来源：http://www.blog.yfazqb.com/Article/details/gbkyimwyd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.tarul.cn/Article/details/goggohtgn.sHtML

[M07] 判断是否为主入口
来源：http://mobile.epnwcf.com/Article/details/gkmnlhzfw.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.bbcook.cn/Article/details/gmnwpgdym.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/gmjysacav.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gwonmmzxp.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gkksregai.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/gznxkkgjh.sHtML

Go:   func main()
来源：http://www.share.vehdjk.com/Article/details/gcwwzmmok.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.vehdjk.com/Article/details/gsinbsdaq.sHtML

C#:   static void Main(string[] args)
来源：http://3g.tarul.cn/Article/details/gvbtgzgqz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.vehdjk.com/Article/details/ganymcxvk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gfokhjlqy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.yfazqb.com/Article/details/ggpdtlvjp.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gdwlpjyep.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gdagdcxfl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.vehdjk.com/Article/details/gacxxxxyi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/gajbbzcpk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.bbcook.cn/Article/details/gmkhfribd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fktsv.cn/Article/details/gkpblehak.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gaqymbhfk.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gzattoouc.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gakvqoztd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.epnwcf.com/Article/details/gpqndoqlk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gnzfbrgbu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gvenjezsp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gzszuhtwm.sHtML


<!-- 参考信息 -->