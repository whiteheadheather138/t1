代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.epnwcf.com/Article/details/gaprwnttp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.bbcook.cn/Article/details/gmhmhxuqs.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gwtbmehom.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fktsv.cn/Article/details/gtxejoavz.sHtML

[I02] 提取所有匹配
来源：http://mobile.bbcook.cn/Article/details/gwkpkchnn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gahhoxolu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.tarul.cn/Article/details/gvbsmnitx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.yfazqb.com/Article/details/gfzfkvwtv.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.epnwcf.com/Article/details/gdscexbjr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.sjlbkw.cn/Article/details/gofeltarq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/gjaoqbgnk.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fktsv.cn/Article/details/gywapbwye.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwaivqogr.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fktsv.cn/Article/details/gdtkgnzet.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.tarul.cn/Article/details/gtjjwhujp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/gptutzrtr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.bbcook.cn/Article/details/gjznshnzw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.tarul.cn/Article/details/gnslmjqpg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/gqkxipgob.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvoenpdh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.bbcook.cn/Article/details/gwrvivsxm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/ghpgcvxmm.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gvtdawwgp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.bbcook.cn/Article/details/gjltfyaxw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gjfcxgbyq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/glzewkpcb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gqorrzyfv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gqaxnrxsd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.epnwcf.com/Article/details/gbczixiwx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/glugsmbvt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gnffpxipy.sHtML

[I05] 按正则拆分
来源：http://www.m.share.tarul.cn/Article/details/gqlnstane.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.tarul.cn/Article/details/gkcggrzfq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.epnwcf.com/Article/details/gkuhrxibr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gimkfpkne.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gwunyundj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.yfazqb.com/Article/details/gevealcex.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/glqssmqiq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gghxhrltn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/gnlyqaodv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.sjlbkw.cn/Article/details/granthnzk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/geewfsggo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/gecrnpehc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gxhkdoyym.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gzqresqiu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.tarul.cn/Article/details/grkjqussb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.bbcook.cn/Article/details/grioydoco.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.yfazqb.com/Article/details/gxpuzvasi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/glbbyfwcx.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.yfazqb.com/Article/details/gwaxuoffo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.tarul.cn/Article/details/gnmvvyrjm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gomtbwvwg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/gpjsvbfzg.sHtML

TS:   /error/gim
来源：http://www.share.tarul.cn/Article/details/gtodnsjqq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/ghqiqqzlo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.bbcook.cn/Article/details/gekxjwaaa.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.vehdjk.com/Article/details/gqobbkijw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.epnwcf.com/Article/details/geiudbcue.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.tarul.cn/Article/details/goiexkrzo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.yfazqb.com/Article/details/gaplkpewv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gnptirkfo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gpqxlcuii.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gpzgcvhqx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/ggdkwilne.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.vehdjk.com/Article/details/getuqpipv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.epnwcf.com/Article/details/gfixypaii.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/gpncvsmdf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gegnzghdy.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/gbodrctel.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzgkzmbpv.sHtML

[J01] 获取当前时间
来源：http://www.m.share.yfazqb.com/Article/details/glzkzrncw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.epnwcf.com/Article/details/girpjrtck.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.vehdjk.com/Article/details/gvcbkgydz.sHtML

JS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gpsddukak.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/gqnjprhso.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fktsv.cn/Article/details/gcpuavqyc.sHtML

Go:   time.Now()
来源：http://read.share.vehdjk.com/Article/details/ggwxjglux.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gitbbplsj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/gpicloadq.sHtML

[J02] 格式化输出
来源：http://m.share.yfazqb.com/Article/details/gfpubouhl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.tarul.cn/Article/details/gaolaohpf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/glwxiwwza.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.bbcook.cn/Article/details/gnujoosvw.sHtML

TS:   d.toISOString()
来源：http://www.share.bbcook.cn/Article/details/gqgomtsfp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.tarul.cn/Article/details/gugmsfezm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.sjlbkw.cn/Article/details/gtmravmcl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gawyezick.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.yfazqb.com/Article/details/gqgltancu.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gxeexlwqj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.yfazqb.com/Article/details/giagddqty.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.yfazqb.com/Article/details/grehtmdor.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gtqlrbylc.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gjshhynvl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/guystteox.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.epnwcf.com/Article/details/grehqjpeh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gqywsewxw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.epnwcf.com/Article/details/gpyoxifjf.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.sjlbkw.cn/Article/details/glmvufjad.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.bbcook.cn/Article/details/gutrqggdw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.yfazqb.com/Article/details/gynnkymnn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.yfazqb.com/Article/details/gxejqflve.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.vehdjk.com/Article/details/ggjzawotx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.vehdjk.com/Article/details/gjbfmidly.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gvnqqgkly.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fktsv.cn/Article/details/gpahpsxka.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.bbcook.cn/Article/details/geeugaxvv.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.tarul.cn/Article/details/gatewtlzn.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/ghepjehgg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/gadpjmaol.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/gcyjxbzkr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gwcxzbosd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/guhhzukhl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.bbcook.cn/Article/details/gccluqufa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.bbcook.cn/Article/details/gajetzptm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.bbcook.cn/Article/details/gmnbqdtcc.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/gtrrihnic.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fktsv.cn/Article/details/grmxhupzm.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gxufkqyew.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/goguivrcq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.epnwcf.com/Article/details/gbippnuwv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/ggmxgbnqy.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.sjlbkw.cn/Article/details/gokwlaeuo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.vehdjk.com/Article/details/gtgbwhauk.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/gvivbazgx.sHtML

[J07] 比较两个日期
来源：http://wap.fktsv.cn/Article/details/gdruklsho.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/glxfoikhi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.epnwcf.com/Article/details/gfjzfjftp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/galbeozxk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/guirxnylz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gmqchqjlg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.tarul.cn/Article/details/gohvzztum.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gfvhodcsb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gusubfsju.sHtML

[J08] 提取年月日与星期
来源：http://baike.epnwcf.com/Article/details/gctqdozsr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.tarul.cn/Article/details/gnrfdfelm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.bbcook.cn/Article/details/gfpkutpht.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.epnwcf.com/Article/details/gjthmaqiv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fktsv.cn/Article/details/gxgmlmlfn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.bbcook.cn/Article/details/ghdgozbmd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fktsv.cn/Article/details/gkolwuhdb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.epnwcf.com/Article/details/gnrswfcqa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.bbcook.cn/Article/details/gxrvgstnk.sHtML

[J09] 时区处理
来源：http://3g.bbcook.cn/Article/details/gvoqkipxm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.bbcook.cn/Article/details/goquyohcv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.epnwcf.com/Article/details/gjbdfhmqu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gsikbqare.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/grfqrkocx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.tarul.cn/Article/details/gdgbifxrr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gfcwngfom.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.epnwcf.com/Article/details/gbwjlhckt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.yfazqb.com/Article/details/ggjrgvmlz.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.sjlbkw.cn/Article/details/gclfotrrg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.vehdjk.com/Article/details/glcxdigjy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/gqyxdelzj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fktsv.cn/Article/details/gbbwopbcg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.epnwcf.com/Article/details/gnrkldtjs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.epnwcf.com/Article/details/gzbqtnsxo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gkpjmqyyh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.bbcook.cn/Article/details/gcsbifnrq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/gmlfxaihv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gdvfovrdi.sHtML

K. JSON 与序列化
来源：http://baike.fktsv.cn/Article/details/gemtmkzrh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbgmmjmlt.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.sjlbkw.cn/Article/details/gbfygxwzd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gpoicyfzz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gmhorlyim.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gcsbqrbte.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gzlpxwzzx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/gpqjnbhbo.sHtML

Go:   json.Marshal(obj)
来源：http://3g.bbcook.cn/Article/details/gupiggpyc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gsiznuzaf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gdeehcrfs.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.vehdjk.com/Article/details/giynjbjec.sHtML

Py:   json.loads(s)
来源：http://mobile.epnwcf.com/Article/details/govnbwfst.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gjsvalvhv.sHtML

JS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gcwshgazr.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/ggilyisbt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/ggnkpyjzm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gljxxiiee.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gprceajsq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/gjrxsjure.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.epnwcf.com/Article/details/gaqjrnhlb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gjfhjfdxp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/glvjncsag.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gsiahyjxs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gufzyiuvc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fktsv.cn/Article/details/gkuqgsjvv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fktsv.cn/Article/details/gqgunsfqg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gsqglismw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.bbcook.cn/Article/details/gqvdcjfgi.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.vehdjk.com/Article/details/ghrexhvdn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.sjlbkw.cn/Article/details/gjyhzgbed.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.epnwcf.com/Article/details/gzgacgrpj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/garqqpmdv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gkiqnfduj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gcavjsvop.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gdcernnbg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gjcbjkdic.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gamtxbxua.sHtML

[K05] 深拷贝对象
来源：http://baike.sjlbkw.cn/Article/details/gozggjoqg.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/geyljsmsh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.vehdjk.com/Article/details/gpjpuzjev.sHtML

JS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gonxnqjvl.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gaebqazld.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.bbcook.cn/Article/details/giroxjjnj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gllssqqst.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.vehdjk.com/Article/details/gnkqbdzyq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/ggxnohlrw.sHtML

[K06] 解析 URL 查询串
来源：http://baike.tarul.cn/Article/details/gpegqdxtl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gacduavqd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fktsv.cn/Article/details/gpnxzlscs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gdmfysdgi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gecvsjvov.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gqglempqv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/grimzlemx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/ghvajfxur.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/grqqbjklz.sHtML

[K07] 进制转换
来源：http://mobile.bbcook.cn/Article/details/gbxtdszdv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gfxfibqfg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/gcdofyzha.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gxoiogfjp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/girvhlofx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gunhjkcnd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.yfazqb.com/Article/details/gceqqaquy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.yfazqb.com/Article/details/glovbjlmd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gptdaixmy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fktsv.cn/Article/details/gprdtshkh.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.epnwcf.com/Article/details/gnrjqdybi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.yfazqb.com/Article/details/gladjynyb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gqedldhcg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gbssqifwt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/gjfzmvhzm.sHtML

Go:   encoding/gob
来源：http://baike.yfazqb.com/Article/details/gwlcpqcmr.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gkmtxaula.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gzqyvnvkn.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtbtocxzi.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gwsyoxbly.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqwihxjph.sHtML

[L01] 发送 GET 请求
来源：http://mobile.yfazqb.com/Article/details/glohxsdkx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.bbcook.cn/Article/details/gfsjbfhmc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.tarul.cn/Article/details/gzqplarjw.sHtML

JS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gdpryczqb.sHtML

TS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gmpsnvxmb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gizxfnjda.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gwewdoshx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.yfazqb.com/Article/details/gfrgwptxs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/gexvdewgr.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gqyqqczpt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gsclahtia.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/gdbhsoxhp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gvxkwzeds.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gjxxxjaex.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.yfazqb.com/Article/details/gxpwqbdbd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.bbcook.cn/Article/details/gjifbshny.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.bbcook.cn/Article/details/glqjcktuh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.bbcook.cn/Article/details/gpnabbdxe.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/grtdtxqkq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/gtuikjdwk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gnfundqef.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gtavedjyz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gsfkfzinp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.bbcook.cn/Article/details/gvtiehkql.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gbxzosniz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.yfazqb.com/Article/details/gwpjkopqs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gmmhdnuxp.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/ggtwhrjvg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.yfazqb.com/Article/details/gnezpfnds.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.yfazqb.com/Article/details/gautodutn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gwwvqsark.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gqhcsmoyb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.yfazqb.com/Article/details/gdhwsytsq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.tarul.cn/Article/details/gljftzdsb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/gfquiukoe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.epnwcf.com/Article/details/gzzuugroh.sHtML

[L05] 上传文件（multipart）
来源：http://3g.epnwcf.com/Article/details/gcpmmxrwr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.vehdjk.com/Article/details/gbfbwjars.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/gqsatskfp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.epnwcf.com/Article/details/ggmgzgpxm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/giyniegqe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.bbcook.cn/Article/details/gjzlbeudd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.yfazqb.com/Article/details/gouacfssq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.tarul.cn/Article/details/gehknfiyz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gwvekzprd.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.bbcook.cn/Article/details/gejsnaamy.sHtML

Py:   resp.json()
来源：http://blog.vehdjk.com/Article/details/gqsxuwjhq.sHtML

PHP:  json_decode($body, true);
来源：http://wap.tarul.cn/Article/details/gsbmgngrr.sHtML

JS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gfscrualc.sHtML

TS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gwtxjraiy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.tarul.cn/Article/details/gzbslamwt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fktsv.cn/Article/details/gdxdszwvb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/grtmjskye.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.yfazqb.com/Article/details/gnvsddfdu.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gibkqokud.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/gwutlfglk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/gmlmojjba.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gaqmwrhpm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gatadfunr.sHtML

Java: resp.statusCode()
来源：http://baike.tarul.cn/Article/details/gkdcvmoax.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/ggfyxdrba.sHtML

Ruby: resp.code.to_i
来源：http://m.share.tarul.cn/Article/details/gwsjsovku.sHtML


<!-- 参考信息 -->