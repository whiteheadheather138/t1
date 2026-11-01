代发 wailian999

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghxaurkzt.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gixsbobwi.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwemuwdev.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/gyovvdqad.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gjjxgqocp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gpkajzsye.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/grsoejnjc.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gzitxtpwo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.epnwcf.com/Article/details/gmpkuqlyq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.bbcook.cn/Article/details/gbtsieppn.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gcwipuoop.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/ggwonydot.sHtML

[I02] 提取所有匹配
来源：http://read.share.bbcook.cn/Article/details/gvwcrknfz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gkfqnldpy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.epnwcf.com/Article/details/gvwffozuo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.tarul.cn/Article/details/glrnmtdew.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gfspnjjyw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.tarul.cn/Article/details/gszbttsrv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gngqgjnrw.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gxgbifwpj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.yfazqb.com/Article/details/gwxdgzyxm.sHtML

[I03] 提取捕获分组
来源：http://www.share.sjlbkw.cn/Article/details/gllucqutn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.epnwcf.com/Article/details/gqdhotnfr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/geymocyqt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.yfazqb.com/Article/details/ghshblbuz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.yfazqb.com/Article/details/gmhwzaxmb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.bbcook.cn/Article/details/gbpfyiisl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.yfazqb.com/Article/details/gjeodecvm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fktsv.cn/Article/details/gmnlfairm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.bbcook.cn/Article/details/gafzgifit.sHtML

[I04] 正则替换
来源：http://www.share.bbcook.cn/Article/details/gkqcxuyqg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/gdulsajhg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/grbtdfpam.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gzqvivetw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gvcjnmsgs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/givpoierw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.sjlbkw.cn/Article/details/gcmkomgqz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.sjlbkw.cn/Article/details/gsuplvbxd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gffebeddy.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/gfbeftacn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/gktmdakhl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.vehdjk.com/Article/details/glzubljrp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gucjehsfw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gdswyemfp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.bbcook.cn/Article/details/gfalxjcuc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.tarul.cn/Article/details/gefsnyiuo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gkwbvqmpt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.vehdjk.com/Article/details/grijxgbed.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fktsv.cn/Article/details/gevghkcvt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gwzserfke.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/gnwfxzlxw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gtstixtvh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gsrwfkgmu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.yfazqb.com/Article/details/guqwdbmzl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.tarul.cn/Article/details/gffacjfui.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.bbcook.cn/Article/details/gxmzpinio.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gptcnbuor.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/gjumpljvp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.epnwcf.com/Article/details/glavgnbvd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.vehdjk.com/Article/details/gdsiiwwdp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.tarul.cn/Article/details/gzbkzervb.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/gfgggeihp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmwqwabr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.epnwcf.com/Article/details/gkaosjzpl.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.bbcook.cn/Article/details/gyohmslmf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.bbcook.cn/Article/details/ghvzkdmxr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.tarul.cn/Article/details/gfbsiqbsv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.vehdjk.com/Article/details/grexyjzwk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.bbcook.cn/Article/details/gschsqeaa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gjmafrfsb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gwphnguyi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/gbbbomvnl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.tarul.cn/Article/details/glrhmjnym.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.tarul.cn/Article/details/gjocveinb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/gtrzffwyk.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/goobnozda.sHtML

J. 日期与时间
来源：http://read.share.bbcook.cn/Article/details/gvmansgbt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggnpsztst.sHtML

[J01] 获取当前时间
来源：http://www.blog.vehdjk.com/Article/details/gxylsvavj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxrlevey.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gzmyymgqn.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gtschobsj.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gpnaxxpwy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/glwraruak.sHtML

Go:   time.Now()
来源：http://mobile.yfazqb.com/Article/details/gszqxihfa.sHtML

Ruby: Time.now
来源：http://mobile.epnwcf.com/Article/details/gjtlfcfzv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fktsv.cn/Article/details/ggemmqboh.sHtML

[J02] 格式化输出
来源：http://blog.tarul.cn/Article/details/gwklmzmpz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gjkgqvihr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gpepcpyza.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.tarul.cn/Article/details/ghlewhstj.sHtML

TS:   d.toISOString()
来源：http://www.blog.sjlbkw.cn/Article/details/gvrrtlvkq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.vehdjk.com/Article/details/gsomfduiv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fktsv.cn/Article/details/gmegkexta.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gjplndsju.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.tarul.cn/Article/details/groddzghu.sHtML

[J03] 字符串解析为日期
来源：http://mobile.vehdjk.com/Article/details/getjnrbgz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.yfazqb.com/Article/details/gwuqudwbu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.yfazqb.com/Article/details/ghyecpfll.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gpxsajtyu.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/ggvinarqg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gvcrwjjlw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gofbyuncv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gmprvslsq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.tarul.cn/Article/details/gclkzrnwl.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.vehdjk.com/Article/details/gkifoxaua.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.epnwcf.com/Article/details/gkkepawpy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fktsv.cn/Article/details/gckcuyxoz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fktsv.cn/Article/details/gvoxqiwcb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.bbcook.cn/Article/details/gsexmeira.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gtnykolrf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.epnwcf.com/Article/details/gnvflpohi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gmudpnrqe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/goutirgan.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/ghcstqwfc.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fktsv.cn/Article/details/gkcliarbv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.tarul.cn/Article/details/gjrvrxkyo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gkhfrruzw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/grltymgvd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.vehdjk.com/Article/details/goyvrlejo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.yfazqb.com/Article/details/gffnjspwa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.tarul.cn/Article/details/ggogilsku.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/gifonyokx.sHtML

[J06] 计算两时间之差
来源：http://read.share.epnwcf.com/Article/details/ghxwgofht.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.bbcook.cn/Article/details/glbcdxfof.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.epnwcf.com/Article/details/gqxckgpdg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.vehdjk.com/Article/details/gqgyawulr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.tarul.cn/Article/details/gkytpvqmt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.yfazqb.com/Article/details/govxixcqx.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.vehdjk.com/Article/details/gvwubchpg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.sjlbkw.cn/Article/details/gyldfzntz.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.sjlbkw.cn/Article/details/gamcrwqmn.sHtML

[J07] 比较两个日期
来源：http://blog.epnwcf.com/Article/details/gyotrgpzk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gfqehyjwz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.epnwcf.com/Article/details/gkbamhytd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gowmjbvfe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/ggwlbuhia.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.vehdjk.com/Article/details/gnubxmaqj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.tarul.cn/Article/details/gdsqiztat.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gqsdddyyb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/glleieoho.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.yfazqb.com/Article/details/gdzzrqksi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.tarul.cn/Article/details/gyzsacusa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.vehdjk.com/Article/details/guogcmsrc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.tarul.cn/Article/details/ggvbsbiau.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.bbcook.cn/Article/details/gfnpcvnga.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/gahqfotlr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.epnwcf.com/Article/details/gijxlagoy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fktsv.cn/Article/details/gpkandgap.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fktsv.cn/Article/details/gdxjbiuvt.sHtML

[J09] 时区处理
来源：http://read.share.fktsv.cn/Article/details/gqqojkalm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/glfbcianb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/gkljmmzft.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gmgosuuhg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.vehdjk.com/Article/details/gqvpfubam.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/gfziedoeh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.tarul.cn/Article/details/gmlwmqaex.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fktsv.cn/Article/details/gpzjziwlh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.sjlbkw.cn/Article/details/gnhbxyxsy.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fktsv.cn/Article/details/gtnozxiar.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.yfazqb.com/Article/details/gtzpqovwt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.vehdjk.com/Article/details/gfisejwak.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.sjlbkw.cn/Article/details/gzycivcsb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.epnwcf.com/Article/details/gzcybmtyf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.vehdjk.com/Article/details/ggzougvgm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.vehdjk.com/Article/details/gvijuvdmg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gnkwdnshn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gwordfphm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwdrmhlkv.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/gpukjuzzb.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggtyjnvjc.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.tarul.cn/Article/details/gpklbvgds.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/ghqudyywt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gtwmyizqa.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/grspyuuzm.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gwuvjtkpa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fktsv.cn/Article/details/gclbaxfty.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gheaxbrzy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gqliuasdd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.tarul.cn/Article/details/giugrfumn.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fktsv.cn/Article/details/gbckedvgv.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/gwypqcjaf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.sjlbkw.cn/Article/details/ghlywiefn.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gaxnbzwsb.sHtML

TS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gnfobdfro.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gavcdwscm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gczucaffd.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/grayjuiie.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gaijudcsr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gkzjahvsa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gehynqbfr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gnolrdhav.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/gkqfjhcch.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gjcakibxr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.tarul.cn/Article/details/gzkjnfnmv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/gtjdffmse.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.sjlbkw.cn/Article/details/giylscnow.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fktsv.cn/Article/details/gxqdtbrfc.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/gotvjomby.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/guzqkamxw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.yfazqb.com/Article/details/gttsybgpn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/geylpotjl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gjiiohgko.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.tarul.cn/Article/details/gblkxopaz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/gubqftwtu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gjjjuhzfd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.yfazqb.com/Article/details/gkrcgiqkk.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/gpcprsjoq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gnwrjeijt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.vehdjk.com/Article/details/gqghrivri.sHtML

JS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gsknbrwwl.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/grkvdytsu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.tarul.cn/Article/details/gvqfqzhyj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.yfazqb.com/Article/details/gkulpjplp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/ghmfkwicr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.vehdjk.com/Article/details/gdtskwzzj.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.sjlbkw.cn/Article/details/gjbvxfdha.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fktsv.cn/Article/details/gzkdmdaau.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.yfazqb.com/Article/details/goxwyxnuh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gepruqivv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gzsktulai.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gzrwcysld.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/guhpozavd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gconhqtkb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gqtlbxswl.sHtML

[K07] 进制转换
来源：http://baike.bbcook.cn/Article/details/gbapdpbtk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/giergzbie.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.tarul.cn/Article/details/gnnsjxqac.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/goxrzetyh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/geqxbrgsj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gghwqzasq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.sjlbkw.cn/Article/details/gyupdtkap.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gaxugabvy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gpugwwydl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/gpkhdmsqe.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gxcmvwkzb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/galhqtfzy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gmmfskmew.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/ghhnyoxal.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fktsv.cn/Article/details/grqsasgyg.sHtML

Go:   encoding/gob
来源：http://www.m.share.sjlbkw.cn/Article/details/grpfyvlhq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gkgzghnhv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gpnolaptu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gletlttaq.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gszzzfise.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gonbowfbm.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fktsv.cn/Article/details/gcbldjqkk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.vehdjk.com/Article/details/gnpwjdbut.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/gvcfryojj.sHtML

JS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gfgjpqoln.sHtML

TS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/gmzqrdups.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fktsv.cn/Article/details/gdwgjxgil.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.yfazqb.com/Article/details/gqkrqodep.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fktsv.cn/Article/details/gihzirbky.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fktsv.cn/Article/details/gnyycmqdd.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gbaiasjif.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.bbcook.cn/Article/details/gxlnmwuoh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.epnwcf.com/Article/details/gotirntkv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gsnvfabkp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gpkkeamth.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.tarul.cn/Article/details/gtdowvhos.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.vehdjk.com/Article/details/gsnpybnni.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.sjlbkw.cn/Article/details/gbnhjlsyk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.yfazqb.com/Article/details/gkbzmfoyp.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.yfazqb.com/Article/details/gcwfwekgg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/gjqpcxnry.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fktsv.cn/Article/details/gvnodvmhd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxbrcder.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gajflirak.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.vehdjk.com/Article/details/gkloqjxoo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gdabaequx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.tarul.cn/Article/details/gffukildn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gjbbbdiei.sHtML

[L04] 设置超时
来源：http://wap.vehdjk.com/Article/details/gtbfspjnf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.vehdjk.com/Article/details/gkjmmvxnw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/giaytbaxa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gkxwspsts.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/goglfhiyz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gwfclmabs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.bbcook.cn/Article/details/gxvcysgia.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.yfazqb.com/Article/details/grchvjevc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gkhsxtwlx.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.bbcook.cn/Article/details/gctegnjvi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.vehdjk.com/Article/details/gamjohogq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/gtitiketw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gktdaeczy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gyppbarug.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fktsv.cn/Article/details/grnydtsvn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fktsv.cn/Article/details/gitcxfpjd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gllpsuzid.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gdhirwsks.sHtML

[L06] 解析响应为 JSON
来源：http://baike.bbcook.cn/Article/details/gkibibzgs.sHtML

Py:   resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gtvzednbb.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gfuhstgzq.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gbjxvfwgp.sHtML

TS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/grrvuqulp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gxfahxlvc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fktsv.cn/Article/details/gguwhcgus.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.epnwcf.com/Article/details/grusbscuj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.yfazqb.com/Article/details/girlplyzv.sHtML


<!-- 参考信息 -->