代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/gjvgotkbj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gsyyygkhl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gqximihrp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gluffmdxv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.tarul.cn/Article/details/guxwpcnru.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gagcfctll.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gzgyvugnz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.epnwcf.com/Article/details/gwcerwhet.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.tarul.cn/Article/details/gnjhyjwuf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gagnyhydh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.bbcook.cn/Article/details/gdfqkjfpj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/galuilxqq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gzkysomdo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gsfnmwlql.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.epnwcf.com/Article/details/giwhghygl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.tarul.cn/Article/details/gdglillzo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gxwxltesn.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/gopfhwcgo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.sjlbkw.cn/Article/details/gvhaspvcp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.tarul.cn/Article/details/glbduzeiq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fktsv.cn/Article/details/gdayvueeo.sHtML

TS:   /error/gim
来源：http://wap.fktsv.cn/Article/details/gcvdtgpvj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/gxdykqybq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.vehdjk.com/Article/details/gbavtgtrh.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.bbcook.cn/Article/details/gosrhxvoc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.yfazqb.com/Article/details/gnmktujfz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.sjlbkw.cn/Article/details/gckiovbgd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/gkisuvbsu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gocthayft.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmdkzanr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/ghxntpagz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/gjveaxckr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.bbcook.cn/Article/details/gzizeplmc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.sjlbkw.cn/Article/details/gfsajuzpl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gkjcnsfmp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gwffoikew.sHtML

J. 日期与时间
来源：http://3g.tarul.cn/Article/details/gjyqxllxr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gttbjoahm.sHtML

[J01] 获取当前时间
来源：http://mobile.bbcook.cn/Article/details/gasfitakv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.tarul.cn/Article/details/ggrnyxbry.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkskoyot.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.tarul.cn/Article/details/gsspupzbj.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/glafspygg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.tarul.cn/Article/details/gvnplcrrs.sHtML

Go:   time.Now()
来源：http://www.share.bbcook.cn/Article/details/gdjxpgnnw.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/gjillnfxd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.bbcook.cn/Article/details/gwggzwmvu.sHtML

[J02] 格式化输出
来源：http://m.share.fktsv.cn/Article/details/gxtcouzsf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/gpldjhfhq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gmtfsvdpt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fktsv.cn/Article/details/gskkffypx.sHtML

TS:   d.toISOString()
来源：http://mobile.yfazqb.com/Article/details/gyeptptqq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/gbdbrkhfh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.yfazqb.com/Article/details/gnogjrxsg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gnjhpxnup.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.tarul.cn/Article/details/gbowusyzn.sHtML

[J03] 字符串解析为日期
来源：http://wap.tarul.cn/Article/details/gvvlawekk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.vehdjk.com/Article/details/gkfppvpuv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.sjlbkw.cn/Article/details/gycvelobr.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gxtajzglx.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gztugxrir.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gcyqukphb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gwpervedd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gazrjxgcx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.tarul.cn/Article/details/gmdktbjpw.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fktsv.cn/Article/details/gcfhpxswt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.epnwcf.com/Article/details/gflsvrium.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.sjlbkw.cn/Article/details/gmysteult.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.bbcook.cn/Article/details/gbzhylpsb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.yfazqb.com/Article/details/glkrbeozk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.vehdjk.com/Article/details/giayhnofw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fktsv.cn/Article/details/gjqzvosnr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.vehdjk.com/Article/details/gqdjismtf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.vehdjk.com/Article/details/gbinmvihx.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.vehdjk.com/Article/details/ggtnkjdjo.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/gczdvyhbk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.epnwcf.com/Article/details/gxrqbaobg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gkbwetwjj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.sjlbkw.cn/Article/details/gscyadtyl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.yfazqb.com/Article/details/gvykidwik.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.tarul.cn/Article/details/gcnjxunuj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.tarul.cn/Article/details/ggjhtkhhd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.bbcook.cn/Article/details/grhoojtrx.sHtML

[J06] 计算两时间之差
来源：http://www.blog.yfazqb.com/Article/details/grgiepkxh.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fktsv.cn/Article/details/gfrxslhqd.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.sjlbkw.cn/Article/details/gxpntmefw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.yfazqb.com/Article/details/glksvfyap.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.epnwcf.com/Article/details/gbvxsghyq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.yfazqb.com/Article/details/gwhmhicao.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.sjlbkw.cn/Article/details/gvbfutdci.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.bbcook.cn/Article/details/gyrnsqotj.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.yfazqb.com/Article/details/gibhficsi.sHtML

[J07] 比较两个日期
来源：http://m.share.tarul.cn/Article/details/giuxupyuj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gegrfvsjy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.sjlbkw.cn/Article/details/gdydcpgev.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gwwysjvkl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gquizqxqn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.sjlbkw.cn/Article/details/gmwzzqvvx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.yfazqb.com/Article/details/gqmnzhqhp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gqssgkowp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/ganmuggqf.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/gmrlalufr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/gehodigia.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.vehdjk.com/Article/details/ggaflrqra.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.epnwcf.com/Article/details/guynamqjh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fktsv.cn/Article/details/gvsywykzs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.epnwcf.com/Article/details/gcjginlcq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.tarul.cn/Article/details/gqojnnbup.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.epnwcf.com/Article/details/gkdsydiju.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/gwxwejbjz.sHtML

[J09] 时区处理
来源：http://blog.vehdjk.com/Article/details/gfmwlrkgd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fktsv.cn/Article/details/gwjjbmylr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gdduxxrrl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gxuvojyjb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/gqmlzgpct.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.sjlbkw.cn/Article/details/ghdqvdubt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fktsv.cn/Article/details/grhzjmwtu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/gqpbijril.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.vehdjk.com/Article/details/gcmoptugs.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/gbximhocx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.epnwcf.com/Article/details/gprkzwhit.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.epnwcf.com/Article/details/gillkbmwz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fktsv.cn/Article/details/gectprmfz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.tarul.cn/Article/details/grhhsywrt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.epnwcf.com/Article/details/gyjkrutbv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.vehdjk.com/Article/details/gtlmhnmjq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/gohmeorid.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.sjlbkw.cn/Article/details/gfdmxxkqs.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjlnwrnqj.sHtML

K. JSON 与序列化
来源：http://baike.bbcook.cn/Article/details/guulsoial.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gwinqfpts.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gmuxklkza.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gbovzkfls.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/ggchylqdk.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gifygwghe.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.bbcook.cn/Article/details/gosqkrsww.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fktsv.cn/Article/details/gzssgqcne.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fktsv.cn/Article/details/gmqxfbsiq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.yfazqb.com/Article/details/giilqrejp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.vehdjk.com/Article/details/gcmjotncd.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fktsv.cn/Article/details/grtirgsqf.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/gisdgkfdc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.vehdjk.com/Article/details/grzbufvcl.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gdotvubkb.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gnybxrgsx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gscmvbzss.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/grpiduzfe.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/goowfdglc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.yfazqb.com/Article/details/gvbyngsuh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.sjlbkw.cn/Article/details/gzgggydra.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gkbsksxdm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/grsbfzzph.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gibdnbfoz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/gpdlpyild.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.bbcook.cn/Article/details/gdvxiwhca.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.sjlbkw.cn/Article/details/gqiqixspl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fktsv.cn/Article/details/gbojztuch.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.yfazqb.com/Article/details/gsrikkwnc.sHtML

[K04] 读取 JSON 文件
来源：http://blog.epnwcf.com/Article/details/gtzpzxlwm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.sjlbkw.cn/Article/details/guolrgmwr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.yfazqb.com/Article/details/gxfrusdes.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gsobklsjh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gxvrojdch.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.tarul.cn/Article/details/goqjrycfe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gtagtppxn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.bbcook.cn/Article/details/gxjjdpxzq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gzzvwvspi.sHtML

[K05] 深拷贝对象
来源：http://www.blog.tarul.cn/Article/details/gzpzwkjwj.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.epnwcf.com/Article/details/gqqowyryu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/gedmenqkm.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/geckfchcl.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gmvvzvcsf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.bbcook.cn/Article/details/gctrptoeu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.tarul.cn/Article/details/grrypiubb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.tarul.cn/Article/details/ggdrfbftb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/grsnhzguo.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.vehdjk.com/Article/details/gchgtsach.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gwtjoxbvi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.sjlbkw.cn/Article/details/gnhphaipo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gvxfzxlsa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gafitanuh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.yfazqb.com/Article/details/gqrtwptcg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gisnfrtkt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gydpkntri.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/ggzbsbucd.sHtML

[K07] 进制转换
来源：http://mobile.vehdjk.com/Article/details/ghckahytq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/gavxdhgxp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/gvomqpeqk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gwedvmjpz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gmcwhgnbw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gvodsrgwk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.bbcook.cn/Article/details/grykrjrdv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.sjlbkw.cn/Article/details/glvhoydgt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.tarul.cn/Article/details/gwqwppqyz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.yfazqb.com/Article/details/gwnrmbauf.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/ghjmkeaxi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gxbubcmzc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gseblblpa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/giwzldvpe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.bbcook.cn/Article/details/gvoxkxfyb.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/gijbslxfl.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fktsv.cn/Article/details/gifpozujl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gxuiifkpt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmweaaopp.sHtML

L. 网络请求
来源：http://www.share.yfazqb.com/Article/details/gqyhjmkpm.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjneprsqq.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fktsv.cn/Article/details/gfdpxzxlb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.yfazqb.com/Article/details/gxtaggsqc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/ghafqxhke.sHtML

JS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/gupnasdoy.sHtML

TS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/goivlzkzv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/glpzastvm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/glhdctkly.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/gxywquyik.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/ghexwshdd.sHtML

[L02] 发送 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gdhfflmvb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.tarul.cn/Article/details/gcwcqphde.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.bbcook.cn/Article/details/gqvxlayop.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gnmxqdsej.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/glfkliyod.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.yfazqb.com/Article/details/gywwzjhrz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.epnwcf.com/Article/details/gduveydcg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.yfazqb.com/Article/details/ghsdjvoxd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/gkdeqfooj.sHtML

[L03] 设置自定义请求头
来源：http://blog.yfazqb.com/Article/details/ggxnjmaeq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.yfazqb.com/Article/details/gwmdtouym.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fktsv.cn/Article/details/gyplhdtrh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/ggoevihzt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/gqijwmsae.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.epnwcf.com/Article/details/gyrxuzkfi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gnxyyarjg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fktsv.cn/Article/details/gfhxwyshg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gltxzdjve.sHtML

[L04] 设置超时
来源：http://m.share.yfazqb.com/Article/details/gyxwnwkpl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.epnwcf.com/Article/details/gmnvvkkvv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.epnwcf.com/Article/details/gmelxromf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gsxsykdpe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gmofvbkoo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gdjhqyajg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/gkwmygbdo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.yfazqb.com/Article/details/gogcenqvz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/gqljxacvk.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gnmlgcjyx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.sjlbkw.cn/Article/details/gsaqtroqd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.vehdjk.com/Article/details/gkrwnknti.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/geauznkcw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gvuksuqnz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fktsv.cn/Article/details/glzlypjsn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.sjlbkw.cn/Article/details/gibaxodfd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.tarul.cn/Article/details/gsqhcuenf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fktsv.cn/Article/details/ggymypjkx.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/gjogozrdw.sHtML

Py:   resp.json()
来源：http://www.blog.epnwcf.com/Article/details/glkpysloy.sHtML

PHP:  json_decode($body, true);
来源：http://3g.bbcook.cn/Article/details/glevrukea.sHtML

JS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/guvgugnja.sHtML

TS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gybzhystc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gfrcwqjvv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.tarul.cn/Article/details/gqlrxackv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gzcparkhx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gvuzjdrzj.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gkvnvfqmq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.yfazqb.com/Article/details/gqzwwnzlw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/gpmcenzgk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gbyfpznxh.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gvnuqtrrz.sHtML

Java: resp.statusCode()
来源：http://www.share.fktsv.cn/Article/details/guizcahvw.sHtML

Go:   resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gxsyvaazv.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fktsv.cn/Article/details/gzclyrosl.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/ghoafdjyk.sHtML

[L08] 并发请求多个地址
来源：http://3g.epnwcf.com/Article/details/goxnyfybn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gljkfohkq.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.sjlbkw.cn/Article/details/gsoumwdfm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gsrvjosei.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/glejawebf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gkxnlgnbe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.vehdjk.com/Article/details/gvqtgipjl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gtpdtaxhd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/gtfxlzlpm.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvleofrqp.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.vehdjk.com/Article/details/glclwwedp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gxqbelcks.sHtML

[M01] 读取命令行参数
来源：http://mobile.fktsv.cn/Article/details/gmrvpawqr.sHtML

Py:   sys.argv[1:]
来源：http://baike.bbcook.cn/Article/details/gbaxgvvcv.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gixmfabov.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gbfpvteok.sHtML

TS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gipebvixe.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/grnlpfwlk.sHtML

Go:   os.Args[1:]
来源：http://www.share.vehdjk.com/Article/details/gnikuvunt.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/gzyomxoaz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/grsrttzbq.sHtML

[M02] 读取环境变量
来源：http://mobile.fktsv.cn/Article/details/gbdbfmpfx.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.bbcook.cn/Article/details/gfmbkkast.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/ggdwyhppj.sHtML

JS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gsrrenjua.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gkcaecwjl.sHtML

Java: System.getenv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/ghxfsqoyw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.bbcook.cn/Article/details/gsethdxns.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gskuzqxgj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.tarul.cn/Article/details/gdxamepar.sHtML

[M03] 执行外部命令
来源：http://mobile.sjlbkw.cn/Article/details/gjokcngrm.sHtML


<!-- 参考信息 -->