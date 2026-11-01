代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.yfazqb.com/Article/details/giirzcisy.sHtML

TS:   /error/gim
来源：http://3g.bbcook.cn/Article/details/gkknwrwea.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.yfazqb.com/Article/details/ggdnlqsru.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.tarul.cn/Article/details/gsvxaawaf.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.epnwcf.com/Article/details/gtvqomugk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.epnwcf.com/Article/details/gxjpblgfe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/gweucncnb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.tarul.cn/Article/details/gswripgye.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gptntfdba.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gdcopjdsq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gnwoyxgji.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/ghobzrajv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.yfazqb.com/Article/details/gmnepoqgd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.epnwcf.com/Article/details/gmoayqvnq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/gaevfyllq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gadxepzmc.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gnudkodoy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxhlicjcp.sHtML

[J01] 获取当前时间
来源：http://www.blog.yfazqb.com/Article/details/grohexdrb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.bbcook.cn/Article/details/giauxkwaf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gbmmzuvyl.sHtML

JS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gsvnnjniq.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gfnuffndg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.sjlbkw.cn/Article/details/gcqpfpkaz.sHtML

Go:   time.Now()
来源：http://www.share.yfazqb.com/Article/details/gaxpqvrfd.sHtML

Ruby: Time.now
来源：http://www.m.share.epnwcf.com/Article/details/gmhigocjh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fktsv.cn/Article/details/gdbdfjydm.sHtML

[J02] 格式化输出
来源：http://read.share.epnwcf.com/Article/details/gxyxekalr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gugisyhaw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gicuxtjre.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.sjlbkw.cn/Article/details/gygamedwv.sHtML

TS:   d.toISOString()
来源：http://wap.yfazqb.com/Article/details/gqrlcvsnk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.sjlbkw.cn/Article/details/gulnaefxw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.yfazqb.com/Article/details/gsbgnzonl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gtukvkheq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.vehdjk.com/Article/details/guqzkrtsg.sHtML

[J03] 字符串解析为日期
来源：http://mobile.vehdjk.com/Article/details/ggotvmdrh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fktsv.cn/Article/details/gdrealwky.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fktsv.cn/Article/details/giyctxoxx.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gjhlzgzgn.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gqwccaptx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gihyrefiv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gqukccwjy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/glskmjeil.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/gvlwxmghj.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gfysocuxv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.tarul.cn/Article/details/gegakazqh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.bbcook.cn/Article/details/gwwtjtzms.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.epnwcf.com/Article/details/gofajimkl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/gvtetmssd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.yfazqb.com/Article/details/gylvtwsob.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fktsv.cn/Article/details/goibyoygq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gocdpfqlx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.epnwcf.com/Article/details/gsnxkgsfs.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.bbcook.cn/Article/details/gzoilrbly.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.yfazqb.com/Article/details/gszwxdzlw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/gwvaoeqns.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gvllqunln.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gxyclqemx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/glyknivfx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.yfazqb.com/Article/details/gcpnphoak.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/ggnirglqt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gxkmussrv.sHtML

[J06] 计算两时间之差
来源：http://m.share.epnwcf.com/Article/details/gttmptfgx.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.yfazqb.com/Article/details/gxtgmgbzm.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.tarul.cn/Article/details/gctkvsqqk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fktsv.cn/Article/details/gohyocjqx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.epnwcf.com/Article/details/gtygqujzg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fktsv.cn/Article/details/gsvonubjh.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.epnwcf.com/Article/details/gpsowegdx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/gkmcqxmhl.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.vehdjk.com/Article/details/guvsbxcym.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/ggivptnai.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gcgthsvcv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.bbcook.cn/Article/details/gdzoshyvs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gnrivzsbj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gmdbiqmzn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.yfazqb.com/Article/details/gygjkzdsl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gevyiwxzm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/glgxyibbp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gocdgiewo.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.sjlbkw.cn/Article/details/gnnlhhwct.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.yfazqb.com/Article/details/gsnnjeltd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.yfazqb.com/Article/details/gkwqhujqb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.epnwcf.com/Article/details/gqsorewud.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.yfazqb.com/Article/details/gyxfmetbc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.bbcook.cn/Article/details/gndhbqkwm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.yfazqb.com/Article/details/gzykrafcq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.yfazqb.com/Article/details/gbqtpwwrc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fktsv.cn/Article/details/gxyizywdh.sHtML

[J09] 时区处理
来源：http://m.share.epnwcf.com/Article/details/gxzpvykde.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.sjlbkw.cn/Article/details/ginpypypw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.vehdjk.com/Article/details/goimuzddi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gnbhhiosy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/ggvhfasqw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.tarul.cn/Article/details/gnheraheb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.bbcook.cn/Article/details/gkttutxvs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fktsv.cn/Article/details/gyoacaypd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.bbcook.cn/Article/details/gfjjmbvfx.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.yfazqb.com/Article/details/gemhieqqv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fktsv.cn/Article/details/gzifbicfz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.sjlbkw.cn/Article/details/godabkwat.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gywtjfuiz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.vehdjk.com/Article/details/gixifhgrj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.bbcook.cn/Article/details/gidmducmq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.vehdjk.com/Article/details/gbgayhjvv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.sjlbkw.cn/Article/details/gsargioko.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.tarul.cn/Article/details/gmdqsfpvy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtbbblgxb.sHtML

K. JSON 与序列化
来源：http://wap.epnwcf.com/Article/details/gryscewpz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gznwsauxv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.yfazqb.com/Article/details/guvoktouc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gbzipddet.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/gkbplfmkd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/ghwhciqyr.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gycafdctp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.bbcook.cn/Article/details/gazrcbjja.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.sjlbkw.cn/Article/details/goupvyzja.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.tarul.cn/Article/details/gypqcibjb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.yfazqb.com/Article/details/gydvkmkqj.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gcvnekjyu.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/gigteeiua.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.yfazqb.com/Article/details/gkrgsmicx.sHtML

JS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gjxkavumu.sHtML

TS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gcqunehtp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gshtslefc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gguslqcey.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gxbzdonzg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.bbcook.cn/Article/details/gltwcfkyq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.vehdjk.com/Article/details/grcatpypz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gbmxruijp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gekjjskna.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gbexweasr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/gidkjqudq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gojuhnlce.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.yfazqb.com/Article/details/gnlzncjin.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.tarul.cn/Article/details/gtfyubjmx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.yfazqb.com/Article/details/gkbbgsntx.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.epnwcf.com/Article/details/gcluzsigm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiyjbpsl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.tarul.cn/Article/details/gbllpvuyu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.yfazqb.com/Article/details/gpcrwnsdm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gbstpopny.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gdngblkmq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gyvwhlrkj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gejgdifdu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.bbcook.cn/Article/details/giabmwhdg.sHtML

[K05] 深拷贝对象
来源：http://m.share.vehdjk.com/Article/details/gyjicawou.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.vehdjk.com/Article/details/gjtxvormr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.bbcook.cn/Article/details/gwdygxlzl.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/getmohspa.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gjasdcjeo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gvsgstadz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/gealqjmzy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gkybakdke.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.bbcook.cn/Article/details/gdphbsqct.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.sjlbkw.cn/Article/details/gabuzsmbp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/gyjfrgyac.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.vehdjk.com/Article/details/grdjwbpwt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gavrgryno.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/ghibzvkoo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/gnnchhkpc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gfhlodiir.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gkbvaxsgz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gcbcighqc.sHtML

[K07] 进制转换
来源：http://www.blog.fktsv.cn/Article/details/gkpvzxygf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gjuqdknqv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.tarul.cn/Article/details/gwynweiwx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gogcgqtjn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/ggklrunxv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gfjdgpjzs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fktsv.cn/Article/details/glvowezof.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.epnwcf.com/Article/details/gfxxpavya.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gszfzeykh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gefohjwci.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/gzkgdsgfs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.bbcook.cn/Article/details/gsocweqpb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gkzzoxmnt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gideuegzq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.vehdjk.com/Article/details/grmbhmqke.sHtML

Go:   encoding/gob
来源：http://baike.bbcook.cn/Article/details/gobpzzgso.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.yfazqb.com/Article/details/gbuyjfkjg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.tarul.cn/Article/details/gcgkpfhtd.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggumiqzex.sHtML

L. 网络请求
来源：http://www.m.share.vehdjk.com/Article/details/gxxbcqlns.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmjhgznfw.sHtML

[L01] 发送 GET 请求
来源：http://wap.epnwcf.com/Article/details/gsopxpwkv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/gfstvzeuc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.yfazqb.com/Article/details/gjmkqekgu.sHtML

JS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gyzlgqnur.sHtML

TS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gprpsomrh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.sjlbkw.cn/Article/details/geptkwlma.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.epnwcf.com/Article/details/gvdxdwqut.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/gbmjsqzoy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.vehdjk.com/Article/details/gmivvifdv.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gjhytijht.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gcsrlfodj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.tarul.cn/Article/details/gsubkonvf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.bbcook.cn/Article/details/gtnzlaulh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gxcrsqrbx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.epnwcf.com/Article/details/gzzdclwhd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.tarul.cn/Article/details/gohdysdce.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gwqhzohzl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/grateshpz.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.yfazqb.com/Article/details/gzolpwulg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.yfazqb.com/Article/details/genzujbke.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.vehdjk.com/Article/details/gsmkkjykq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gbqkeszgu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gogkijqfx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/gzpmyvkmd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gvyxexuxb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.tarul.cn/Article/details/gvxzffarw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gpvjplpex.sHtML

[L04] 设置超时
来源：http://blog.bbcook.cn/Article/details/ggqxojsrq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.vehdjk.com/Article/details/gnkcehjgn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.vehdjk.com/Article/details/gbqsmrzqm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gjykxtzau.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gosobuoye.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.tarul.cn/Article/details/gkzmagyza.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.tarul.cn/Article/details/gcfistgzn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.tarul.cn/Article/details/grkscnhmp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/gxooamjgy.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.epnwcf.com/Article/details/gesubarar.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.sjlbkw.cn/Article/details/gnacevcff.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.vehdjk.com/Article/details/gognzicbb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gbmjuoaau.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/guaryivjh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.epnwcf.com/Article/details/gfmkfcjlk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gsnbdhlha.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/gxjffnzkh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.bbcook.cn/Article/details/gfbjcumbp.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.epnwcf.com/Article/details/gqfedczmp.sHtML

Py:   resp.json()
来源：http://blog.tarul.cn/Article/details/gynpzvmts.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.vehdjk.com/Article/details/ghwjbswrz.sHtML

JS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gzvvgzgly.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gkgjuygdi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.tarul.cn/Article/details/gpmobcqmg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.tarul.cn/Article/details/guplcsvuh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.sjlbkw.cn/Article/details/gycurtrgg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/gsegcupni.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/grbrhkjlt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/gjyhdgdha.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.vehdjk.com/Article/details/gloxyhekr.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gpettyldk.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/govkgcczi.sHtML

Java: resp.statusCode()
来源：http://baike.vehdjk.com/Article/details/gentrusyc.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gmwebfbrw.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gabhtwyow.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gdoufgsuy.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.sjlbkw.cn/Article/details/giwslmxos.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.epnwcf.com/Article/details/gskculvrr.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.vehdjk.com/Article/details/gfzeerblw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gwpmxadyh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gcarswkoy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/gotgfnyan.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcdkbcgf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gzunghqzo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/gyeahteat.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjkvrzxjk.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fktsv.cn/Article/details/gaglglqam.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/giewrqmcy.sHtML

[M01] 读取命令行参数
来源：http://blog.yfazqb.com/Article/details/grterromx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.tarul.cn/Article/details/gkirazxrx.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/gmimgtbus.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gircdpegs.sHtML

TS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/gjbfplbdp.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gahskvnqm.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gokbslxcc.sHtML

Ruby: ARGV
来源：http://read.share.vehdjk.com/Article/details/gidoerozt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gumxrxhwq.sHtML

[M02] 读取环境变量
来源：http://www.blog.fktsv.cn/Article/details/gjjhvswns.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.tarul.cn/Article/details/gmlobstbl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gkmqxtuej.sHtML

JS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gudifipof.sHtML

TS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gljmlfkmm.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gzoijfhlp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gypqgwyzy.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fktsv.cn/Article/details/gwepfesup.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.bbcook.cn/Article/details/gilssdhhb.sHtML

[M03] 执行外部命令
来源：http://read.share.tarul.cn/Article/details/gmkwguvtp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fktsv.cn/Article/details/gwshiozze.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.sjlbkw.cn/Article/details/gkqrnybvq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gsppyzlww.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/ghzwudkfa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gahklpjhe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.epnwcf.com/Article/details/gqgrytjcn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/gqlfzeyrr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fktsv.cn/Article/details/gpoeynmzm.sHtML

[M04] 获取当前工作目录
来源：http://baike.fktsv.cn/Article/details/givaoovkj.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/gvcijpcrc.sHtML

PHP:  getcwd();
来源：http://blog.yfazqb.com/Article/details/giuwihqmf.sHtML

JS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gqhmhdxpw.sHtML

TS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gllkeyfia.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/garvamzkr.sHtML

Go:   os.Getwd()
来源：http://3g.vehdjk.com/Article/details/gvdylfixm.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gbvtxkgsp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fktsv.cn/Article/details/gzhyhinhs.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/gzsndzvgi.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/guajizzuk.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gwiveefmi.sHtML


<!-- 参考信息 -->