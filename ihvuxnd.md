代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.sjlbkw.cn/Article/details/gkzwpouyy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.tarul.cn/Article/details/gfmhqtmlm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/glfrjabyd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gykhhbclp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.epnwcf.com/Article/details/gzudyhaij.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gicpjafbo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gbzgxrhww.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.bbcook.cn/Article/details/glbmfnuph.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.epnwcf.com/Article/details/gwnojvlsi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gtgdonkok.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.sjlbkw.cn/Article/details/ggxfdchds.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gfflrivbp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gbbrmplml.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gunvrunwz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.bbcook.cn/Article/details/gomclpkgj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.sjlbkw.cn/Article/details/gzuwajzpx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/glwvlhghb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.sjlbkw.cn/Article/details/ggekrofnx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.bbcook.cn/Article/details/gmfxqihwv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gqsumxxkx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/gyxucshsq.sHtML

TS:   /error/gim
来源：http://wap.sjlbkw.cn/Article/details/gvtnooiii.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fktsv.cn/Article/details/gmayqjciy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.yfazqb.com/Article/details/gknjjhrrk.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.yfazqb.com/Article/details/gyfntgghe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.epnwcf.com/Article/details/gvkwwabne.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/gpwjchsrz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.tarul.cn/Article/details/gtnuhbdtk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gsoclxoce.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/ggfobpdvz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gkjoymjbt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/gdosdnyqm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.bbcook.cn/Article/details/gvjjyirph.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.bbcook.cn/Article/details/gkssdzjkr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/geeuiarqf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxyxineth.sHtML

J. 日期与时间
来源：http://baike.sjlbkw.cn/Article/details/gowsygpmw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmwwzmcnn.sHtML

[J01] 获取当前时间
来源：http://baike.bbcook.cn/Article/details/gavwygbpn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/ggrsyxnyd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/giqnxbmaj.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gsmydjzik.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gfkpxixlq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/ganjogxba.sHtML

Go:   time.Now()
来源：http://mobile.vehdjk.com/Article/details/ghvakstsf.sHtML

Ruby: Time.now
来源：http://www.blog.bbcook.cn/Article/details/gqfpltvsf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.vehdjk.com/Article/details/grixyfpsm.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/goxnvzfwm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gaygvboxr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/giiafuvsq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.sjlbkw.cn/Article/details/gxhkgxdwy.sHtML

TS:   d.toISOString()
来源：http://www.share.yfazqb.com/Article/details/grdjtmgre.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/gdcmuotxx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/gzezzplvx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gwnrwahnk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/gnvoqvcbw.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/glijacfcp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.tarul.cn/Article/details/gmnxqhtvn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.vehdjk.com/Article/details/gsjnidljy.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gvdpabtcq.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/glbvfmlza.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gschhsjot.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gkgmhwndv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gekbczjeg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fktsv.cn/Article/details/gtjxpvxem.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.bbcook.cn/Article/details/gnzfllnuw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.vehdjk.com/Article/details/gaaqyxbuw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/gaqbdkcms.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.vehdjk.com/Article/details/gkbuqlyyj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.epnwcf.com/Article/details/gsvliowwd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.tarul.cn/Article/details/gyiqyjkzl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.vehdjk.com/Article/details/gcmgzrwcj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.sjlbkw.cn/Article/details/gskdfpspi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/gifgslcjq.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.sjlbkw.cn/Article/details/gkxkeftwz.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.vehdjk.com/Article/details/gigfiuahg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fktsv.cn/Article/details/gaxxlnzsh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/ggdcfmffh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/grmhdpeou.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gkxnzmqnx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/gkuoxqimc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fktsv.cn/Article/details/gtbycjrrj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/gifcwbryl.sHtML

[J06] 计算两时间之差
来源：http://wap.yfazqb.com/Article/details/gscrgpdwn.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.bbcook.cn/Article/details/gunqxqbfp.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.yfazqb.com/Article/details/gygpfufrv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.sjlbkw.cn/Article/details/gdcapxuyp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.bbcook.cn/Article/details/gyibcfmtc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/guvquostm.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.tarul.cn/Article/details/gynmqltsk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.bbcook.cn/Article/details/gcwuabxsa.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/gzjzcmwap.sHtML

[J07] 比较两个日期
来源：http://wap.fktsv.cn/Article/details/gfjyjnoos.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gsacardxv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.bbcook.cn/Article/details/gwumwcpfb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/ggchcbidx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/gswihhadv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.yfazqb.com/Article/details/gagohclqq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.yfazqb.com/Article/details/ggseyjtaw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gmunbuoda.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/ghyitsurs.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/ggmcluzka.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/gbnhnqvqw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/gsspkjkbu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.tarul.cn/Article/details/gtgqhisvc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fktsv.cn/Article/details/gqauxgghx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/gkorxgsyt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.yfazqb.com/Article/details/gepqqxlsh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fktsv.cn/Article/details/guycxhhzc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/gsumznftz.sHtML

[J09] 时区处理
来源：http://www.share.tarul.cn/Article/details/gpewzybrb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.yfazqb.com/Article/details/grgfvfxsx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.bbcook.cn/Article/details/ghjdriyaf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gdwmafsgl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/ghdpmqwqc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.vehdjk.com/Article/details/gqwvzhtkc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fktsv.cn/Article/details/grarywfhc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.bbcook.cn/Article/details/geotbnghp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.bbcook.cn/Article/details/gokgotosg.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.tarul.cn/Article/details/gowpozlaa.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gxfnuyyfd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.bbcook.cn/Article/details/ghjyixzam.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fktsv.cn/Article/details/gikzeqlcf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.bbcook.cn/Article/details/gvduipyja.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.bbcook.cn/Article/details/gdvhzoqwp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.vehdjk.com/Article/details/galblmkyl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.sjlbkw.cn/Article/details/gcmuxubrb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.epnwcf.com/Article/details/gwfbctqeo.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gooajfoma.sHtML

K. JSON 与序列化
来源：http://www.m.share.fktsv.cn/Article/details/gmirrrcqr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gndiuihkg.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.epnwcf.com/Article/details/gyqmfkxbg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/giecwehsi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/gjogvngkw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gnrrmctdq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gffddtrhu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.yfazqb.com/Article/details/gatpyisdm.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/gckrvbzgj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gifxrinaw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.yfazqb.com/Article/details/ghhalwouw.sHtML

[K02] JSON 字符串转对象
来源：http://wap.bbcook.cn/Article/details/govhryprq.sHtML

Py:   json.loads(s)
来源：http://mobile.tarul.cn/Article/details/gwoanfolh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.yfazqb.com/Article/details/gldsosabd.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gsrkzefyn.sHtML

TS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gbpvckzya.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gwmdkkbok.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.epnwcf.com/Article/details/gwevfojqy.sHtML

Ruby: JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gugkwzcfp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.vehdjk.com/Article/details/giqkcrnrx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.tarul.cn/Article/details/gqykjfmti.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gcmrihbms.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gjpdevrrw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gtaarpftc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gleangpom.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.epnwcf.com/Article/details/gknnlnnsc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/gnnjfoxir.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.sjlbkw.cn/Article/details/glddxlpbh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.sjlbkw.cn/Article/details/grgruebwq.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.vehdjk.com/Article/details/gmbqwtvbb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.bbcook.cn/Article/details/gdrfbdatz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.sjlbkw.cn/Article/details/gjzwzbimk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gsfnuapia.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/glvguvkrr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gxaoejsnl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gpufgghix.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gqnkpyuto.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.yfazqb.com/Article/details/grbbvmrur.sHtML

[K05] 深拷贝对象
来源：http://m.share.fktsv.cn/Article/details/gaemqgcvx.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fktsv.cn/Article/details/gqixblyjo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gvukbkdsw.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gpivwtonw.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gewyuqvpc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.tarul.cn/Article/details/gdaqlinvv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gsjgbadej.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gzgivlmoo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.epnwcf.com/Article/details/grdevjmck.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/gaxtfcgfn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.epnwcf.com/Article/details/gsqzosyxq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.tarul.cn/Article/details/gcugnqwjk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/ghgpljmsz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/groocpzbz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.epnwcf.com/Article/details/gafzjaung.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gedsthngu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gxiwqvmng.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gvszhkyka.sHtML

[K07] 进制转换
来源：http://3g.yfazqb.com/Article/details/gpvwawujs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gsraerpbp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gdzipewnf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gachfnktk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gosxzhrdu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/geuuvtsbz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.vehdjk.com/Article/details/glxungllc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gionlqtsx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gynmhkhdf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.vehdjk.com/Article/details/gsznrcwoa.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/gedcjynrs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.yfazqb.com/Article/details/gcskltjpu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gtmmbjore.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gsxcfpiou.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.tarul.cn/Article/details/gwxriaxlw.sHtML

Go:   encoding/gob
来源：http://wap.tarul.cn/Article/details/gyczfjpnn.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.epnwcf.com/Article/details/gjostpoyf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gjhroifom.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gszatmbpa.sHtML

L. 网络请求
来源：http://www.share.sjlbkw.cn/Article/details/gikhevusi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gsgziyljn.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.sjlbkw.cn/Article/details/geflnevos.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.vehdjk.com/Article/details/geggrzqhs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.tarul.cn/Article/details/groxmakwt.sHtML

JS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gnvedepgi.sHtML

TS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gixjhrlxr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gqtfqndfa.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gncctovaj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.tarul.cn/Article/details/gocobjfpm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.tarul.cn/Article/details/gxcymqxbg.sHtML

[L02] 发送 POST JSON
来源：http://www.share.yfazqb.com/Article/details/gxfupmbfy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gylbaekrm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.tarul.cn/Article/details/gljvqyuly.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gfuimlzfg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/ghnklfcvx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.yfazqb.com/Article/details/gabktinkg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/guenlbtza.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.epnwcf.com/Article/details/gredtlggy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/gyibgeozg.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/gkndbfhkd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.sjlbkw.cn/Article/details/gulihzalb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.epnwcf.com/Article/details/gklcelvxd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gggufonrx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gdhenaggt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.tarul.cn/Article/details/ghxdxfivu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gpnhbzvej.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/gycdjncmv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gzadtkpmo.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/gmbzvvdmg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.vehdjk.com/Article/details/gpjyjrknn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/ggqpndsly.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gdwoawihb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/giczmbwyu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.epnwcf.com/Article/details/ghrxywclb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gvxjdnyer.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/gwqirhdqm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.yfazqb.com/Article/details/gpbqucwxv.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fktsv.cn/Article/details/gurjtgsxm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.epnwcf.com/Article/details/gypgcwzvv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.bbcook.cn/Article/details/gjyxlnskk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/ghnkoaiso.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gjvvebwhf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/gzeazntdu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.sjlbkw.cn/Article/details/gushcolie.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.sjlbkw.cn/Article/details/gjqyxdpep.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.vehdjk.com/Article/details/gmpuznewl.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gtnqgrqgc.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/grauefvxa.sHtML

PHP:  json_decode($body, true);
来源：http://3g.tarul.cn/Article/details/giolfavud.sHtML

JS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/glpzsthhb.sHtML

TS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gfltqfmhh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gktdamsni.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fktsv.cn/Article/details/gxrzusxwk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.tarul.cn/Article/details/genmhhrzj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gjyngoppt.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/ggsaqzuwh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fktsv.cn/Article/details/gvswdaldq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/gcouhjubu.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gwnrehthl.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gjwnzoyvb.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/gichuhrwg.sHtML

Go:   resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gkjhehhst.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fktsv.cn/Article/details/gmsdgcfxb.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gngtywffy.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gjexjkwli.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gayxwercp.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/gslcdcmhp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gdfogwntz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gtlccuzyz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/gojmrszav.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/gxuytbiet.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gccebhsaa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/glypuayyy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdxyumdmk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.bbcook.cn/Article/details/gpycouagj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gbktjrzrp.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gpzlpwopf.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/gvzjcznzb.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwknjjnye.sHtML

JS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gcemqyxeq.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gojzqohel.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/ghefhpmpi.sHtML

Go:   os.Args[1:]
来源：http://www.share.fktsv.cn/Article/details/gkfplhskc.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gkchqtrwz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gcuymlayl.sHtML

[M02] 读取环境变量
来源：http://read.share.vehdjk.com/Article/details/gidpeebkc.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.epnwcf.com/Article/details/gfdzfhszo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gvjortvfb.sHtML

JS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gwtfhfvjg.sHtML

TS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/graesdrzk.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/girgvucfv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/ggebdogeo.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/gqasqlpmt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/grhyqynhw.sHtML

[M03] 执行外部命令
来源：http://3g.bbcook.cn/Article/details/gonazkfuc.sHtML


<!-- 参考信息 -->