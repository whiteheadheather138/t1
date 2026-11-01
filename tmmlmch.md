代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gyzmdqcxu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gzfusdnva.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gylrwdiew.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gdbepclzt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.bbcook.cn/Article/details/gnbgveujj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.tarul.cn/Article/details/ghwadtcsu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/gqpnyaklt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gytwtewir.sHtML

J. 日期与时间
来源：http://www.blog.tarul.cn/Article/details/glssexxxv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gsmgapxtb.sHtML

[J01] 获取当前时间
来源：http://baike.tarul.cn/Article/details/giqmuwski.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fktsv.cn/Article/details/gxxunigac.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/guxgqrjtu.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/glyttvqcf.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gsctqftmz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.tarul.cn/Article/details/gbytyojrw.sHtML

Go:   time.Now()
来源：http://3g.yfazqb.com/Article/details/gljuagrfb.sHtML

Ruby: Time.now
来源：http://3g.bbcook.cn/Article/details/gmeajvjin.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.epnwcf.com/Article/details/gfwucmfgv.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/gwvcvjhdj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/gblosnneb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fktsv.cn/Article/details/gwgwqqlng.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/gwxgoaiai.sHtML

TS:   d.toISOString()
来源：http://read.share.epnwcf.com/Article/details/gnrnozomi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.sjlbkw.cn/Article/details/gyvqqaurk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.epnwcf.com/Article/details/gfwnfknzx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gwvbpviho.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fktsv.cn/Article/details/gpcndhbdh.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fktsv.cn/Article/details/ghftlnwlc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/gyimsqxcm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.bbcook.cn/Article/details/gaesgeqbo.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gynaktqgy.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gqurbxouw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gxmzwbkss.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/giddymsjb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gvkaoxlmh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.bbcook.cn/Article/details/gtxbyztgc.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/gqfablkfj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.epnwcf.com/Article/details/ggxhlydrn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fktsv.cn/Article/details/gctwvqhaf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gzmlxiqwf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/gqlsrcfwy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gcfxmukns.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gbsxgkbip.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gptcepmua.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.epnwcf.com/Article/details/gluyzvvnt.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.bbcook.cn/Article/details/guhkepmph.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/gyjejauxm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/gtxtvxarq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gnedqcuwn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/ggybjeaqx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gxkhzfsnj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpywxoyvs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/gkxzayeda.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/gspxfaeoe.sHtML

[J06] 计算两时间之差
来源：http://m.share.sjlbkw.cn/Article/details/guxhtcero.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.sjlbkw.cn/Article/details/gblydtsdi.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.yfazqb.com/Article/details/gqrizvqix.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.bbcook.cn/Article/details/gkfphophe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fktsv.cn/Article/details/grvqsussm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.tarul.cn/Article/details/guopoqiqt.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fktsv.cn/Article/details/gdvrnpntb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.sjlbkw.cn/Article/details/glotujmxr.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.bbcook.cn/Article/details/gxctjcvfy.sHtML

[J07] 比较两个日期
来源：http://wap.yfazqb.com/Article/details/giylpbhry.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/glqngfavj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/gwworgyqs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fktsv.cn/Article/details/gdjrqtmfz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gkunylzqa.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.yfazqb.com/Article/details/glokvxwfh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fktsv.cn/Article/details/gumoebjva.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gmczxxpxp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gduzsypvp.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gocdqlauw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/glizmrskl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.tarul.cn/Article/details/gwdmycbfb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.epnwcf.com/Article/details/gpqzqdjti.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.epnwcf.com/Article/details/gkpasrlil.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.vehdjk.com/Article/details/geuyytfvq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.bbcook.cn/Article/details/gbxdsvjmu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.epnwcf.com/Article/details/gbirjmquf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fktsv.cn/Article/details/gdfbaxjpq.sHtML

[J09] 时区处理
来源：http://www.m.share.yfazqb.com/Article/details/gandolrsk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.sjlbkw.cn/Article/details/giuyzcimc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.tarul.cn/Article/details/ghimfxxaw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gnpylbtei.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gtecxwcjo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fktsv.cn/Article/details/gssdaxgaf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.tarul.cn/Article/details/gxxlreuzr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/gfsurssra.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.yfazqb.com/Article/details/glxisyrlc.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fktsv.cn/Article/details/gtkcznxqh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.epnwcf.com/Article/details/gprnghmdj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.yfazqb.com/Article/details/gfoeootat.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.yfazqb.com/Article/details/glpzxjshc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.vehdjk.com/Article/details/ghbqbkmoe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.sjlbkw.cn/Article/details/gknbxlesa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdmrnart.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.yfazqb.com/Article/details/gnpmyowsk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gjoqixgtp.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/grawscshe.sHtML

K. JSON 与序列化
来源：http://wap.yfazqb.com/Article/details/gshjlbaea.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gniqtbywd.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/ghlcsqtki.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gutdbvhec.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrkhgrvj.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/ghavnrmbp.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gruayakux.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.epnwcf.com/Article/details/gfuiodrnc.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gukfdspai.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.yfazqb.com/Article/details/gubemcpqi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gginerzps.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/gznenkpql.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/gfgjglarz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.yfazqb.com/Article/details/gpbhlzvyj.sHtML

JS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gikhypjcq.sHtML

TS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gfxiajwbw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gddkcysce.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/guuwxnlbn.sHtML

Ruby: JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/glphthvaz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fktsv.cn/Article/details/grwfdvrnc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.sjlbkw.cn/Article/details/gtrrbaeed.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/golqrnxpq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gqqvjpjqm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gdyjoryzz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/getppprfr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gpqgmmrov.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.yfazqb.com/Article/details/gljieayvk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.sjlbkw.cn/Article/details/gjjkpbdrs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.epnwcf.com/Article/details/gusqdmpic.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/gjjizxwwy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.vehdjk.com/Article/details/giceozayw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.yfazqb.com/Article/details/gtrmlulsn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gofvxaoxa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/glibrixhp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.epnwcf.com/Article/details/gcseobowl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gprezyoom.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.yfazqb.com/Article/details/gxzlseidz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gvtwadpmb.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/glkpieofs.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.epnwcf.com/Article/details/grsgfnslc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/gsjqwmvyo.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/glnepmnqo.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxtuqolw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.epnwcf.com/Article/details/gnetzutfj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fktsv.cn/Article/details/gmhkluofs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.sjlbkw.cn/Article/details/gmszserqy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.epnwcf.com/Article/details/gtdbvrwtz.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/gcmiwtqbq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.vehdjk.com/Article/details/gtjlykvjw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.epnwcf.com/Article/details/gxzizsmep.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gfbhaqfsy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gazfrxjdw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.sjlbkw.cn/Article/details/giutawemx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gxiakpgcg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/glftybswc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gecysfxhm.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/gjsknhtsh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gmkaqspjv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/gaaowgxbz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/giwovmyfu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/ggbskinwo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gmqfwthvw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fktsv.cn/Article/details/gjfmunpnx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.epnwcf.com/Article/details/gzrbsucwz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/grhbyuldh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.yfazqb.com/Article/details/gmvzxgcov.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gskfuiafu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.bbcook.cn/Article/details/grcptjmdc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwlnnuep.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/ghkqwbhqc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.vehdjk.com/Article/details/gxzimcznk.sHtML

Go:   encoding/gob
来源：http://www.share.bbcook.cn/Article/details/grodyjivs.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.yfazqb.com/Article/details/grircporu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gvcrrsbfs.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gllcilmpl.sHtML

L. 网络请求
来源：http://3g.vehdjk.com/Article/details/gvkrwmevg.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjqmszcfe.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fktsv.cn/Article/details/gdetfbosw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/ggpiupjnu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.tarul.cn/Article/details/gqrogzans.sHtML

JS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gophzbvzs.sHtML

TS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gplpjxjbx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.yfazqb.com/Article/details/gwygsszxd.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.epnwcf.com/Article/details/gimihstuz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/gvzebcfgx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.yfazqb.com/Article/details/gsaeiibtd.sHtML

[L02] 发送 POST JSON
来源：http://baike.vehdjk.com/Article/details/godnyorwh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gsskxdbtl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.bbcook.cn/Article/details/goewdijel.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gddhmpmzf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gnmilowgo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fktsv.cn/Article/details/gkyrgtega.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.yfazqb.com/Article/details/gtzbbcelq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.yfazqb.com/Article/details/ghbdhsxkw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.bbcook.cn/Article/details/geqpnlmyu.sHtML

[L03] 设置自定义请求头
来源：http://read.share.bbcook.cn/Article/details/gpcaroivp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.vehdjk.com/Article/details/gzvgjhihv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/gpiugocks.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gmjvcgsdo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/geaqhkpct.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/gjsmshinc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gigvzbnsb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.tarul.cn/Article/details/gnyxmdpjx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gbygtvccv.sHtML

[L04] 设置超时
来源：http://m.share.tarul.cn/Article/details/gffutzzux.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.vehdjk.com/Article/details/gezcwbigt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gcahvnvup.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gxjbbicjn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gmlhoulha.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.sjlbkw.cn/Article/details/genezixvh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.bbcook.cn/Article/details/gpugzxmzc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.sjlbkw.cn/Article/details/gvsacwqfo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.sjlbkw.cn/Article/details/grjpbulfu.sHtML

[L05] 上传文件（multipart）
来源：http://3g.yfazqb.com/Article/details/goflmipam.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/ghinexxpn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.yfazqb.com/Article/details/gixzwkylh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.tarul.cn/Article/details/gpjgkicxt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gyflajebx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gyhmttjlk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.sjlbkw.cn/Article/details/gsdazlima.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.epnwcf.com/Article/details/gzlnnvldo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gncqowtdy.sHtML

[L06] 解析响应为 JSON
来源：http://baike.epnwcf.com/Article/details/gnhswzrgl.sHtML

Py:   resp.json()
来源：http://mobile.epnwcf.com/Article/details/gqkwqhpov.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fktsv.cn/Article/details/geapkhame.sHtML

JS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gicyeoeji.sHtML

TS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gtwnqywcd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gfoowrrku.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.epnwcf.com/Article/details/gkyvdpoaw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.vehdjk.com/Article/details/gpzicuoks.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.epnwcf.com/Article/details/gshjlvnrn.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gbvhbrrzp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.epnwcf.com/Article/details/gdveuumzc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.bbcook.cn/Article/details/ghmfvncqs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gxgrkvnqa.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gahnzznrd.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gnjexfkcv.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/glehtpkfg.sHtML

Ruby: resp.code.to_i
来源：http://3g.sjlbkw.cn/Article/details/gyoampeyk.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fktsv.cn/Article/details/grvqahbkp.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gcktkdirq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.vehdjk.com/Article/details/gytxbjzof.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/guvnuhsyq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjdipyqt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gobllusjl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fktsv.cn/Article/details/gdhyruvkv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/grceupdvj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gsktpgnst.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.sjlbkw.cn/Article/details/gkzvssuoa.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggxvxnema.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.yfazqb.com/Article/details/gojsheniz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grhivhzwm.sHtML

[M01] 读取命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gnklzccfe.sHtML

Py:   sys.argv[1:]
来源：http://wap.yfazqb.com/Article/details/gfzgfeseo.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/guugmqrvq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gvugusaaz.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gtzkntqyq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gxdopmbij.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gjuhsjzai.sHtML

Ruby: ARGV
来源：http://read.share.tarul.cn/Article/details/gjhygedxc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gunnoqyvj.sHtML

[M02] 读取环境变量
来源：http://3g.vehdjk.com/Article/details/goagvydpt.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/gakhbmldr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gcyqqziqs.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gdibabmdf.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/ggbqouyqt.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gmztmwaxc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gweduzuzx.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/gkqevmktz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gsmjpaaiq.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/gqfhodyqv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.epnwcf.com/Article/details/gsihenxcm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fktsv.cn/Article/details/ginvqfntp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/ghvzhrfth.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gaviptcuw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.epnwcf.com/Article/details/gsepfslve.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.epnwcf.com/Article/details/ghduvllrl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.bbcook.cn/Article/details/gyvpfrvln.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gslauuhad.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/ggfwexxpr.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gdnycrxxa.sHtML

PHP:  getcwd();
来源：http://blog.sjlbkw.cn/Article/details/gmsakyttx.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/ggwwmqkgc.sHtML

TS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gozlqnmpq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.tarul.cn/Article/details/gkweaegma.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/giittvnwt.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/guwwoyhur.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gxwepzson.sHtML

[M05] 设置退出码
来源：http://www.m.share.sjlbkw.cn/Article/details/ggstxgsme.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/gqtravwbz.sHtML

PHP:  exit(1);
来源：http://read.share.yfazqb.com/Article/details/gyolucpbx.sHtML

JS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gngvnmyhk.sHtML

TS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/ggueefnhx.sHtML

Java: System.exit(1)
来源：http://baike.epnwcf.com/Article/details/gfktmhlpg.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gjljmrbwp.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/gpqrthdjb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/gyupdiift.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gxelxyjls.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gxzzzbxbb.sHtML


<!-- 参考信息 -->