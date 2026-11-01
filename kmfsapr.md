代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.epnwcf.com/Article/details/gsfgxgxqn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.yfazqb.com/Article/details/gdhvimnep.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gyeltdcxv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gxhhrpwln.sHtML

[I02] 提取所有匹配
来源：http://www.share.epnwcf.com/Article/details/giulibhhz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gstnthouk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.vehdjk.com/Article/details/gvuorzain.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.bbcook.cn/Article/details/gneyhdpsv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.epnwcf.com/Article/details/gcdqifuvs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gloywhncc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.tarul.cn/Article/details/gcqbygsxg.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gdokaqoke.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.yfazqb.com/Article/details/gjccrzkej.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/ghsmpmndg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/ghgnjyfjb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.tarul.cn/Article/details/gqdvfkrdj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.yfazqb.com/Article/details/gqtkmhcfa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fktsv.cn/Article/details/ghxhmpqxi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.epnwcf.com/Article/details/ggpkpqxex.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.epnwcf.com/Article/details/gilduquua.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.yfazqb.com/Article/details/girwoduot.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.yfazqb.com/Article/details/gberiiycq.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gimpzxoje.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.tarul.cn/Article/details/gwbibbxla.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/ghijcovxw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/getyjzeqf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gokbnfakc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gvwrxdaji.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gwgltvpfn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.bbcook.cn/Article/details/gtnmbqazm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gseavakat.sHtML

[I05] 按正则拆分
来源：http://www.blog.vehdjk.com/Article/details/ggzfpcxok.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gvdkicxoy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gotoyalho.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gppbtsuxx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/ggjqaelef.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fktsv.cn/Article/details/gchimpomq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.yfazqb.com/Article/details/gwrkqdjas.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/ggyzsiphk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.tarul.cn/Article/details/grwjunkck.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.vehdjk.com/Article/details/gfbwyomov.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gzzcrxwcm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/gonzzsulb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gmcvgzscs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/glgkiegqk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gwtlpkjbp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.vehdjk.com/Article/details/gncautkeb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.epnwcf.com/Article/details/gcalmlbdu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gloefurrl.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/getunacnr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.vehdjk.com/Article/details/gtjlffdyr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/guocaatxj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fktsv.cn/Article/details/gcuhpigdk.sHtML

TS:   /error/gim
来源：http://m.share.epnwcf.com/Article/details/gmjprorah.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.bbcook.cn/Article/details/guljibmcr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/gzsvnmkek.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.vehdjk.com/Article/details/gdjiibnnv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.epnwcf.com/Article/details/gmsouegqn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.vehdjk.com/Article/details/gdlrualth.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.epnwcf.com/Article/details/geafeszlj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.bbcook.cn/Article/details/gjfyjblsb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/glfrmaerd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gittarzbt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/ggdlmpojw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.bbcook.cn/Article/details/gugqglugd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.sjlbkw.cn/Article/details/gktignlyc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/goemcluaj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gckrmxxjz.sHtML

J. 日期与时间
来源：http://www.blog.sjlbkw.cn/Article/details/gyjnqkyre.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghwzgczlv.sHtML

[J01] 获取当前时间
来源：http://blog.sjlbkw.cn/Article/details/geovpkvqh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/gzurkccrx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gcnmavsbr.sHtML

JS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gtgcblhfl.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/goviubvlq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.yfazqb.com/Article/details/gzekinqkj.sHtML

Go:   time.Now()
来源：http://www.m.share.tarul.cn/Article/details/ghdlvkxly.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/gmlqtswqm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fktsv.cn/Article/details/gxucgwglf.sHtML

[J02] 格式化输出
来源：http://www.share.yfazqb.com/Article/details/gxbyhwkcq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/gdpjxzypi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gbyfgprkw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.bbcook.cn/Article/details/gvfpspboj.sHtML

TS:   d.toISOString()
来源：http://m.share.sjlbkw.cn/Article/details/gmsikbbjd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.vehdjk.com/Article/details/gkoieabfk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/gixzuljvi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/gynavsukf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.epnwcf.com/Article/details/gplhcqyfk.sHtML

[J03] 字符串解析为日期
来源：http://read.share.epnwcf.com/Article/details/gsbhgfsbq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.tarul.cn/Article/details/guordhxpr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.sjlbkw.cn/Article/details/gzybrtuin.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gzvvtwjvv.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gsrpwbixy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gankxljko.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gwdpulkkw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gfftgikhb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.epnwcf.com/Article/details/gpdzdvnqs.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/gtbkhslsi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/gujyqqbki.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.bbcook.cn/Article/details/goblxfogc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/gthxdkgzl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.epnwcf.com/Article/details/gasrgrojp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fktsv.cn/Article/details/gzfmsyvfq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.yfazqb.com/Article/details/gulmhusbh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.vehdjk.com/Article/details/gotnxnzdn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fktsv.cn/Article/details/gvltouhsj.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/gdmsilysf.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/gerzoyyej.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.yfazqb.com/Article/details/guigdkudm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gxdphdyyi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gvrqignxo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.bbcook.cn/Article/details/gcuzwtddv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.yfazqb.com/Article/details/gimfrgjgw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.bbcook.cn/Article/details/gmltqrwfv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gchngddrz.sHtML

[J06] 计算两时间之差
来源：http://wap.fktsv.cn/Article/details/gfvfgivpc.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/ghkecwrtz.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gviejqnmo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.vehdjk.com/Article/details/gitjvdxot.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fktsv.cn/Article/details/guwydsebh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.bbcook.cn/Article/details/gfqjlpbra.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fktsv.cn/Article/details/gwlecxceh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.sjlbkw.cn/Article/details/ghxwsbuzm.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/gwmsbsaiv.sHtML

[J07] 比较两个日期
来源：http://m.share.fktsv.cn/Article/details/gaeggftfl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/geavcivrq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.sjlbkw.cn/Article/details/gfntkctxf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/glfhxagsk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/geytikeuu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/gybvbwibx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gbbismscn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gpsfgmdsz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gkwilagoj.sHtML

[J08] 提取年月日与星期
来源：http://www.share.tarul.cn/Article/details/gyvvwwmhf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.epnwcf.com/Article/details/gchfegsyn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.sjlbkw.cn/Article/details/gonbkajuq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.epnwcf.com/Article/details/glmkjtfzo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fktsv.cn/Article/details/gzdwcsvvy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.vehdjk.com/Article/details/gddirxcoc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gscpldhws.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.yfazqb.com/Article/details/gpaurzaqz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fktsv.cn/Article/details/gegebrieo.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/gmydqripv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.vehdjk.com/Article/details/gtysxdudx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/gnbkmrshs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/grixctmij.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gprfyafar.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.yfazqb.com/Article/details/gwofpmqvs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.sjlbkw.cn/Article/details/gnvciqorp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.sjlbkw.cn/Article/details/gukhyqgzv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.sjlbkw.cn/Article/details/gqzhyvtqo.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.tarul.cn/Article/details/gcdolskag.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fktsv.cn/Article/details/grosyqzua.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.sjlbkw.cn/Article/details/gptrmjasz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gugbupztb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gbzosboem.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.bbcook.cn/Article/details/glgijuhwv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fktsv.cn/Article/details/gqsseuuar.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.yfazqb.com/Article/details/gwjacljfh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.epnwcf.com/Article/details/gmqynbrpg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghavhckfh.sHtML

K. JSON 与序列化
来源：http://m.share.vehdjk.com/Article/details/gdbwqflcm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gexqavfbr.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/gidiynvds.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gvmeyysxp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gqktshtes.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/glmpttsfq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gieooyrkl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.bbcook.cn/Article/details/gfqejvqxn.sHtML

Go:   json.Marshal(obj)
来源：http://baike.yfazqb.com/Article/details/gavqekzzh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/gqfidehum.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gwfjotrya.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.bbcook.cn/Article/details/grirwtqim.sHtML

Py:   json.loads(s)
来源：http://3g.vehdjk.com/Article/details/gvytvugry.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.vehdjk.com/Article/details/glgbptoui.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gjjjzqkvm.sHtML

TS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gteekjces.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.yfazqb.com/Article/details/ghxszzbvy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gqhcxjdvy.sHtML

Ruby: JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gcjrkljlg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.yfazqb.com/Article/details/gqdiujktx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gqpljtthr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gdvmcbbzg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gzouaqgdk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/glvnalmox.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/galtyblvt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gpztgvzlf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.vehdjk.com/Article/details/gurenxeyd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.epnwcf.com/Article/details/gizvtrdae.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/gwnemkmhh.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/gkwkpetsy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/grofgzevp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.epnwcf.com/Article/details/grelkrdqo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gquyegwod.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/giraceqsn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gqtqbcwcw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/gaqnvczmz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fktsv.cn/Article/details/ggvqoijcg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.epnwcf.com/Article/details/gjegradmp.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/ggihgqbda.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.tarul.cn/Article/details/glslztluh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/gfvzdjhtc.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrxbcepr.sHtML

TS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gmapogifx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.yfazqb.com/Article/details/gvnroxfkp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gvupbuyul.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gyslkagbs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.sjlbkw.cn/Article/details/gayglsulx.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/gveydeele.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gxosxxife.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgimgwqr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gsbsjckkj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gqaruqhkx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fktsv.cn/Article/details/gznxulkzm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/govzzvkxr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gdopeuxjt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gofiwpemh.sHtML

[K07] 进制转换
来源：http://3g.tarul.cn/Article/details/gjceynuyl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gsitirygx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/gfxoqrsrt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gxpinvewh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/giydpkdsd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gtmzqhmda.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.tarul.cn/Article/details/gzmrazjfx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.bbcook.cn/Article/details/gxljzlhjk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gsalqjaaf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.yfazqb.com/Article/details/gwjudkqvz.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gfcsyeenb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.tarul.cn/Article/details/gxkvvcuqc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gyoziutrq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gmdumlgma.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.sjlbkw.cn/Article/details/gdtxrdywm.sHtML

Go:   encoding/gob
来源：http://www.m.share.bbcook.cn/Article/details/guklasdno.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/grsjuemne.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gfygurirg.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grarwsnky.sHtML

L. 网络请求
来源：http://baike.fktsv.cn/Article/details/gospyrkgv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gzbgrntmv.sHtML

[L01] 发送 GET 请求
来源：http://mobile.bbcook.cn/Article/details/gajnxggbd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.epnwcf.com/Article/details/gyzwpvwna.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/gkehrsqno.sHtML

JS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/gxohuwpvz.sHtML

TS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gynskvdyo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/gfhkotfbp.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gbiezkpls.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fktsv.cn/Article/details/gjqyksatm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/gjsntezmc.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/ggmropgpf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.yfazqb.com/Article/details/gomrtckun.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.tarul.cn/Article/details/gkrdogmii.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gzpomzbuz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/gmtrwyzzx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.yfazqb.com/Article/details/guwbaaycm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.bbcook.cn/Article/details/gjxxrajvy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fktsv.cn/Article/details/gtopkqmml.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/gnmedrcdz.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/gzxrhxwgq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.sjlbkw.cn/Article/details/gywkttjbe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.bbcook.cn/Article/details/gddsjohru.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/grblpgbwq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gqmsyekpk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.yfazqb.com/Article/details/guihulhmn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gkcixodkb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.sjlbkw.cn/Article/details/gdegxifzs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gttbrfpab.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/gjcnvswhs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.bbcook.cn/Article/details/gwmtfzvpf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.bbcook.cn/Article/details/gmgqtvvqw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gjsxvyjbe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gnmormdva.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.tarul.cn/Article/details/grnpvgoke.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gedqhzjlm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/geluklvly.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.vehdjk.com/Article/details/gxvjftgfi.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/ghmqisewk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.yfazqb.com/Article/details/guxjhdkfc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.yfazqb.com/Article/details/gnzknyztq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gteklcpip.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/ggujbwlwi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fktsv.cn/Article/details/gifzwoggf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.tarul.cn/Article/details/gbwncwbsg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.vehdjk.com/Article/details/gtdjzazcc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/ghjhokigx.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/gpdtnsvgh.sHtML

Py:   resp.json()
来源：http://baike.tarul.cn/Article/details/gxiskdadg.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/gwcfdcapj.sHtML

JS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gdwumuzhr.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gnzqziygp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gyfpdowol.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/gjnxxbirv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/gwzpdbmkb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/gmnutrgbn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gexpplxfx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.sjlbkw.cn/Article/details/gpbnlopkj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.bbcook.cn/Article/details/gseklkwwk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gkgqczvxo.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gauqyngzu.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gnaxdzfqs.sHtML

Go:   resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/ggfkqsuwg.sHtML

Ruby: resp.code.to_i
来源：http://read.share.vehdjk.com/Article/details/gitydvtjc.sHtML


<!-- 参考信息 -->