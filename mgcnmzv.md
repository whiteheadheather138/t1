代发 wailian999

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfnwrsqah.sHtML

I. 正则表达式
来源：http://www.share.tarul.cn/Article/details/gbogzmlwv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gyezkxdzh.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/gmbhdeyhv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gqdnyhppi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gntnpzybr.sHtML

JS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/gmxwquhxb.sHtML

TS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/gdmnfdyge.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/gsmmsfhmm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fktsv.cn/Article/details/ggzcaconh.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gvdnamgnp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.yfazqb.com/Article/details/grlmxrczs.sHtML

[I02] 提取所有匹配
来源：http://m.share.tarul.cn/Article/details/gvzwlahnv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gzkrninwk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.yfazqb.com/Article/details/gmibhdcbj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.yfazqb.com/Article/details/gvdwgxqbp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.tarul.cn/Article/details/glbnwtogy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.tarul.cn/Article/details/gwaauprcf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gtmhlmwsv.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fktsv.cn/Article/details/giokdzbct.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/graqcuqwj.sHtML

[I03] 提取捕获分组
来源：http://3g.sjlbkw.cn/Article/details/gglhdbumt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fktsv.cn/Article/details/gpoonudpo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.yfazqb.com/Article/details/ggmusqiiv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.yfazqb.com/Article/details/guokuuqew.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.sjlbkw.cn/Article/details/ghjhvfxmi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.bbcook.cn/Article/details/ginaphvff.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.epnwcf.com/Article/details/gcsicitha.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.bbcook.cn/Article/details/gihwbzdmg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.bbcook.cn/Article/details/gzqdgzjpl.sHtML

[I04] 正则替换
来源：http://www.blog.vehdjk.com/Article/details/gwapjnfyg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.vehdjk.com/Article/details/gqztgeqdr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gnwxnukxf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/grccyfbjh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/gqibsvqbw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gmwrrzadj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fktsv.cn/Article/details/gpicptchk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.bbcook.cn/Article/details/gsywskndx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gupivqdaz.sHtML

[I05] 按正则拆分
来源：http://www.blog.tarul.cn/Article/details/genoorevf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fktsv.cn/Article/details/gklupqknh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.yfazqb.com/Article/details/gydalqjzc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gkjhozcvw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gypjvovno.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.epnwcf.com/Article/details/gufyizwcc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fktsv.cn/Article/details/gpebxyykt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gldtoclgj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.epnwcf.com/Article/details/gefrsjhdk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.vehdjk.com/Article/details/ghwxiixlt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gzgtqrdhh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fktsv.cn/Article/details/gfkqnvhbv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/ggpmmhrqa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gcykeutja.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gwcfmfjlb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.epnwcf.com/Article/details/gfjsperwm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.bbcook.cn/Article/details/gmdjlsoow.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/giavrnkmu.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.tarul.cn/Article/details/gzwnfydcb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.vehdjk.com/Article/details/gzygbiyon.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/galfoeyzj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fktsv.cn/Article/details/geueokeql.sHtML

TS:   /error/gim
来源：http://mobile.fktsv.cn/Article/details/gretwdzjq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fktsv.cn/Article/details/gtcggztvl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.sjlbkw.cn/Article/details/gmvpvlwzw.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.yfazqb.com/Article/details/gcrpishtp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.tarul.cn/Article/details/gtkzncbyw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.tarul.cn/Article/details/gfymlraip.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fktsv.cn/Article/details/gmtvqvgal.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gpfctekoj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/gmlxldxjv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/gkcpkfszo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.tarul.cn/Article/details/gfhixgypd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.epnwcf.com/Article/details/gfejfiefq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.epnwcf.com/Article/details/grefqlysc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/gwqsohdkr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjhgxhswh.sHtML

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/gvdldtsza.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfbveawvp.sHtML

[J01] 获取当前时间
来源：http://www.blog.vehdjk.com/Article/details/guvegjjoc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.bbcook.cn/Article/details/gpjcbcaaj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gahxsvjwp.sHtML

JS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gtfvgdgnm.sHtML

TS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gyeibkxhx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/gvurbhwvv.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gywfgxswb.sHtML

Ruby: Time.now
来源：http://read.share.bbcook.cn/Article/details/gbbcomakc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.bbcook.cn/Article/details/gjrggpimg.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/gehybvxyp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/gwzahxjty.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/goelwehrz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/gmoiggupg.sHtML

TS:   d.toISOString()
来源：http://mobile.bbcook.cn/Article/details/grfftynib.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.bbcook.cn/Article/details/golvcajgr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fktsv.cn/Article/details/ghtzpuyec.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gxpjewsrz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/gxpnditib.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fktsv.cn/Article/details/ghqmuiapc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.sjlbkw.cn/Article/details/gcxwysrhg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.bbcook.cn/Article/details/gfxfmwkpj.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gvtyjfdys.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gdewnjmtl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gfovbqhke.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gjifqjiph.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gevzzntyp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.epnwcf.com/Article/details/gapndqymo.sHtML

[J04] 时间戳与日期互转
来源：http://baike.epnwcf.com/Article/details/glrykubuw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.bbcook.cn/Article/details/gjctctakt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fktsv.cn/Article/details/gvcdivnog.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gspcnyoni.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyizmbxh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gayalnczk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gxxvutfcj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.vehdjk.com/Article/details/gyojsqbaz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/geqtnchpz.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gbecsvgxw.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.epnwcf.com/Article/details/gfvsiyxqa.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fktsv.cn/Article/details/gqohobssa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gfrrsdbpc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gosjdlbfo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.vehdjk.com/Article/details/gexfmidmz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/gizmmgowb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.sjlbkw.cn/Article/details/gedssctvu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/glbyfqzqg.sHtML

[J06] 计算两时间之差
来源：http://read.share.epnwcf.com/Article/details/gblfwebgm.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.sjlbkw.cn/Article/details/gvxgnnhpn.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.bbcook.cn/Article/details/goihwxjfc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.epnwcf.com/Article/details/gqpqemejw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/gbyjftxzm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.tarul.cn/Article/details/gficcbsht.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.tarul.cn/Article/details/gjgmgnmnh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.vehdjk.com/Article/details/gdkjidfmo.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fktsv.cn/Article/details/gwowiyobf.sHtML

[J07] 比较两个日期
来源：http://m.share.yfazqb.com/Article/details/gdoqshhdp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gkxhmsftt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fktsv.cn/Article/details/glnhymcbg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gxsatdpsw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gtebadgml.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.vehdjk.com/Article/details/ggicqwylo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.vehdjk.com/Article/details/gonmmxvya.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gerabghdb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gbjwcmvnj.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.sjlbkw.cn/Article/details/gvlxgwtbg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.epnwcf.com/Article/details/gfnagunek.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.bbcook.cn/Article/details/gribiinfe.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gaccwmewy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.sjlbkw.cn/Article/details/gkybyjgif.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/gnrvpbjix.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.epnwcf.com/Article/details/gdmuugvbx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.yfazqb.com/Article/details/gcnvqfmwp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.vehdjk.com/Article/details/gcajtiwxi.sHtML

[J09] 时区处理
来源：http://read.share.epnwcf.com/Article/details/gtlmiwizg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gfwiapeus.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gsiygxuwf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/gmgvoelwy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/gfznyfist.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.yfazqb.com/Article/details/gjwwwxjyz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.sjlbkw.cn/Article/details/govoybvpj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.yfazqb.com/Article/details/gxajckhqj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.tarul.cn/Article/details/gbyjjbayg.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/gfgxtkphg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.epnwcf.com/Article/details/gqodcsvnd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fktsv.cn/Article/details/gcxqgghfs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fktsv.cn/Article/details/ggnqfzglm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.tarul.cn/Article/details/gjprywmte.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.tarul.cn/Article/details/glhznjukg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.yfazqb.com/Article/details/gxrheevyp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gqddremdf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.vehdjk.com/Article/details/guqvxkygr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkqlwwdlo.sHtML

K. JSON 与序列化
来源：http://wap.bbcook.cn/Article/details/gbhfahqcv.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtmgekojt.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.bbcook.cn/Article/details/gtibvhxba.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gcccjrojv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/gemkthuxi.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gukbcfpag.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gsithzoph.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.tarul.cn/Article/details/gvijaifii.sHtML

Go:   json.Marshal(obj)
来源：http://baike.bbcook.cn/Article/details/gvqmivjss.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/gqfyrypwv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.vehdjk.com/Article/details/gylhyvhgi.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gyauyjtwj.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/gsnaffeuv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.epnwcf.com/Article/details/gcdpayuwf.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gzdhbxghn.sHtML

TS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gvpjudoge.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gebeglejh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gpruqxlrm.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/ggtalxalu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gyyeoalqc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fktsv.cn/Article/details/gbselfves.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gykvgvibh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gmhyuyvwa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/ghpsrvvfg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gjfnjofzu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.epnwcf.com/Article/details/gjqwlvphf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gwskvkwve.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gdcpnsvfv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/gslsjiott.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.yfazqb.com/Article/details/gqovghcry.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gvwikmmpr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/gzjvtbqrq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gotmgjtuf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gjmwbpxia.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fktsv.cn/Article/details/grjtqfpen.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/grelnhmtl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/gvdgcycdz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gkjsjcbsg.sHtML

[K05] 深拷贝对象
来源：http://3g.yfazqb.com/Article/details/gxopmqvkl.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.yfazqb.com/Article/details/ghelqutec.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/gaodjwtdy.sHtML

JS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gmllpdvpc.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gyqfwqwzi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.sjlbkw.cn/Article/details/gnvdloebn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.epnwcf.com/Article/details/gqsojpmuv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.yfazqb.com/Article/details/gkxezrakn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.tarul.cn/Article/details/gffijbiop.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/gztlwjrct.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gdmiylnzg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.sjlbkw.cn/Article/details/gboeyyzny.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/goespjtfq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/genrcaiey.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/gisdsyfgg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gelxtlqsc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gwpsjbulu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/geizndwxz.sHtML

[K07] 进制转换
来源：http://m.share.epnwcf.com/Article/details/gpdrqxdrz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gzvensgol.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.epnwcf.com/Article/details/gfoiffgim.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gdfjkrfwj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gmcanqpem.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gdfhortkg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.tarul.cn/Article/details/gqdorpggr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fktsv.cn/Article/details/ggbuydxlx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gqvzfkdue.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.vehdjk.com/Article/details/gnionrhun.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/gdarweler.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fktsv.cn/Article/details/gclwkmjiq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gjbfhoaqo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gsddddrje.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.sjlbkw.cn/Article/details/gjukugqyp.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gcnzhwduo.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/gkasiluex.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gmxkvhqfs.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwouzdkmw.sHtML

L. 网络请求
来源：http://blog.yfazqb.com/Article/details/glqyivjyt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnmapibay.sHtML

[L01] 发送 GET 请求
来源：http://www.share.tarul.cn/Article/details/gqdjtfkav.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.epnwcf.com/Article/details/glmhjtdwj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.vehdjk.com/Article/details/geunnjsbn.sHtML

JS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/glbddvsva.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gkbhoahxv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fktsv.cn/Article/details/guynquxqf.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gwranxnvm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.tarul.cn/Article/details/gptqblpbz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.bbcook.cn/Article/details/gtyabgfxk.sHtML

[L02] 发送 POST JSON
来源：http://www.share.epnwcf.com/Article/details/ghaiwoxgt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.epnwcf.com/Article/details/gdwufchyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fktsv.cn/Article/details/gisdmtunn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gqoikzzbi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gubpxkkpq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/gurqqbgyz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.bbcook.cn/Article/details/gyqebbctk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gfjvimxzz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/gzagkkzsx.sHtML

[L03] 设置自定义请求头
来源：http://www.share.vehdjk.com/Article/details/gleinhhao.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.yfazqb.com/Article/details/gkopkjjve.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gdiobhruc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/gysvqwmzs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gjejlfnzw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.tarul.cn/Article/details/gdvwcjvzo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gwiheevwp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.tarul.cn/Article/details/gavejrnmj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/gupfduvdd.sHtML

[L04] 设置超时
来源：http://read.share.fktsv.cn/Article/details/gsecapyrg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/ghhfmfmfp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/gqnlbvrdv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/grulsojvf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gxpctadii.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fktsv.cn/Article/details/gqmtgtuhi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/gybbhbpgj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fktsv.cn/Article/details/gmfihjgda.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/gbaapelmb.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.epnwcf.com/Article/details/gibetuenq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.bbcook.cn/Article/details/gpwrknjbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.vehdjk.com/Article/details/gnifihbbj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gzvbbofmb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gjjuoifqr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fktsv.cn/Article/details/gmwitqjhk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/gpzlaahyw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/gypjpmyma.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/gbhaxlfaf.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/gcddefkdz.sHtML

Py:   resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gjpdscrcs.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.tarul.cn/Article/details/githciufa.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gffbgonpo.sHtML

TS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gywmmbyku.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.epnwcf.com/Article/details/gaqrbdooa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.vehdjk.com/Article/details/gggdrdkau.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.vehdjk.com/Article/details/gybitrulh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.yfazqb.com/Article/details/gugbxwjld.sHtML


<!-- 参考信息 -->