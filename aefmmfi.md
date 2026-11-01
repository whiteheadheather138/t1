代发 wailian999

TS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gfnjqfkop.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/glsythmlg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/ggezrdpxk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gnonzlvxn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.sjlbkw.cn/Article/details/gqhvoguat.sHtML

[J04] 时间戳与日期互转
来源：http://baike.bbcook.cn/Article/details/gzxbemsrl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.vehdjk.com/Article/details/gbwjqtqvv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.epnwcf.com/Article/details/gxfpmlukl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.vehdjk.com/Article/details/gogmjkqjh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.epnwcf.com/Article/details/gchampjrh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.bbcook.cn/Article/details/gbuzatyru.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fktsv.cn/Article/details/gqhxhtlvv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fktsv.cn/Article/details/gdemeuhbf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.sjlbkw.cn/Article/details/gwtmnopmb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.tarul.cn/Article/details/gebhjnitv.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.yfazqb.com/Article/details/gpjhyifec.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gkhybjhqf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gmzdhaxdt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gaywspgbm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/ghsdkekon.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.epnwcf.com/Article/details/gtqlsalzr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/gfwygaiba.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/guhsiaryl.sHtML

[J06] 计算两时间之差
来源：http://mobile.sjlbkw.cn/Article/details/gjpsggrgo.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/gvrlhxygp.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.vehdjk.com/Article/details/gmtmjalck.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/ghbjwxkno.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.yfazqb.com/Article/details/gekjlakpp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.vehdjk.com/Article/details/gyxbogwhj.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.tarul.cn/Article/details/gfimpxtqn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.tarul.cn/Article/details/gbejlmdjd.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.sjlbkw.cn/Article/details/ghkmtsapz.sHtML

[J07] 比较两个日期
来源：http://3g.tarul.cn/Article/details/gettbkyjn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gdqzquget.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.yfazqb.com/Article/details/gowbfnwsd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gzrexweah.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gfkvxsokr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.vehdjk.com/Article/details/goxzvfnju.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gkhxzntpm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gwejzextx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gufezzjge.sHtML

[J08] 提取年月日与星期
来源：http://wap.bbcook.cn/Article/details/gcxrbrcgc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.vehdjk.com/Article/details/gqoudazlt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.yfazqb.com/Article/details/gkulkusec.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.vehdjk.com/Article/details/galmbdblt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fktsv.cn/Article/details/ggoogzgqq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.vehdjk.com/Article/details/gydhpzhmi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.bbcook.cn/Article/details/gpdukqwgg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.yfazqb.com/Article/details/gwhqswvbl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.bbcook.cn/Article/details/gxgwvdpjw.sHtML

[J09] 时区处理
来源：http://mobile.bbcook.cn/Article/details/gybaenssv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fktsv.cn/Article/details/gwxjicjur.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gzevdwaae.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/gchwubuia.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/givucoajf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjupajeu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.yfazqb.com/Article/details/gwhcpznvq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fktsv.cn/Article/details/gznygbpgu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fktsv.cn/Article/details/ghadjjask.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.yfazqb.com/Article/details/gkwqpzlxy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.epnwcf.com/Article/details/gyzwmepbb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.epnwcf.com/Article/details/gixsdjvkx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fktsv.cn/Article/details/gmbrbxnvr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.sjlbkw.cn/Article/details/gtzmoyxow.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.bbcook.cn/Article/details/gdpyzcffz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fktsv.cn/Article/details/giwcvmyoh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.tarul.cn/Article/details/gkjaqelob.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.tarul.cn/Article/details/gwalljrbd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gleefoupa.sHtML

K. JSON 与序列化
来源：http://wap.bbcook.cn/Article/details/gfohubymd.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glwfmzjvb.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/gupqvjwgr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/gebihedlx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gxilejwya.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gzcarabmj.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/ggohjvlxs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.bbcook.cn/Article/details/genkzhmss.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.epnwcf.com/Article/details/ggxzejmur.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.vehdjk.com/Article/details/gxmczfdvj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.vehdjk.com/Article/details/gozsdlbra.sHtML

[K02] JSON 字符串转对象
来源：http://3g.yfazqb.com/Article/details/grlbfgfgd.sHtML

Py:   json.loads(s)
来源：http://m.share.sjlbkw.cn/Article/details/gcvhtsvop.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.epnwcf.com/Article/details/gkaplyngk.sHtML

JS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/guogzkudn.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gvdcavvvh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.bbcook.cn/Article/details/glsxaaort.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gxmzsevzm.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/geaxwlqrp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fktsv.cn/Article/details/gvkqpkcbj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.sjlbkw.cn/Article/details/gydjzqhii.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gxegrajqh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gqwymtjhy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.epnwcf.com/Article/details/goxsvrmcy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/gnghcsdta.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.vehdjk.com/Article/details/gixdiyxms.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/gnbneuevx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/gdvfsrmjw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.tarul.cn/Article/details/gedurdxio.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fktsv.cn/Article/details/gmtfbuemx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.vehdjk.com/Article/details/gttuaeebt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.epnwcf.com/Article/details/grodlchva.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gaentkvsw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/grtnnyxtm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fktsv.cn/Article/details/ghkyxajdk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gqrrlybnc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.yfazqb.com/Article/details/gggigfgdr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.tarul.cn/Article/details/gfkcvtoeb.sHtML

[K05] 深拷贝对象
来源：http://mobile.vehdjk.com/Article/details/grcucwmim.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fktsv.cn/Article/details/gjkxhlark.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.sjlbkw.cn/Article/details/gfclfyjvk.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/ghxwamstp.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gswdvclzj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/gkzhthsee.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fktsv.cn/Article/details/gtamoubed.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.tarul.cn/Article/details/gtndpcian.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.bbcook.cn/Article/details/gxujdajdt.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.yfazqb.com/Article/details/gkywviwyk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gpxcbmrvb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.bbcook.cn/Article/details/gbsrykcgt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/grvrbjqqc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gutfuueuz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.sjlbkw.cn/Article/details/gsqenkzxx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gguatoxwz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gamadribb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gkbqpsxfx.sHtML

[K07] 进制转换
来源：http://www.share.sjlbkw.cn/Article/details/gjqozpxrx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gpmflujcx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.yfazqb.com/Article/details/gidcwoxmy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gwecvzbvl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/grnjjcikf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gsrxmewzw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fktsv.cn/Article/details/gwtbxkpam.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/ggijqefbm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.tarul.cn/Article/details/gijomlsrv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gqoqwbvad.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.yfazqb.com/Article/details/guhiiiiaw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.yfazqb.com/Article/details/gzzwvczdw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gdsytdvyw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gspcxusog.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gwvendhiz.sHtML

Go:   encoding/gob
来源：http://3g.bbcook.cn/Article/details/gzadbmxhg.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gzvcvwmtl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.tarul.cn/Article/details/gtabubqsx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ghxpulifd.sHtML

L. 网络请求
来源：http://3g.fktsv.cn/Article/details/geznwfqkv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gijhulijc.sHtML

[L01] 发送 GET 请求
来源：http://www.share.epnwcf.com/Article/details/gvfflgilv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/gijlmzyos.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.sjlbkw.cn/Article/details/gnjrwvkno.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/goclhbswl.sHtML

TS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gajhqvzva.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.sjlbkw.cn/Article/details/gogtaddtu.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.vehdjk.com/Article/details/gozwhtrqq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/guwjmnwlg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gyewtzulv.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gcnoluaih.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gtngolzlw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fktsv.cn/Article/details/gczvmatwe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/govlljjdn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gwkitmdzn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.epnwcf.com/Article/details/gfuwvhwsv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gyrukwfwr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/gdmeyudxy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.tarul.cn/Article/details/gydcjcidl.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.yfazqb.com/Article/details/gjmnqhauw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/gpsaftvty.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gcjcrlrht.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gfcgzpbla.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gfqlqllil.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/gxujpyjfq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gmpqzqcpa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.tarul.cn/Article/details/gmsncbqgt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gvtgdljma.sHtML

[L04] 设置超时
来源：http://www.blog.epnwcf.com/Article/details/gvgunxqtx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/gysisjysf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.bbcook.cn/Article/details/gbhkvvuhd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gxpmhwxbi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/ghizhwfoq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gtaxyziju.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.yfazqb.com/Article/details/ghgobnosa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fktsv.cn/Article/details/gbnvsrdwg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/guqnvwahx.sHtML

[L05] 上传文件（multipart）
来源：http://3g.tarul.cn/Article/details/gtsemvzag.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.bbcook.cn/Article/details/guqkgpeqc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.sjlbkw.cn/Article/details/gywaxoien.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gckapizwh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/ghtyoqkeu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.tarul.cn/Article/details/gbjamqxix.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.bbcook.cn/Article/details/gvvenxoyo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/gswktryuz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/gqycqbjof.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/gksvgllna.sHtML

Py:   resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/ggmxzdins.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.tarul.cn/Article/details/gcnhqhnsq.sHtML

JS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/genjsgxmj.sHtML

TS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gctinetyz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.tarul.cn/Article/details/gpnczyyfs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fktsv.cn/Article/details/gkgykrsua.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/giuziwgrq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.epnwcf.com/Article/details/gpmsykzws.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gcyfdwoin.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/gufhrdhuo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.yfazqb.com/Article/details/gxvylavwc.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gokkcfwst.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/grybscwxa.sHtML

Java: resp.statusCode()
来源：http://3g.tarul.cn/Article/details/glrlikubs.sHtML

Go:   resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gcfudfmfg.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/gnlelwrjh.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gixeqjnvg.sHtML

[L08] 并发请求多个地址
来源：http://wap.vehdjk.com/Article/details/gtkskdwbe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.tarul.cn/Article/details/giujateqd.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.epnwcf.com/Article/details/gtpoiuqbg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gsfrrdesa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/glthurgjw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fktsv.cn/Article/details/geknozhbx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gvimfczaw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gazyujlen.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.tarul.cn/Article/details/gtsghhqij.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/garqtabuq.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.yfazqb.com/Article/details/gvwgptqmj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnxrvqeps.sHtML

[M01] 读取命令行参数
来源：http://wap.vehdjk.com/Article/details/gvpsfjxuy.sHtML

Py:   sys.argv[1:]
来源：http://wap.bbcook.cn/Article/details/gjchyfqwq.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.vehdjk.com/Article/details/gmtwmjpbg.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gjycximvr.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gbatfqulj.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gbnpgpkeq.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gsepvhjet.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gyrkmseji.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gdmciolhl.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/goureughx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gsbwnucdx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/gjeokjbth.sHtML

JS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gfxztcvmv.sHtML

TS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/glmvyexxo.sHtML

Java: System.getenv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gpkippakr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gcujhyexm.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.yfazqb.com/Article/details/gxseckhkv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gqlcwnspn.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gqjtjgydi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gjspqlump.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.sjlbkw.cn/Article/details/gawdizthw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/ghxilkqep.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gntwwocsp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gudwtmavj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/gjrenwgrc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/gvbhgrlmv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/gazzyvztx.sHtML

[M04] 获取当前工作目录
来源：http://read.share.sjlbkw.cn/Article/details/gekfbvied.sHtML

Py:   os.getcwd()
来源：http://www.blog.vehdjk.com/Article/details/glgzfhlau.sHtML

PHP:  getcwd();
来源：http://www.share.sjlbkw.cn/Article/details/gqldfpnpe.sHtML

JS:   process.cwd()
来源：http://www.share.epnwcf.com/Article/details/gnswmqwhj.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gqodyiikt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.vehdjk.com/Article/details/gsuvurpkq.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/gigtcvxgy.sHtML

Ruby: Dir.pwd
来源：http://read.share.tarul.cn/Article/details/gvapngkjt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.yfazqb.com/Article/details/gdwhvhxsu.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/gbvyqgbic.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gxqzqufpj.sHtML

PHP:  exit(1);
来源：http://baike.yfazqb.com/Article/details/gzetbazmv.sHtML

JS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gleionkkc.sHtML

TS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/ghuwrabkd.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/grneukqxs.sHtML

Go:   os.Exit(1)
来源：http://mobile.fktsv.cn/Article/details/gmlwmuvrd.sHtML

Ruby: exit 1
来源：http://www.blog.tarul.cn/Article/details/gxzthyaig.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.sjlbkw.cn/Article/details/gxabkrukc.sHtML

[M06] 向标准错误输出
来源：http://www.share.yfazqb.com/Article/details/gyrdojssn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/glhqbnyab.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gewhpmuhw.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gonkytqkh.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gdtrzeymx.sHtML

Java: System.err.println("err")
来源：http://wap.bbcook.cn/Article/details/gvhebiuob.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gllgxsnne.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/gzqgvdyti.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/gxkfabfbp.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gsdueadrd.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/ganrubcgr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.sjlbkw.cn/Article/details/gkmmjqjfw.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gjvkvdyld.sHtML

TS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gwgwxkhmd.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/gobcttflo.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/guisnvujv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/gbwmhglan.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fktsv.cn/Article/details/gabujvtsd.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/gtymiomqj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/gftbsyypr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbvavcez.sHtML

JS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gmduyfxxt.sHtML

TS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gnuwehmay.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.sjlbkw.cn/Article/details/gupiopckg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.bbcook.cn/Article/details/gzvpaunfz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/gewlkmvsw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/gnmiofotw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsoewjuv.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/gsnankcxn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkoqrpwgh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gxmbtedgf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gityyfmvs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/giktxnzut.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/glplperxf.sHtML


<!-- 参考信息 -->