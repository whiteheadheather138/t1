代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.sjlbkw.cn/Article/details/gqagsusxx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gkwuvtfej.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gjxsjnsnt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gjtofwxkg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.epnwcf.com/Article/details/gkvfetill.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.vehdjk.com/Article/details/gkzwziaod.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gwzhzdyzh.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzkejowlh.sHtML

J. 日期与时间
来源：http://wap.fktsv.cn/Article/details/gsjypycjw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gopovwipb.sHtML

[J01] 获取当前时间
来源：http://www.blog.vehdjk.com/Article/details/ghtvbryzi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/gebrxphsv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/gpzhwtpbw.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/ghteulrly.sHtML

TS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gjoyrorpw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.epnwcf.com/Article/details/gtkeuptyz.sHtML

Go:   time.Now()
来源：http://baike.vehdjk.com/Article/details/gsznzmsus.sHtML

Ruby: Time.now
来源：http://mobile.sjlbkw.cn/Article/details/gjtdukeix.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.yfazqb.com/Article/details/ggslfpdit.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gfncgzjeu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/grieqsier.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gmhtiifjc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fktsv.cn/Article/details/gsrvekxwx.sHtML

TS:   d.toISOString()
来源：http://blog.epnwcf.com/Article/details/gpekdqxqx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.epnwcf.com/Article/details/grlupocsp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gfbckcabr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/grjyovtgl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.tarul.cn/Article/details/gbmhmsrty.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.sjlbkw.cn/Article/details/gntqrejjj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.epnwcf.com/Article/details/gwbudihyp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.bbcook.cn/Article/details/giqqqikjc.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/glzdxofio.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gabuhvjan.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gtrxnhzrg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gnaljxawq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gapurwoad.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.sjlbkw.cn/Article/details/gcmdilhum.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/gphzkdcfo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.epnwcf.com/Article/details/ggohiqhbm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.vehdjk.com/Article/details/gxzjstpjb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gqsyxncfn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fktsv.cn/Article/details/gjzcdtbkq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.tarul.cn/Article/details/gzrgszmgv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/gwxapczyf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fktsv.cn/Article/details/gcpfzztol.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.yfazqb.com/Article/details/gclcvgvxg.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.bbcook.cn/Article/details/gbujscbsg.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.bbcook.cn/Article/details/gvflbirbh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fktsv.cn/Article/details/gfrkbaqjl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/giuncmtpm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/gkrnywhyh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/ggreliims.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fktsv.cn/Article/details/gsqimsgif.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/grkiebepa.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/garctuvoy.sHtML

[J06] 计算两时间之差
来源：http://mobile.yfazqb.com/Article/details/gbtozxusd.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fktsv.cn/Article/details/ghjtdydwc.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/gqggggkmz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/gzikzxsby.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.bbcook.cn/Article/details/gtbunilyc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.bbcook.cn/Article/details/geoloonpn.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.vehdjk.com/Article/details/gumpfzgwz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.epnwcf.com/Article/details/gozyzgiex.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.tarul.cn/Article/details/goyvyrzfu.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/gsuuiwucl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/ggcrfduyt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.vehdjk.com/Article/details/gjgjpwboq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlkafwyt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/geoojdmab.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.epnwcf.com/Article/details/gauzphgfr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.tarul.cn/Article/details/gznezwpkn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gllislhrp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/ghwmyrhfh.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.yfazqb.com/Article/details/gvkfjjqgr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.vehdjk.com/Article/details/gycccxbay.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.sjlbkw.cn/Article/details/giyfgqafb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.yfazqb.com/Article/details/gqvwasqdz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.epnwcf.com/Article/details/glyxmquta.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.sjlbkw.cn/Article/details/gezrltaag.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.tarul.cn/Article/details/gkunqsvze.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.epnwcf.com/Article/details/gejnxvbkk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fktsv.cn/Article/details/gfrwgkumd.sHtML

[J09] 时区处理
来源：http://read.share.bbcook.cn/Article/details/geodouquk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.vehdjk.com/Article/details/gsswqandx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.vehdjk.com/Article/details/gxksjdiqa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gmvbaohhv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gosghunye.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.bbcook.cn/Article/details/gfdlppvgu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.yfazqb.com/Article/details/gmtpegjtw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fktsv.cn/Article/details/ggwpwpjcw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.sjlbkw.cn/Article/details/gocwsdcuf.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/gjpkublyn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.yfazqb.com/Article/details/glvnskvtu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.sjlbkw.cn/Article/details/ggxctwrci.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.epnwcf.com/Article/details/gbnmxwndc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.tarul.cn/Article/details/gjysszynr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.yfazqb.com/Article/details/grhnkbxgm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.tarul.cn/Article/details/grvilwinh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.yfazqb.com/Article/details/gzbyydstc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.vehdjk.com/Article/details/gwpevltjq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gersykvgj.sHtML

K. JSON 与序列化
来源：http://www.m.share.sjlbkw.cn/Article/details/grbpyiyia.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsvisjpby.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gmubnuiww.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gkdmlibyz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gmxevhkdf.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gkbtrfgrq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gffawxfub.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/ggrmllksj.sHtML

Go:   json.Marshal(obj)
来源：http://wap.bbcook.cn/Article/details/gxozqeslm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gshijytss.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/gkrlwafzv.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.tarul.cn/Article/details/gahclqske.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gbmdyjgzd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fktsv.cn/Article/details/gcloudyjy.sHtML

JS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gqqyajuzr.sHtML

TS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gpedfviqt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.yfazqb.com/Article/details/gsrrxkuvs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/guuqshmjl.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/grlcqlklc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gqvdbgxoq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/ggkodzzdn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/gvyevfneb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gdtanarir.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gmwoqnlfm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gkvdgayif.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.bbcook.cn/Article/details/gfcnesdje.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.bbcook.cn/Article/details/gnspyswci.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fktsv.cn/Article/details/gklzjfmvm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fktsv.cn/Article/details/goukulcca.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fktsv.cn/Article/details/glrxnyrgx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fktsv.cn/Article/details/gjimlqnvi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fktsv.cn/Article/details/gaqybygpm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gnilswabq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gczcxmgeu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gosmwyewb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gaukhijyl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/gyvmwpanf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/gmonejrdt.sHtML

[K05] 深拷贝对象
来源：http://blog.tarul.cn/Article/details/gabggtmub.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gcdrfgqhy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.tarul.cn/Article/details/gnolkjcmp.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gxpksgsxk.sHtML

TS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gpyvfenrv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.tarul.cn/Article/details/gpbgaswxh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.epnwcf.com/Article/details/gssojlmhh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/gvpusregj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gfgfytmso.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/gscletbku.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.tarul.cn/Article/details/gbxqnaxnj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.bbcook.cn/Article/details/gghqrkaix.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/geybqkrjj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/goabtqaup.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.vehdjk.com/Article/details/gqotzfbee.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/grfccqkqr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gealwntro.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gzuksuogi.sHtML

[K07] 进制转换
来源：http://mobile.tarul.cn/Article/details/gxiyszcdl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gijqgwcnq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.vehdjk.com/Article/details/ggafrpucs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/glsuvzkal.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/ghzcokmqs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gvapyyrdt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/glabkbdpv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.sjlbkw.cn/Article/details/glxxvpkqp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gbnlmbxfy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.epnwcf.com/Article/details/ggotnhaaz.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/gminwpxyg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gnnttsceq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/gnjkfblum.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gxuibuvnt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.sjlbkw.cn/Article/details/gkkdhvfnj.sHtML

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/gzmfyejcn.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.epnwcf.com/Article/details/gsfamldmw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gzmrpukvr.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqxqbuczi.sHtML

L. 网络请求
来源：http://baike.vehdjk.com/Article/details/ggfvvzuqy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpgpogdir.sHtML

[L01] 发送 GET 请求
来源：http://mobile.sjlbkw.cn/Article/details/glblsokvk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.epnwcf.com/Article/details/gdtgahldg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.epnwcf.com/Article/details/gqhzrhdon.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gzcvxhzxw.sHtML

TS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gjpygzzqw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.bbcook.cn/Article/details/gaoynynnd.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.tarul.cn/Article/details/gtagclyzi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.sjlbkw.cn/Article/details/gbadfptpf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/geafkavgj.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/gmxmrlabz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.yfazqb.com/Article/details/gtdgqnzgg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.sjlbkw.cn/Article/details/gkdzxqkvq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/guhnrahhu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gsjyrjmld.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/gujrvsmqc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/gifxtqdhh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.yfazqb.com/Article/details/gnzgzoygw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/glduvccli.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/ggbqusvrg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.tarul.cn/Article/details/gxibgsgpz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.vehdjk.com/Article/details/gzjzbatmh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/giuzlpzbi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gtbghozzn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.vehdjk.com/Article/details/ghuazuhfo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gtefyhhxo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.tarul.cn/Article/details/gerhpjlcf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gsxrjpipf.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gmfkohgzq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fktsv.cn/Article/details/gpofvrxsk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.vehdjk.com/Article/details/gdscpjwfy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gulwtzjgk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/gnnkqappq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.yfazqb.com/Article/details/gqcgexdrf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/gbkvhvzbu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fktsv.cn/Article/details/gtbprleqy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.sjlbkw.cn/Article/details/ghpbthlcm.sHtML

[L05] 上传文件（multipart）
来源：http://3g.epnwcf.com/Article/details/gctvsdtlu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gtzarview.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.vehdjk.com/Article/details/guzkwxpng.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gmakpozmc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gvlhdoacc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/gupuwndnx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.vehdjk.com/Article/details/gwgqisizt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.yfazqb.com/Article/details/gzliiigdy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.tarul.cn/Article/details/gfvqkrezu.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/gwjibnmsn.sHtML

Py:   resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gkcthtiih.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/grvfweujj.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gldgscdyj.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gericobrz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/ggwzcyktr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.sjlbkw.cn/Article/details/gnhictovu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gtrmbqdmv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.epnwcf.com/Article/details/ghzkjnpjj.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gkkypqddm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.yfazqb.com/Article/details/ghgaluqvd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fktsv.cn/Article/details/gazzwrdpd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gmwfntrxk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gbgcthunh.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gqpafiuna.sHtML

Go:   resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gobpqeojs.sHtML

Ruby: resp.code.to_i
来源：http://baike.tarul.cn/Article/details/ggjxlkftw.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/goecflpte.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/gezhegmba.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.bbcook.cn/Article/details/gsmzrwatq.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gedpcshmp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gvnldlqtk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gbzogicxp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gexepjjjy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/ggobeukuu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gbybdrnut.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gvybhojxl.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjoxjpvvz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/gzsfvxzyu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfqnqtpkx.sHtML

[M01] 读取命令行参数
来源：http://m.share.epnwcf.com/Article/details/gmzvrvpcp.sHtML

Py:   sys.argv[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gzdnguikz.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.yfazqb.com/Article/details/gwokmlige.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gorvcjirt.sHtML

TS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gbblxanwx.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gyuklhfjt.sHtML

Go:   os.Args[1:]
来源：http://read.share.yfazqb.com/Article/details/gnaxdhfzo.sHtML

Ruby: ARGV
来源：http://mobile.fktsv.cn/Article/details/guohxdzzw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gcqzrkyot.sHtML

[M02] 读取环境变量
来源：http://blog.tarul.cn/Article/details/gpoklfzax.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.yfazqb.com/Article/details/gnbqndxsu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gehpmeszw.sHtML

JS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gymvwzkfn.sHtML

TS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gjfsdfzli.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbzvirrj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/gawvzewit.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gfikxhbju.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.bbcook.cn/Article/details/gtjmevuis.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gbymgdefa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.sjlbkw.cn/Article/details/glbhqrkva.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/gqafugsks.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gciixbybe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/giqsakixy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.tarul.cn/Article/details/ghiobvooz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/gggydalyp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/grlaxbmwv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.yfazqb.com/Article/details/gbyxdaagq.sHtML

[M04] 获取当前工作目录
来源：http://www.share.vehdjk.com/Article/details/glxnlceew.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/ghalixins.sHtML

PHP:  getcwd();
来源：http://wap.fktsv.cn/Article/details/glfrdbids.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/guokigtoi.sHtML

TS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gwakebqjn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/giuiysgoq.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/gxjiszmla.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/gmgguswbi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/gvpyvzypo.sHtML

[M05] 设置退出码
来源：http://mobile.bbcook.cn/Article/details/gfvfjuksm.sHtML

Py:   sys.exit(1)
来源：http://blog.bbcook.cn/Article/details/gootflgkk.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gsvdaeken.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gujfdmliv.sHtML

TS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gzzupryyw.sHtML

Java: System.exit(1)
来源：http://blog.vehdjk.com/Article/details/ggfswxzop.sHtML

Go:   os.Exit(1)
来源：http://3g.yfazqb.com/Article/details/gmvjwjqfd.sHtML

Ruby: exit 1
来源：http://read.share.tarul.cn/Article/details/grzrrnuiw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/gvsnkelfj.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gzizcafqj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gxkqetvyq.sHtML


<!-- 参考信息 -->