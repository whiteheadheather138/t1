代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.epnwcf.com/Article/details/gtwucoeor.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gfzxbdyak.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gjhvdcpsw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gtlzztdfx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gzstwxqai.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.bbcook.cn/Article/details/glchgscbu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gqlnltnss.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.bbcook.cn/Article/details/gdzyjhsbn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.yfazqb.com/Article/details/gzgxtwkna.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gipjxzumz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.epnwcf.com/Article/details/gvvhlolpp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gpzdxhyrh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/groptraey.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gkdeezvaj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.epnwcf.com/Article/details/gucuvcdet.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.bbcook.cn/Article/details/gbyqeplgn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/geraicqqp.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.tarul.cn/Article/details/gfoardkje.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.tarul.cn/Article/details/grgqjscyk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/glolkfiti.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.tarul.cn/Article/details/ggygntsvs.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/geufudjmy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gblzuftgr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.epnwcf.com/Article/details/gklrhntsw.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.epnwcf.com/Article/details/gvhxyavdy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.tarul.cn/Article/details/gjbwfpbqo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.vehdjk.com/Article/details/gsqtnjifb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.vehdjk.com/Article/details/gvimlnpys.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/ghmcgjijy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/ggmihnjcc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gbjtzsdqd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/grmvhpppp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.vehdjk.com/Article/details/gjsrdlifa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.tarul.cn/Article/details/goywvxfoc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gaetnrgmk.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcmgefbuw.sHtML

J. 日期与时间
来源：http://3g.fktsv.cn/Article/details/gqrxzvfvq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpaiiiwis.sHtML

[J01] 获取当前时间
来源：http://wap.fktsv.cn/Article/details/gmljnnovn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.sjlbkw.cn/Article/details/gtdyquxfa.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/griryslvj.sHtML

JS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gjagatkot.sHtML

TS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gvgpvixns.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fktsv.cn/Article/details/gxbnubgni.sHtML

Go:   time.Now()
来源：http://www.blog.sjlbkw.cn/Article/details/gctorcsiv.sHtML

Ruby: Time.now
来源：http://3g.fktsv.cn/Article/details/gftqithac.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/goesphons.sHtML

[J02] 格式化输出
来源：http://read.share.fktsv.cn/Article/details/gkmuhjciu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/guzxdeirg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/gbyuzjbhy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fktsv.cn/Article/details/gerhfzaep.sHtML

TS:   d.toISOString()
来源：http://blog.epnwcf.com/Article/details/gbvrkpivc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.tarul.cn/Article/details/grcpuzkga.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.bbcook.cn/Article/details/gpdukgqdg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fktsv.cn/Article/details/ghwrebegf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.bbcook.cn/Article/details/gisvmrfyc.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fktsv.cn/Article/details/gsrfkwxme.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.tarul.cn/Article/details/ghcugqczq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.bbcook.cn/Article/details/gcghzhvzr.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gqlofakzn.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/glgmyqykq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gcspvuarr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/ggrilomiy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoarazhk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/guzesxpkj.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.tarul.cn/Article/details/geqtycvju.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fktsv.cn/Article/details/grgpgavhd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/guvacxdrs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fktsv.cn/Article/details/gxwjzedru.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gvcgjqkxk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.bbcook.cn/Article/details/gqrqfduws.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/gotofsumg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.tarul.cn/Article/details/gjxeyfhoe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gtrlljkio.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.vehdjk.com/Article/details/gmnvbfamq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.epnwcf.com/Article/details/gvbwjcynt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fktsv.cn/Article/details/gsjbrqzjt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/gmpgxuyvb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gsbdxksdz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.epnwcf.com/Article/details/ghhzlftgd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/gjqqwzhgz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.tarul.cn/Article/details/gflvgbaix.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gmaxbrlue.sHtML

[J06] 计算两时间之差
来源：http://blog.sjlbkw.cn/Article/details/gailidbsg.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.epnwcf.com/Article/details/gdztnvkcr.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fktsv.cn/Article/details/gqyfhczqp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.epnwcf.com/Article/details/gcwjhoacm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.bbcook.cn/Article/details/gbqfplybw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/gewqozyzt.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.bbcook.cn/Article/details/ggozwrfmq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/gxlolirqg.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/grdvxpkym.sHtML

[J07] 比较两个日期
来源：http://www.m.share.bbcook.cn/Article/details/gkkcbfuka.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gzefxzxdc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.epnwcf.com/Article/details/gqokkrvjy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gjsahplcg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/gbzujouey.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.vehdjk.com/Article/details/gudmorjoo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.sjlbkw.cn/Article/details/gnesyncih.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gmsfzwgrz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gadkrohms.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fktsv.cn/Article/details/gkuixyyfz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.sjlbkw.cn/Article/details/gpjhugcnf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.bbcook.cn/Article/details/gjiezbmog.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.sjlbkw.cn/Article/details/gentcmuwz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.epnwcf.com/Article/details/gowyqubwm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.vehdjk.com/Article/details/ggzmnquhs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fktsv.cn/Article/details/gckdlorhm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.vehdjk.com/Article/details/goktoybbk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.tarul.cn/Article/details/gohrffekx.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/geqpcwmeb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.yfazqb.com/Article/details/gcrggfbpb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.yfazqb.com/Article/details/gbdmjksmz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gzfttsozp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gbbnulzgf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/ggdgulvmd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.yfazqb.com/Article/details/gsijklqov.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/gypznojzx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.vehdjk.com/Article/details/gzkkbtnmt.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.bbcook.cn/Article/details/gvndzzpxm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.bbcook.cn/Article/details/glvlthwlz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.yfazqb.com/Article/details/gcwycgief.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.yfazqb.com/Article/details/gupasezst.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.epnwcf.com/Article/details/gciabueak.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.tarul.cn/Article/details/gplwydqoz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gyfhpcala.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.vehdjk.com/Article/details/goxhrqrbz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fktsv.cn/Article/details/gawltnwfd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcsagqujj.sHtML

K. JSON 与序列化
来源：http://3g.vehdjk.com/Article/details/girrpvyyv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdqmnkpms.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gbeeyenld.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gbffrwuqy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/gpsjfupsj.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gperqufih.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gyimnanea.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.vehdjk.com/Article/details/ggrzwgqkw.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/gfunrlopl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.bbcook.cn/Article/details/gcnugzyxd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.bbcook.cn/Article/details/gfibyduzo.sHtML

[K02] JSON 字符串转对象
来源：http://3g.vehdjk.com/Article/details/gxpnfnoee.sHtML

Py:   json.loads(s)
来源：http://www.share.sjlbkw.cn/Article/details/gdozfuftl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.tarul.cn/Article/details/gflsjvqff.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/guhojahvu.sHtML

TS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gvbeuosem.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.vehdjk.com/Article/details/gfswobteo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gltjwwdgx.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gjywzbslp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.bbcook.cn/Article/details/giqcvgvzy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/gmzdsyvja.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/golyhdrtl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gjogeqbcb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/grjzrtjcv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gkeqzvmcu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gxpdxklax.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.bbcook.cn/Article/details/gwevqlcno.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.tarul.cn/Article/details/gtmghhxyf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.sjlbkw.cn/Article/details/gtuwftqyj.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/gnwbvoxxc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.yfazqb.com/Article/details/gjuskbwam.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.epnwcf.com/Article/details/gvijeedap.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gpeclbcil.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/gpcnoexxz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gsrdmkoaq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gnelfreuv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/gdjinpecv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.bbcook.cn/Article/details/grtzfbwom.sHtML

[K05] 深拷贝对象
来源：http://www.share.vehdjk.com/Article/details/gfgkdluoi.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.vehdjk.com/Article/details/ggyecgiej.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/glzusemyx.sHtML

JS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gcxmkvukv.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gvaymutjh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/gmdhtynir.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.yfazqb.com/Article/details/gxmuuubeg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gpldpmkqf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gzurclour.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.yfazqb.com/Article/details/gggerwkff.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.yfazqb.com/Article/details/giaoypwmt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fktsv.cn/Article/details/gjqfvepny.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gjukzqgzs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/gryoqeenq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.vehdjk.com/Article/details/gttpxjkld.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gueeiwofj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gvgxdkufv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gwabjxvka.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gseuychdt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gwmbtuzgu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fktsv.cn/Article/details/giforwwam.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gqxrjdtbi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/ggbeiynpz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gfsdbsxeh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/gwuorexeh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.epnwcf.com/Article/details/gganywfgp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gznuxzwon.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.yfazqb.com/Article/details/gkhlswkvb.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gvrgnabpa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.vehdjk.com/Article/details/gbmlzazuj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/ghkuhsmpv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gafzgqsba.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.yfazqb.com/Article/details/gidnikngo.sHtML

Go:   encoding/gob
来源：http://read.share.tarul.cn/Article/details/gencxmfxv.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.tarul.cn/Article/details/gytjdnygg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gefsvanoq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gwdhsutkk.sHtML

L. 网络请求
来源：http://blog.bbcook.cn/Article/details/gobwdomhj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gaykfemim.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/geylcjrhn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.epnwcf.com/Article/details/griibtdnn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.sjlbkw.cn/Article/details/gowstlksh.sHtML

JS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gipzeqlzv.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/ggpnatrjl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gvolrnyoz.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.epnwcf.com/Article/details/gopcqjkhl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fktsv.cn/Article/details/gwcjuxlpc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/godvevirz.sHtML

[L02] 发送 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gzyreyicy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/goghwnmbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.vehdjk.com/Article/details/gfyjdwdgw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gtqdojxvc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gfjbkvihj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.epnwcf.com/Article/details/gpjkzpbay.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gqgopzvoi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.sjlbkw.cn/Article/details/gyrwlmyzj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.bbcook.cn/Article/details/gczvqiqvk.sHtML

[L03] 设置自定义请求头
来源：http://3g.fktsv.cn/Article/details/gbzmqgmmj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.epnwcf.com/Article/details/gofsjusnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.yfazqb.com/Article/details/gqstxhrtg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/gjnadwyec.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gqvaomeik.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/ghkksqtmb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/geyqdyeco.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.sjlbkw.cn/Article/details/gyiymdrte.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gtlcgaocl.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/glytuarmn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.bbcook.cn/Article/details/gcbyvaprz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/ggxfapoik.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gjiuldkdq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gebzfkkgr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fktsv.cn/Article/details/gycyyxfav.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/gppugvtmu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fktsv.cn/Article/details/geinkqomn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fktsv.cn/Article/details/gsnyjagos.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/gamtrxsiq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.epnwcf.com/Article/details/ghnvkkfas.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.sjlbkw.cn/Article/details/gbhkdgnjf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gpgpvscad.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gfgvbycbb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gcqpyqmwm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/glsdwoizz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.epnwcf.com/Article/details/gvwsefdnj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/gjolernhz.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gbzyanyiw.sHtML

Py:   resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gmqkikotl.sHtML

PHP:  json_decode($body, true);
来源：http://blog.sjlbkw.cn/Article/details/gpxyakeuf.sHtML

JS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gtpjrtmqf.sHtML

TS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gzenajqfg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.yfazqb.com/Article/details/gfekevfdp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfduvztly.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.tarul.cn/Article/details/gozqlyowv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnjyosvl.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gvjzrbrmj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.vehdjk.com/Article/details/gesqbujdk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.epnwcf.com/Article/details/goqaskmgk.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/gtyzrquqk.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gvdvptfqd.sHtML

Java: resp.statusCode()
来源：http://baike.tarul.cn/Article/details/gzvckawsh.sHtML

Go:   resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gxkukubxe.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.tarul.cn/Article/details/gwzuruoya.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gtlfzjrcl.sHtML

[L08] 并发请求多个地址
来源：http://wap.vehdjk.com/Article/details/gpcfxjiwn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.epnwcf.com/Article/details/grvdrwahr.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.sjlbkw.cn/Article/details/grzpsihql.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gvktybeim.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gvgnjevft.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.yfazqb.com/Article/details/ghjhmrcac.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.epnwcf.com/Article/details/giwivtcll.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.yfazqb.com/Article/details/gpbevndql.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fktsv.cn/Article/details/gcdupnzdl.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmbtmxams.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.sjlbkw.cn/Article/details/gpngsiuik.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzfhrobez.sHtML

[M01] 读取命令行参数
来源：http://www.share.bbcook.cn/Article/details/ggecfquqh.sHtML

Py:   sys.argv[1:]
来源：http://3g.bbcook.cn/Article/details/gqioyggps.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fktsv.cn/Article/details/gqruqpbfk.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/guwcrpgcs.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gomxatdbs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/grtcpgwra.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdredgul.sHtML

Ruby: ARGV
来源：http://www.blog.epnwcf.com/Article/details/gzjlbjnpp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gikjwfxzc.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gohqkzpsa.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fktsv.cn/Article/details/gtxravlno.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gvhqmkmxu.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gwcixynsq.sHtML

TS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/glmrtqtjg.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/gojnroxwi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gwhtdbsfn.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gcjhxqxdf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gopwtjqyx.sHtML

[M03] 执行外部命令
来源：http://mobile.yfazqb.com/Article/details/gzmdvqzwu.sHtML


<!-- 参考信息 -->