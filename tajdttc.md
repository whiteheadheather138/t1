代发 wailian999

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gpgyiefzr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gzmqiaion.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gwyslbqdf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gtaucuvsu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/ghftbiffh.sHtML

[J04] 时间戳与日期互转
来源：http://3g.sjlbkw.cn/Article/details/gkbshxutu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.vehdjk.com/Article/details/gkbouhpxx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.sjlbkw.cn/Article/details/gsrkkfrpy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.yfazqb.com/Article/details/gvsoymbwl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.vehdjk.com/Article/details/gejnamgvk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.tarul.cn/Article/details/gsmiwooka.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.tarul.cn/Article/details/gjqtuqwek.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gvhktbtmh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.yfazqb.com/Article/details/gzefoaswq.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.vehdjk.com/Article/details/ggmgdmojz.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.tarul.cn/Article/details/grmjpkflg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.bbcook.cn/Article/details/gyeneccjl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/gbrejqlwm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gyxqytfqn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.vehdjk.com/Article/details/gbqvqcxvz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.sjlbkw.cn/Article/details/gjxhjxgdd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/gcpvohbzf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.epnwcf.com/Article/details/glgxdofrv.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqxubacr.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.vehdjk.com/Article/details/gtcygrooi.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fktsv.cn/Article/details/guwyllqph.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgirwxhs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.vehdjk.com/Article/details/gkwzrofzx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.tarul.cn/Article/details/gexetrrup.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gkxqrfcfl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.epnwcf.com/Article/details/givuspypp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.bbcook.cn/Article/details/ghqnlzdzr.sHtML

[J07] 比较两个日期
来源：http://read.share.tarul.cn/Article/details/gsmisghtb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/grzyqezvo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fktsv.cn/Article/details/gwmhvwwmu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gdinhkiuy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/gmaqqtsnv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.tarul.cn/Article/details/gnootfdvo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fktsv.cn/Article/details/gfvefnfti.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gufyllsdw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gbmocesca.sHtML

[J08] 提取年月日与星期
来源：http://m.share.vehdjk.com/Article/details/ggukdbxlg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.bbcook.cn/Article/details/grbpmmnwe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gdclmxocw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.sjlbkw.cn/Article/details/ghijnjwnd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.yfazqb.com/Article/details/gzieqexct.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/gaxlquxtq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.yfazqb.com/Article/details/gedteatba.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.epnwcf.com/Article/details/gcfwusnbd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/gdladaubq.sHtML

[J09] 时区处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gxodhjxvx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.vehdjk.com/Article/details/gkakcfdiw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.epnwcf.com/Article/details/givtfjqam.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gsewicuws.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gfsoouwrl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.sjlbkw.cn/Article/details/gkadptkqn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.vehdjk.com/Article/details/gvqlksunw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.epnwcf.com/Article/details/guwskleal.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.tarul.cn/Article/details/gkbggaplz.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.epnwcf.com/Article/details/gwmkiiwpl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/gnwjwicos.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.sjlbkw.cn/Article/details/gjavlkbav.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gaqvvwrev.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fktsv.cn/Article/details/gygehyfuy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.bbcook.cn/Article/details/gkrsehqaq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.tarul.cn/Article/details/gdvllzhcs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.epnwcf.com/Article/details/gjsdajrng.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gjvyrnvcl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjysjqxpt.sHtML

K. JSON 与序列化
来源：http://www.blog.sjlbkw.cn/Article/details/gfspyghbc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gferkrqph.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.yfazqb.com/Article/details/gquwvrxjp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gxvdnafsk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gbxznwuao.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ghdkzfnxj.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gwymekriq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.bbcook.cn/Article/details/gnpzjgmgp.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fktsv.cn/Article/details/ganugtosk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.epnwcf.com/Article/details/gonitaayq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.epnwcf.com/Article/details/gsitonqzz.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.bbcook.cn/Article/details/gylupmddl.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gflnvdowg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/gfanrvwip.sHtML

JS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gucujlrpa.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gfwibcpvz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.vehdjk.com/Article/details/ggxsddwib.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gopmhjjzp.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/grwagmatb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gvawhsdxk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/gawtwsexx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/grlsjwjlt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/glfxnydwv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gtsbeeeai.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gqeilcpkg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.epnwcf.com/Article/details/gzrbrvkis.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/gbnrzzeel.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.yfazqb.com/Article/details/gfharebvz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.tarul.cn/Article/details/gocwgsvre.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.bbcook.cn/Article/details/ggqkeersn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fktsv.cn/Article/details/giahjitbt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.epnwcf.com/Article/details/glwepcqbe.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/galehadeo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gibdlotqp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.vehdjk.com/Article/details/gxqjtntto.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gouihsger.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.epnwcf.com/Article/details/gigwzjeow.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.vehdjk.com/Article/details/gcoxtflst.sHtML

[K05] 深拷贝对象
来源：http://m.share.yfazqb.com/Article/details/gbpysmjts.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gbykcamrj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.vehdjk.com/Article/details/gujerfldy.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gwfvzzjsg.sHtML

TS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gxcmpamna.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.tarul.cn/Article/details/gnrjzziyj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gswplmreq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.tarul.cn/Article/details/gjwxnulio.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbswjvdv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fktsv.cn/Article/details/geuutlllp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gckyabagp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.yfazqb.com/Article/details/gsfdxjlhn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/ganxtjwhu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gojewkemi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.vehdjk.com/Article/details/gmyucfsem.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gfgfxycbp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/ghsfvjbdn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/grwiwwpvt.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gbgoyietd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gtxfvuiwv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.vehdjk.com/Article/details/gedbsxddr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gsnekoepi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gbbrgxosb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gkucbalsl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fktsv.cn/Article/details/gizaczqln.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.epnwcf.com/Article/details/gfajfspkn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gnyniedco.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.vehdjk.com/Article/details/gdmahgqtq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gmvoyzhok.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.vehdjk.com/Article/details/gcusgwyth.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gakqjnbce.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gjcevctnl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.tarul.cn/Article/details/gpsuzhprk.sHtML

Go:   encoding/gob
来源：http://wap.sjlbkw.cn/Article/details/gibjaltrk.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.bbcook.cn/Article/details/guysbuxxn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gwlvanifp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbldldoqr.sHtML

L. 网络请求
来源：http://3g.vehdjk.com/Article/details/gqxtxookd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ggihedblu.sHtML

[L01] 发送 GET 请求
来源：http://baike.epnwcf.com/Article/details/gjcmhlhrh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fktsv.cn/Article/details/gxjpknjab.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.bbcook.cn/Article/details/gjrjikied.sHtML

JS:   await fetch(url)
来源：http://www.share.tarul.cn/Article/details/goidipynv.sHtML

TS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gjaqcureo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.epnwcf.com/Article/details/gjfdvmmvy.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.tarul.cn/Article/details/gvlckpamv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fktsv.cn/Article/details/ghnzrimzr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.tarul.cn/Article/details/gplwczuvq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gdixyrkta.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gxuptmeog.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.vehdjk.com/Article/details/glvxbdadt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/gplhdjrzn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gqffrehoz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.yfazqb.com/Article/details/glqcksdzl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.yfazqb.com/Article/details/ghxjdtbzq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.bbcook.cn/Article/details/gvkbpcsul.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/gwuehquxo.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.sjlbkw.cn/Article/details/gjaoixvea.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.bbcook.cn/Article/details/giuxvgzjl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.tarul.cn/Article/details/gyyacgmxf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/gqnovzuuz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gmaghbnhv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/gpnjwhzgi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gpnvmbwjf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/ghwxoczlh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/gkraipwfw.sHtML

[L04] 设置超时
来源：http://www.share.epnwcf.com/Article/details/gxlttcvws.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.epnwcf.com/Article/details/gmjhrajvx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gzfodbvjy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gbqqxgxhn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gnvkgphtx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.bbcook.cn/Article/details/gdhhjaujz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.epnwcf.com/Article/details/gfdvltlof.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.epnwcf.com/Article/details/gurvbsets.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/gcveagnhd.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/gcppjdbzv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.vehdjk.com/Article/details/gqnznogng.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/gsylebywe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/gaewrqimk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gyslnkuqg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.yfazqb.com/Article/details/gexiesswa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/glhveaoyy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gdrhfsfwp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.tarul.cn/Article/details/gjcunfkkp.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gexjounrh.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/ghjuemtej.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/grtqcvljc.sHtML

JS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/ghqmxzfom.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/ggvoivvab.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gahrxjdxw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.tarul.cn/Article/details/gcndocswa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.sjlbkw.cn/Article/details/guioczhry.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gthlkqcpv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gvnyzvavr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/gtxhyllbd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.vehdjk.com/Article/details/gdadrcwkr.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gojxhouba.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gluderxho.sHtML

Java: resp.statusCode()
来源：http://www.blog.sjlbkw.cn/Article/details/gfrrnvwfz.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/gzywuqqee.sHtML

Ruby: resp.code.to_i
来源：http://blog.sjlbkw.cn/Article/details/gxgfspfrm.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/giulxdgoz.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.vehdjk.com/Article/details/gtshnsuxw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/ggvwqxnto.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/grzgwztvf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gbyeggbfz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gqlixitjs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.tarul.cn/Article/details/gdmerorya.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.epnwcf.com/Article/details/gpcobjvsd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/ggpsdzkvn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.sjlbkw.cn/Article/details/gagwzvkki.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcnoexukh.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/ghxuvtcbq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/guayaepko.sHtML

[M01] 读取命令行参数
来源：http://read.share.fktsv.cn/Article/details/gjruvfonq.sHtML

Py:   sys.argv[1:]
来源：http://baike.epnwcf.com/Article/details/guuukdqen.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gznsvrsst.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gosdqfiew.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gzijyftfa.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gpialajvr.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gvofocehq.sHtML

Ruby: ARGV
来源：http://mobile.bbcook.cn/Article/details/gekfvbkwv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gatdquoor.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gkkfjmmuh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gdrtxtebw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gtorkravd.sHtML

JS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gcwbfysus.sHtML

TS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gijbgwshx.sHtML

Java: System.getenv("HOME")
来源：http://3g.epnwcf.com/Article/details/ghrfrwvkp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gohcqyyoc.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/gsvnigwfy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/goumprtkd.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwbandwj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fktsv.cn/Article/details/gbbnjzmvs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gzbmrcwql.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gpsmlczuq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/glgkqlxoj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gwfdbhvqk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.tarul.cn/Article/details/gyqhnghjt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.sjlbkw.cn/Article/details/grbvkgiat.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.bbcook.cn/Article/details/gzykncojl.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/gsgsjhyht.sHtML

Py:   os.getcwd()
来源：http://blog.vehdjk.com/Article/details/giscxzbaj.sHtML

PHP:  getcwd();
来源：http://wap.sjlbkw.cn/Article/details/gquijboyh.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gtfkkbczt.sHtML

TS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gclwtcvbp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fktsv.cn/Article/details/gpujjaejf.sHtML

Go:   os.Getwd()
来源：http://3g.vehdjk.com/Article/details/goovwggol.sHtML

Ruby: Dir.pwd
来源：http://m.share.tarul.cn/Article/details/ghgwonyif.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gvrlfyymt.sHtML

[M05] 设置退出码
来源：http://m.share.tarul.cn/Article/details/gnbexsqwp.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/gjtbkcovf.sHtML

PHP:  exit(1);
来源：http://blog.yfazqb.com/Article/details/gmljfqiub.sHtML

JS:   process.exit(1)
来源：http://wap.fktsv.cn/Article/details/gdmfucrgz.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gobtqccwc.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/glohfdyzi.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gqfhxpikz.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/govlekccs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.tarul.cn/Article/details/gzrmhmlqs.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gizosnsce.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/ggyhmbekq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gdvdfbwya.sHtML

JS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gedbiqfss.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gyzhnqpgo.sHtML

Java: System.err.println("err")
来源：http://read.share.yfazqb.com/Article/details/gqkowimvv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/gspptwuhk.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gcrlfdoac.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.sjlbkw.cn/Article/details/gmbvhordf.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gqrhlikzi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.bbcook.cn/Article/details/ggjjfauwq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.bbcook.cn/Article/details/gauhcrovr.sHtML

JS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/grhlmtyqw.sHtML

TS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gmhkbjnfg.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/giqzvneol.sHtML

Go:   func main()
来源：http://3g.sjlbkw.cn/Article/details/gijlycuta.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.yfazqb.com/Article/details/ggxkojdfw.sHtML

C#:   static void Main(string[] args)
来源：http://wap.sjlbkw.cn/Article/details/geyqmctya.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/gasbhybdf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.yfazqb.com/Article/details/glavynezr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/giabvuohl.sHtML

JS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gssioxwps.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gotyzryuq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/gablulsop.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/gdcaxtgeh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/gmjhmouao.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.bbcook.cn/Article/details/gwyewlseu.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/goqwddfmq.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/ghkwvyzcu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grchhztwu.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/glsebcbqg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gnqmnspda.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gogosjtio.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gpvercsdi.sHtML


<!-- 参考信息 -->