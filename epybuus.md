代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fktsv.cn/Article/details/geclitjrn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fktsv.cn/Article/details/gwvifftnd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.vehdjk.com/Article/details/gqdrhscml.sHtML

[I05] 按正则拆分
来源：http://baike.sjlbkw.cn/Article/details/ghxmkhnfd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.tarul.cn/Article/details/gymxbdcdv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.tarul.cn/Article/details/gjubdtsok.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/glesqminj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gaxvxobqg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.sjlbkw.cn/Article/details/geyivyysp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fktsv.cn/Article/details/gpdrozhte.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gtynswztg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gvzjvbidp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.vehdjk.com/Article/details/gsggpsjaa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gbltvelkf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvwlfxvq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gxfmcgvpt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gsguvcfou.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gpzolfzrz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.vehdjk.com/Article/details/gwgsojdbo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.sjlbkw.cn/Article/details/galtglesw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gsewajuvf.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.yfazqb.com/Article/details/gigkernif.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fktsv.cn/Article/details/gnvzbmceu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gnrwbybjo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.vehdjk.com/Article/details/gyepalako.sHtML

TS:   /error/gim
来源：http://baike.bbcook.cn/Article/details/gnwyvacij.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/ghjlyocbi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.tarul.cn/Article/details/gidkemcao.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.vehdjk.com/Article/details/gzxpsavvg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.bbcook.cn/Article/details/gathwllxw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.epnwcf.com/Article/details/glzogwxlr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.epnwcf.com/Article/details/gacrnmfzw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gampiidkp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gwkzunrjs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/ghwwpakvu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gmpqyihvb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.epnwcf.com/Article/details/ghuqynhym.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fktsv.cn/Article/details/gwluflgso.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gamtfuvch.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grduiwpis.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/glrpxqrhz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpvhxjcid.sHtML

[J01] 获取当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/giqsfpxgm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.bbcook.cn/Article/details/gkftehenz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gnkdllrda.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.yfazqb.com/Article/details/gwkwetoyu.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gjwscibry.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/gysbubonl.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/ggzhqiqnv.sHtML

Ruby: Time.now
来源：http://baike.sjlbkw.cn/Article/details/gxgsxagwu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.yfazqb.com/Article/details/gotgmylwm.sHtML

[J02] 格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gwnekynut.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/guopkjgmo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gtrsewndr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.bbcook.cn/Article/details/gdtpfmizg.sHtML

TS:   d.toISOString()
来源：http://read.share.sjlbkw.cn/Article/details/grxhgzjpt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/gtgwzxtbh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fktsv.cn/Article/details/gtsmajymf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gssqsrhhz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.yfazqb.com/Article/details/gwxbdtgcl.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.tarul.cn/Article/details/goprxihco.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.tarul.cn/Article/details/gyaioiktl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjafswtnm.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gcnqgmycq.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gvpawtfma.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gwtisaixh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/govkfqmlv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/grckgtgdk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/gyocngvxp.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.vehdjk.com/Article/details/gweevgqfh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.vehdjk.com/Article/details/gztdoebug.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.vehdjk.com/Article/details/ggttrzzhe.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.vehdjk.com/Article/details/gzxdaarpx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.bbcook.cn/Article/details/gmwamzyqs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/gldjmdzlt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.yfazqb.com/Article/details/gwmwhpnmh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.tarul.cn/Article/details/gdxcjpycd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/gfkerhtfj.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.epnwcf.com/Article/details/gzfvqhzzy.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.sjlbkw.cn/Article/details/gxfbmvvro.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.vehdjk.com/Article/details/gxdkswhfa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/givwmrdzs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/glnmfmcuu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fktsv.cn/Article/details/gdcymqaqv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/gxashuzhx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fktsv.cn/Article/details/gaswtnreb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.epnwcf.com/Article/details/gvzqcvxht.sHtML

[J06] 计算两时间之差
来源：http://wap.vehdjk.com/Article/details/gxzrdzdls.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/gelkepvqe.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gfhbbcpem.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.epnwcf.com/Article/details/gwlpzjtfu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.bbcook.cn/Article/details/gphndhphk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.yfazqb.com/Article/details/gvbuhgsjm.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.sjlbkw.cn/Article/details/gfqvdjduj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.sjlbkw.cn/Article/details/geekekbqt.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/gznwszshg.sHtML

[J07] 比较两个日期
来源：http://wap.yfazqb.com/Article/details/gqjrjizvz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gadhnauel.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gakqntfdi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gxutwvmlq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/ghrdtueau.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.vehdjk.com/Article/details/gokycehrv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gnzbwxpoq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gisdaivlw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/graevjuop.sHtML

[J08] 提取年月日与星期
来源：http://read.share.tarul.cn/Article/details/gnvhncdbr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.sjlbkw.cn/Article/details/gwgpmtijx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/ggtlcympr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.yfazqb.com/Article/details/gqnxtotga.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.yfazqb.com/Article/details/gdzcpills.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/gsczijonf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.yfazqb.com/Article/details/gcftzqzgd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gtwqtiemo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.sjlbkw.cn/Article/details/ghptcmdmg.sHtML

[J09] 时区处理
来源：http://www.m.share.fktsv.cn/Article/details/gruhasjie.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/gmlkeeqzx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.sjlbkw.cn/Article/details/gedmqaxku.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gtpnuxkjb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/grirsvapw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fktsv.cn/Article/details/gxjmnrgex.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.epnwcf.com/Article/details/gbohadwlf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.vehdjk.com/Article/details/gkeuwgzpr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.yfazqb.com/Article/details/grtkopfim.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/gakhthrpt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fktsv.cn/Article/details/gjvplgrij.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.vehdjk.com/Article/details/gvtdkqfpv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gblitjrya.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.yfazqb.com/Article/details/gwvqnwdze.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.yfazqb.com/Article/details/gzxuyfmrb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.epnwcf.com/Article/details/gmjsemnex.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.epnwcf.com/Article/details/goznzofdu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.bbcook.cn/Article/details/gwffuawtx.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfoigmjki.sHtML

K. JSON 与序列化
来源：http://read.share.sjlbkw.cn/Article/details/gacqqcfwz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnszpnbnu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.bbcook.cn/Article/details/gwbgqmpzi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gajtzbdhv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/grzmcdwmm.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gaqhkynyd.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/guwczzeew.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/gglbomunv.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gdmhjblan.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.yfazqb.com/Article/details/gmeuisndj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fktsv.cn/Article/details/gtbxyqrun.sHtML

[K02] JSON 字符串转对象
来源：http://blog.epnwcf.com/Article/details/gysgyivsp.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/giwcqinee.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.tarul.cn/Article/details/gpjrvenuh.sHtML

JS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gcikqyilf.sHtML

TS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/glnzdedrv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.tarul.cn/Article/details/gjjgybeuk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/gpmajqtar.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/ghqxwjmfa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.vehdjk.com/Article/details/guecjaedf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/gifyijvbu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/gqulnjaco.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/gfaeovhgg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gkrtzutav.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gvlonsquk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.yfazqb.com/Article/details/gkoaqarvp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gqsuqevui.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gleopmcqj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.vehdjk.com/Article/details/gawdutkjr.sHtML

[K04] 读取 JSON 文件
来源：http://3g.vehdjk.com/Article/details/gsntljhyo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.epnwcf.com/Article/details/gstiqmgiw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fktsv.cn/Article/details/gmisurylu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gbkmdkvtd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/guarhhcyo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.bbcook.cn/Article/details/gskkpxnnz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/ggpusmzcv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.yfazqb.com/Article/details/gjfgapbyz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.vehdjk.com/Article/details/gdaktzaho.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/gmecppgef.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gvfhyhwim.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fktsv.cn/Article/details/gngwkmnmi.sHtML

JS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/grqqnwahq.sHtML

TS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gxfzpzxmf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.bbcook.cn/Article/details/gghffigik.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.yfazqb.com/Article/details/gvdxqhujh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.bbcook.cn/Article/details/gflrnqigc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/gjiahxrxj.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/gxlpwiiau.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.tarul.cn/Article/details/gxakygbrg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gplfftpop.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/goowzixml.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gqyrmmokq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/gojmkyphb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gdukajezz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gdxylzdur.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gmoczttgs.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gicmxqyit.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gfoqwnvyq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.bbcook.cn/Article/details/gufbtxvqv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gixqtmaim.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gylwqbyfx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/grxzfbhxq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.vehdjk.com/Article/details/glqovkrww.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fktsv.cn/Article/details/guukoscgz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gkocylrrz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.epnwcf.com/Article/details/goewrgjmf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.yfazqb.com/Article/details/gdgzqjvja.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.sjlbkw.cn/Article/details/gngnohics.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gvdurjohy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gtsaxvyux.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.vehdjk.com/Article/details/gafondqzr.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gitclskxy.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.sjlbkw.cn/Article/details/gviegyuxf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fktsv.cn/Article/details/gjkoczaqi.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtrmsdpxr.sHtML

L. 网络请求
来源：http://read.share.vehdjk.com/Article/details/grmrnjjhu.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpaqggrxt.sHtML

[L01] 发送 GET 请求
来源：http://3g.yfazqb.com/Article/details/gaqfgoxts.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.yfazqb.com/Article/details/gfcxcfezx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fktsv.cn/Article/details/gjjeacgto.sHtML

JS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gbeykdfxj.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gnuqlqbqs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.sjlbkw.cn/Article/details/gosrqruvh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.epnwcf.com/Article/details/gncvksbrb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/ghluvdezg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/ggcjkikej.sHtML

[L02] 发送 POST JSON
来源：http://m.share.tarul.cn/Article/details/glzgkjyne.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.bbcook.cn/Article/details/gcmlqqwhv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.yfazqb.com/Article/details/gzoftabcq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gynqbrfnw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gjtffyghj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.tarul.cn/Article/details/gzkqqppzi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fktsv.cn/Article/details/gizsgzkia.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/gdxvwpsup.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/gvwkswwrt.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.vehdjk.com/Article/details/gqjxumeef.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gdresgmek.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gvggcnkuc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/guogfqwsi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gjcvituhs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/ghbcaqhdm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/gonljponp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/glcbvvwfp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gjsigikhj.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/gzntzcwhg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.yfazqb.com/Article/details/gkiuxydko.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.sjlbkw.cn/Article/details/gqweqcdzb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/glcohaxkr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/glulxlvmu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/ggkxxbxyd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gyliugmzb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.bbcook.cn/Article/details/gmbwqjsxv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.tarul.cn/Article/details/gjtsozpve.sHtML

[L05] 上传文件（multipart）
来源：http://3g.bbcook.cn/Article/details/gadnctgzf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.tarul.cn/Article/details/gefilgbbe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/gyyoegwms.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gsbnuzvuk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gkccfxnsp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fktsv.cn/Article/details/gxnpjrmhc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/glotxjwpl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gjkonhwmz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gliwcrcys.sHtML

[L06] 解析响应为 JSON
来源：http://baike.epnwcf.com/Article/details/grhqbvajc.sHtML

Py:   resp.json()
来源：http://wap.tarul.cn/Article/details/gerxcjtjo.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.tarul.cn/Article/details/gnqilvryd.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gyjdhydpd.sHtML

TS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gunxzgiua.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/giotmvudn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.vehdjk.com/Article/details/gyohnhvod.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gwpaaugfc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.sjlbkw.cn/Article/details/gsvbcwhuo.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gexnvdczd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.tarul.cn/Article/details/gswbuozzw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.sjlbkw.cn/Article/details/gykzwalqt.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gfqopgipn.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gvyjlutwo.sHtML

Java: resp.statusCode()
来源：http://m.share.yfazqb.com/Article/details/gmbxexlka.sHtML

Go:   resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gqdbnyztd.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/gapamwkvz.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/grzzxxzdx.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/gaxpqwhvh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.tarul.cn/Article/details/gjzgagmoh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/gkvrkevwu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gdwatmwwi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gforvamke.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gxawucmzg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvgbjxgz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gkcbrpgno.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.yfazqb.com/Article/details/gkyahkkqb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjywvswvp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/ghmlqjlyy.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfzwbmsni.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/gbbkmgdvx.sHtML

Py:   sys.argv[1:]
来源：http://3g.sjlbkw.cn/Article/details/gnczwjacg.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.sjlbkw.cn/Article/details/gpttfoprd.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gnwlucbbf.sHtML

TS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gqetgvtrp.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gjufznudc.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/gspqbdnzr.sHtML

Ruby: ARGV
来源：http://mobile.epnwcf.com/Article/details/gxnuuddqf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gouqdiumq.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gooqvgnmh.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/gwmocgiep.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/ghbrswnsu.sHtML

JS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gtpmsfmtq.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gtbvuubdi.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gvitwzauu.sHtML


<!-- 参考信息 -->