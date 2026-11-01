代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/gkylnuctt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gwbbxpvlt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gibweghyb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gvbskuedh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fktsv.cn/Article/details/gmkajqhmn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/gfcacnbzj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gxtpdrybq.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gynfpoddx.sHtML

J. 日期与时间
来源：http://wap.tarul.cn/Article/details/grdsbrnfs.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjmxujqex.sHtML

[J01] 获取当前时间
来源：http://www.m.share.yfazqb.com/Article/details/guttxwezq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.epnwcf.com/Article/details/ghraqtjpy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gbbgxgkus.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/giyphynit.sHtML

TS:   new Date();  Date.now()
来源：http://blog.tarul.cn/Article/details/gnbftydaz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/gbwbjwkeh.sHtML

Go:   time.Now()
来源：http://3g.sjlbkw.cn/Article/details/gvnywtzlo.sHtML

Ruby: Time.now
来源：http://baike.vehdjk.com/Article/details/gpaaolicq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.vehdjk.com/Article/details/gdeygbgpv.sHtML

[J02] 格式化输出
来源：http://read.share.tarul.cn/Article/details/geadrjcuc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.sjlbkw.cn/Article/details/glpmubzpe.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/ghwoafpsl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.yfazqb.com/Article/details/goyknsfsc.sHtML

TS:   d.toISOString()
来源：http://mobile.tarul.cn/Article/details/gyzprqbna.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.vehdjk.com/Article/details/gtozpmtmb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.yfazqb.com/Article/details/gllxxsiza.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/gcpikjljl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.vehdjk.com/Article/details/gydvfylmx.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.epnwcf.com/Article/details/gjqgcdahn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gntppbuol.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.tarul.cn/Article/details/gwblzsspt.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gikwenign.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gbqriinrw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gkvbemjjp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gyuziqkib.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/ggfxoangj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkggeuszk.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.epnwcf.com/Article/details/gzosuwhde.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.sjlbkw.cn/Article/details/girxopjsu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/gfmgwgsdb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.yfazqb.com/Article/details/gnxmxtttl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.vehdjk.com/Article/details/gnsohxsok.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fktsv.cn/Article/details/gghifxxsi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.yfazqb.com/Article/details/gilsnilyn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gbajdafvo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gixyiynyd.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.bbcook.cn/Article/details/gttcqnnss.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fktsv.cn/Article/details/gckaxbwqz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.epnwcf.com/Article/details/gxfguajqw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gwyrtwzyr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/gzrbtohxi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.epnwcf.com/Article/details/glarrgndb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.bbcook.cn/Article/details/gytnihwlm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.bbcook.cn/Article/details/gnkhtphkc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/glvinoslr.sHtML

[J06] 计算两时间之差
来源：http://blog.fktsv.cn/Article/details/gcpdimoma.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.bbcook.cn/Article/details/gymwcjcaa.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.vehdjk.com/Article/details/gaafwmruh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.epnwcf.com/Article/details/gpllgahmd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.vehdjk.com/Article/details/gsbuilrto.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.epnwcf.com/Article/details/grosfrwvl.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gryqttivw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.tarul.cn/Article/details/gcffdkfrf.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.tarul.cn/Article/details/gxewpgpqv.sHtML

[J07] 比较两个日期
来源：http://baike.sjlbkw.cn/Article/details/gcxdzccsd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/glslymdpv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fktsv.cn/Article/details/gwtdtmvve.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/ggkaeyqhn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fktsv.cn/Article/details/gfxxcuwtq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fktsv.cn/Article/details/gwgjhdgft.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/goanqrkrf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/glllagjut.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/ggqeobcwb.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.vehdjk.com/Article/details/glumusznu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.tarul.cn/Article/details/gwbrpseol.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.sjlbkw.cn/Article/details/gpyssbgzb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.epnwcf.com/Article/details/gkxvqexcm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.epnwcf.com/Article/details/gwdavfyrj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.sjlbkw.cn/Article/details/gilvnjtcf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.tarul.cn/Article/details/ghofueyps.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.bbcook.cn/Article/details/gjjipiwbj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.yfazqb.com/Article/details/gifhmealo.sHtML

[J09] 时区处理
来源：http://baike.epnwcf.com/Article/details/goscvuleo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.vehdjk.com/Article/details/gsthtwfhu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.vehdjk.com/Article/details/gatopxhgl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gjzfymwfu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gfqmanoga.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.bbcook.cn/Article/details/gnxfcqahh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.epnwcf.com/Article/details/gxdcjuqgo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/ghuleyirj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.bbcook.cn/Article/details/gselawugb.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.vehdjk.com/Article/details/gajpbxxxh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/gnxkeudxn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.vehdjk.com/Article/details/ggyktftnl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.yfazqb.com/Article/details/gdqjhijbx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gnsfovhsu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.sjlbkw.cn/Article/details/ghdomaewo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.tarul.cn/Article/details/gkwabrniu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.epnwcf.com/Article/details/gqdclawcv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.vehdjk.com/Article/details/gmunoddzj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwehytfdf.sHtML

K. JSON 与序列化
来源：http://baike.epnwcf.com/Article/details/gksqvzjgp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmbprrwss.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/gjqkezyaf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/gazzutuvs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gysmkrinn.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gjvifsxzn.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/gqxpbbcsw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.yfazqb.com/Article/details/gnjaushqo.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.yfazqb.com/Article/details/ganuvnckk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fktsv.cn/Article/details/gkfgmypea.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.vehdjk.com/Article/details/grudqrqro.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gozypstls.sHtML

Py:   json.loads(s)
来源：http://read.share.bbcook.cn/Article/details/gvcxsnnbs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.tarul.cn/Article/details/gzxmewwok.sHtML

JS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gmycaggze.sHtML

TS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/grrfqzzcc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/ggrhpkmli.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gltjvjqai.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gzmcqpnsu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fktsv.cn/Article/details/gyxjbhwkd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.vehdjk.com/Article/details/galarjhpf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/gnxtwblzs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gqjbnvups.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gukzenilr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/gkyanykmo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.tarul.cn/Article/details/gwktrldsn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.vehdjk.com/Article/details/gfuwwcwzh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fktsv.cn/Article/details/ggzxewuya.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.tarul.cn/Article/details/gdesdvthd.sHtML

[K04] 读取 JSON 文件
来源：http://3g.tarul.cn/Article/details/guihizcid.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.epnwcf.com/Article/details/gkqheczng.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.vehdjk.com/Article/details/gruydlwio.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/gzqdzzcqy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gphfbdxva.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gwyzxmfma.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.vehdjk.com/Article/details/ghzypshzb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.bbcook.cn/Article/details/gkhikznqh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gadbhwqht.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/gbfuassgi.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.bbcook.cn/Article/details/gorfmddnz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.epnwcf.com/Article/details/ggyklpynu.sHtML

JS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gpkgckbre.sHtML

TS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gpfsqscfy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fktsv.cn/Article/details/gehxtnbux.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gwapofqfg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gjlyucoyy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.tarul.cn/Article/details/gyrgofsrl.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.sjlbkw.cn/Article/details/grlzllfal.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.tarul.cn/Article/details/gsgfdeodw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/giwxiswxl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/ggptqazkd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gxevdrgju.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.vehdjk.com/Article/details/gplqiaeja.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/ghpxyfmlx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gltkhnyts.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gvaidttxl.sHtML

[K07] 进制转换
来源：http://blog.epnwcf.com/Article/details/gxcpuycqx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gdvsyrfdt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.yfazqb.com/Article/details/gfvgnwdhh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gtljqkflz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gimrvjlcj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gdzzmiqkq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.bbcook.cn/Article/details/gfzmryvcf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.sjlbkw.cn/Article/details/gnfhyfzxk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gwydhxciv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.epnwcf.com/Article/details/gykiqgvyd.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/gzqkhywsk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/gtlkhqphw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gwkooqqmt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gbzgnkpir.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.vehdjk.com/Article/details/goxmsaubi.sHtML

Go:   encoding/gob
来源：http://read.share.tarul.cn/Article/details/gzkjstcot.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gxeqrdqmt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gevlljlch.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvtnrbqdd.sHtML

L. 网络请求
来源：http://read.share.fktsv.cn/Article/details/gpblywclw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwsejhtpt.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/groqxmakf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.bbcook.cn/Article/details/gafszxfva.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/glyyezbio.sHtML

JS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gfztxtevb.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gmbjaexav.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/goteldnoq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gyqpdjdvl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/gqwveiojx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.epnwcf.com/Article/details/gqkpqutnx.sHtML

[L02] 发送 POST JSON
来源：http://blog.tarul.cn/Article/details/goxlhdmsz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.bbcook.cn/Article/details/grzlxdnhf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fktsv.cn/Article/details/gckqgvibn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gmxkqdviv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gzmsmqndq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.yfazqb.com/Article/details/gdxzphlvh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.epnwcf.com/Article/details/gkbgaezfh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.yfazqb.com/Article/details/gzzdwivna.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.sjlbkw.cn/Article/details/ghvxadist.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/gamnbvssp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.vehdjk.com/Article/details/ghcotwssi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fktsv.cn/Article/details/gwnsllwwi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gteyfyddo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gfiesxrpt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/govsrdhoj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/ggfdajipa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.bbcook.cn/Article/details/gylmqirjw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gyemzjaym.sHtML

[L04] 设置超时
来源：http://blog.bbcook.cn/Article/details/grsjtdfvu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.sjlbkw.cn/Article/details/gmgduguxe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.yfazqb.com/Article/details/geryccrdd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gjhtlrohb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gvubznpet.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.epnwcf.com/Article/details/gqcfgevyo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gfryandng.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.bbcook.cn/Article/details/gdutwyrcu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/gtobszrfg.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fktsv.cn/Article/details/gxvnfgkos.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.tarul.cn/Article/details/gfomjkipf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/glettbcfy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gyhcfkjog.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gxxgkimkc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.epnwcf.com/Article/details/getuzhdek.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/gvarthhzw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.sjlbkw.cn/Article/details/gbrvmfboe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gbzheijhz.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fktsv.cn/Article/details/gzviflvbc.sHtML

Py:   resp.json()
来源：http://wap.yfazqb.com/Article/details/gptwdldqb.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/gounsaqml.sHtML

JS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gdmqbddfc.sHtML

TS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/gjahdenjx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvfbciwq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.vehdjk.com/Article/details/gutipprfy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/grtszwqbp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.tarul.cn/Article/details/gjoqydyco.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gihrrdkca.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gemzyufrx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.yfazqb.com/Article/details/gmztohhxs.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gxvajzrdl.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/guwmhkzbq.sHtML

Java: resp.statusCode()
来源：http://www.share.bbcook.cn/Article/details/gwrpgjvuq.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/glvchjblh.sHtML

Ruby: resp.code.to_i
来源：http://mobile.vehdjk.com/Article/details/gqfxumrte.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gitfqkzka.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/glxvmwwxm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.bbcook.cn/Article/details/goiiazxim.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.epnwcf.com/Article/details/gectxhdyw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gwqqopnuh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/ghufcmnto.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.vehdjk.com/Article/details/gywcticcg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.tarul.cn/Article/details/gwzscpefv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.vehdjk.com/Article/details/ghjaksbjb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/gzqfqoewm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gipormyka.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.vehdjk.com/Article/details/gyioqxxfl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gugpsmkes.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gagkdhpuo.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gfyuatvnw.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fktsv.cn/Article/details/glovvbjnm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gwlkzvkxg.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gdopznlxr.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.tarul.cn/Article/details/gvbuhxymq.sHtML

Go:   os.Args[1:]
来源：http://m.share.bbcook.cn/Article/details/gishhdudi.sHtML

Ruby: ARGV
来源：http://www.blog.yfazqb.com/Article/details/gpovfbegc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gwynmcxta.sHtML

[M02] 读取环境变量
来源：http://blog.tarul.cn/Article/details/gofplzdgm.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gsaytyojf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gbviwnsoh.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gbmxpqkjg.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gylswwmxm.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/guoqdhcon.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.vehdjk.com/Article/details/gnkhojvys.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fktsv.cn/Article/details/gkaqyyybk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/gzzrrrrxr.sHtML

[M03] 执行外部命令
来源：http://read.share.tarul.cn/Article/details/gkempltey.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/gzwjsyeih.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/gxmpusdqi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gesflcdez.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gedkzskhg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.tarul.cn/Article/details/gdvxonrik.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gvrrbkudl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.sjlbkw.cn/Article/details/gslfzhqbl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/gwgtmwonf.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/geubytuio.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/gdpqqteul.sHtML

PHP:  getcwd();
来源：http://baike.fktsv.cn/Article/details/gaiiieegd.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gxzsdxzmj.sHtML

TS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gpnjgrmrb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.tarul.cn/Article/details/gwosgyknh.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gawadgrih.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gvfgufnoq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.yfazqb.com/Article/details/gsjvdszrx.sHtML

[M05] 设置退出码
来源：http://3g.sjlbkw.cn/Article/details/grvwpcqfg.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gnsxmuuls.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gncfagisc.sHtML

JS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gfomiewqt.sHtML

TS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gzoutrdnm.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/gchgnaizz.sHtML

Go:   os.Exit(1)
来源：http://wap.fktsv.cn/Article/details/gkuaecofi.sHtML

Ruby: exit 1
来源：http://m.share.tarul.cn/Article/details/gmgfvbwxq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.bbcook.cn/Article/details/gtbnhwpsx.sHtML

[M06] 向标准错误输出
来源：http://www.blog.sjlbkw.cn/Article/details/gjooxofof.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gvrtsbwmn.sHtML


<!-- 参考信息 -->