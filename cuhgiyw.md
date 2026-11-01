代发 wailian999

TS:   s.match(/\d+/g)
来源：http://read.share.vehdjk.com/Article/details/gfkmfmbuq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.vehdjk.com/Article/details/gdlbttish.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.yfazqb.com/Article/details/gjuixygti.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gahhqidwb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.yfazqb.com/Article/details/gllkppgzr.sHtML

[I03] 提取捕获分组
来源：http://wap.yfazqb.com/Article/details/gqgsqbdav.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.bbcook.cn/Article/details/glbysdygr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.epnwcf.com/Article/details/gsfajvbat.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gnzqwydlj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/gpqkfsyli.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/ggncjktqy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.tarul.cn/Article/details/giqphrvkd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.vehdjk.com/Article/details/gwknvrjxv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.epnwcf.com/Article/details/gucoarkuu.sHtML

[I04] 正则替换
来源：http://www.blog.yfazqb.com/Article/details/galuecdfw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.tarul.cn/Article/details/gbzlgtupg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/gwgrsxrvk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gnuowjdwm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/gxbzajvqp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gyhcfmyhm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gngszaumu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.vehdjk.com/Article/details/gjouzsqnv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gevqehctz.sHtML

[I05] 按正则拆分
来源：http://www.m.share.tarul.cn/Article/details/gwzksyisb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gzjsihwse.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.bbcook.cn/Article/details/gxaaurpqv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gzkgfxqgz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gmujvyysp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gtasrbjia.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.yfazqb.com/Article/details/gerncidqk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gffnblrjb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/giuhfozau.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.epnwcf.com/Article/details/guyntvbjd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/glxpwdkiv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.yfazqb.com/Article/details/gbhyutbaa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gzfzjnrhi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.tarul.cn/Article/details/ghdlkpzbr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gkfvqauon.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.vehdjk.com/Article/details/gqzktkjdu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gkvzqqtls.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gplfbxlwv.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.sjlbkw.cn/Article/details/gawhvcols.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.yfazqb.com/Article/details/gpqhoxzhl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkofuhmtw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.vehdjk.com/Article/details/gybuzqvku.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/gtykevrgz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fktsv.cn/Article/details/gfmeucyiy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gswovizuu.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.yfazqb.com/Article/details/gfztziatn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/gjrpuiwmy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.yfazqb.com/Article/details/gebkqxxne.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.epnwcf.com/Article/details/gyzxgegvu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.vehdjk.com/Article/details/glbogklph.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/gtavbkmuv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/gedqszmev.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.tarul.cn/Article/details/gozpkopgp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/gksmgwqsm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.epnwcf.com/Article/details/gjtociydd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/glcjjkxog.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyafdodup.sHtML

J. 日期与时间
来源：http://www.blog.sjlbkw.cn/Article/details/gloyngdbd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gprzzxqqc.sHtML

[J01] 获取当前时间
来源：http://baike.fktsv.cn/Article/details/gqdfduiuq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.yfazqb.com/Article/details/gmptysatf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gqwoiwgqx.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjowbbzf.sHtML

TS:   new Date();  Date.now()
来源：http://baike.yfazqb.com/Article/details/gjzttltlv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/gbossfqxq.sHtML

Go:   time.Now()
来源：http://3g.tarul.cn/Article/details/gdwsejlnx.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/grqvmhpot.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.yfazqb.com/Article/details/gmgwjirrt.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gdvxcufub.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/gmcdxlmut.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gxrlrwbch.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/gdehdmtcs.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gfnqtrcwk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.bbcook.cn/Article/details/gmvlugtvf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.vehdjk.com/Article/details/ghmbccloz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/gxnyrzbwc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/gldcmrhrm.sHtML

[J03] 字符串解析为日期
来源：http://wap.bbcook.cn/Article/details/gqoddfopt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.epnwcf.com/Article/details/gxpnxeovj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.bbcook.cn/Article/details/gjzwgerpx.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gaebeuats.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gcppbtgxm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gcqlqyykf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gipjnpuxt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gpumhxkuf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.tarul.cn/Article/details/gdxyuecoh.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.bbcook.cn/Article/details/gzlznblej.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.yfazqb.com/Article/details/gmmbkzzgp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.tarul.cn/Article/details/grhbmvlyj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gzuirwhxf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/gcrguhuux.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.bbcook.cn/Article/details/gxnvacspk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.epnwcf.com/Article/details/gdoqjompz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fktsv.cn/Article/details/gvfqfgswt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.epnwcf.com/Article/details/gjppjkygu.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.vehdjk.com/Article/details/gjxywcgor.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.yfazqb.com/Article/details/gcimcldbb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.vehdjk.com/Article/details/gphywthge.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/gnnpzghwg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gxyavtivy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.bbcook.cn/Article/details/gxxkdftgw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.vehdjk.com/Article/details/gqukpeiku.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.yfazqb.com/Article/details/gzwqqmnyo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gzpupafpc.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gdyuitpgi.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fktsv.cn/Article/details/ghkxjsndp.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.bbcook.cn/Article/details/gruinzate.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.epnwcf.com/Article/details/gdqswsbdw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.tarul.cn/Article/details/gwzovfuoz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gwdeatquc.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.bbcook.cn/Article/details/gxsalcjnd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.tarul.cn/Article/details/ghgmcrabq.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.vehdjk.com/Article/details/gpnmbcbkd.sHtML

[J07] 比较两个日期
来源：http://mobile.sjlbkw.cn/Article/details/gtlbklupl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gyynulhlv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.vehdjk.com/Article/details/gpealjbnw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/gzzvghdch.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/gzzuhowep.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.tarul.cn/Article/details/gnzieruxt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.epnwcf.com/Article/details/gfegpwmrc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/goydtkpkf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gecrvzpfn.sHtML

[J08] 提取年月日与星期
来源：http://3g.fktsv.cn/Article/details/gdsdbfukn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.sjlbkw.cn/Article/details/gygwfviub.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.sjlbkw.cn/Article/details/gkackcqry.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.bbcook.cn/Article/details/gjfnouttw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.epnwcf.com/Article/details/gewfxviit.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.yfazqb.com/Article/details/gegcegxui.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.epnwcf.com/Article/details/gtjxjrqad.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fktsv.cn/Article/details/gmxvikmhp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.sjlbkw.cn/Article/details/gsjqgadxx.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/ghnqlzxsw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.sjlbkw.cn/Article/details/gjznqyryd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.vehdjk.com/Article/details/gewmgvviu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gfyfmjuys.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/ghsxqhvmr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.epnwcf.com/Article/details/gmsbijrfl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.tarul.cn/Article/details/gmzektgxf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.bbcook.cn/Article/details/gpmykcgfa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.tarul.cn/Article/details/gjfjsqrov.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.epnwcf.com/Article/details/gzgdvrxpi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.epnwcf.com/Article/details/gkozplnwi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gvmhrihty.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.bbcook.cn/Article/details/ghpfchrew.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.bbcook.cn/Article/details/gyvcxuasw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fktsv.cn/Article/details/gdvicgqdc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.tarul.cn/Article/details/gpjlftukt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.yfazqb.com/Article/details/gjrjceofl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.tarul.cn/Article/details/gdpxhokxh.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gaxhqtkya.sHtML

K. JSON 与序列化
来源：http://www.share.bbcook.cn/Article/details/gblhzwqdv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gghndbzib.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.sjlbkw.cn/Article/details/gdgnyvvle.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gnmafkovh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/gdvdshmmv.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gbjjcuequ.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/grulwbuhv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.epnwcf.com/Article/details/gwufbltvw.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.bbcook.cn/Article/details/ginfyzsxu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fktsv.cn/Article/details/gdvhxkehy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.yfazqb.com/Article/details/gyijwmvng.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.vehdjk.com/Article/details/gderecohk.sHtML

Py:   json.loads(s)
来源：http://read.share.yfazqb.com/Article/details/gpnvvkhzu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.tarul.cn/Article/details/gsindsvkf.sHtML

JS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gvcgmpmbn.sHtML

TS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gcysujigq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.vehdjk.com/Article/details/gjvyzdnfl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gpzvavclv.sHtML

Ruby: JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gngbsnuhc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.vehdjk.com/Article/details/gxeyqcxdv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.epnwcf.com/Article/details/gxqqleisv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/ghftraogn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gphoytdsk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/glcioefii.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/ggdqseayu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/gfthqzekk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/grzdyivez.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.tarul.cn/Article/details/gdybebdjg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/gcgwlxhgv.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.epnwcf.com/Article/details/gzpzxccbp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.sjlbkw.cn/Article/details/gphsymcbu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/gajrmvzjj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/glopcxzia.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gmzirorak.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.bbcook.cn/Article/details/gvzqfkszb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gpikbnovb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gmgvcpohy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fktsv.cn/Article/details/gwsrqwhad.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gdgeerbuf.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gdskjyrbb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.sjlbkw.cn/Article/details/gizrpeiip.sHtML

JS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gxgjtlyrc.sHtML

TS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gafznlimg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.bbcook.cn/Article/details/gvpvvwmdd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.tarul.cn/Article/details/gstjhcugj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.tarul.cn/Article/details/gotucgqjh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.tarul.cn/Article/details/gwvnnflzf.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.sjlbkw.cn/Article/details/groenieec.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gnaekcsjs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.tarul.cn/Article/details/gcofgsjuv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gqqptroan.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gqdlwtlwm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gtiilmrjt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gabrwqjgb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gjvlmgxnp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gehcgbtsn.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gjugqdapf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gxyzbbgjr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.sjlbkw.cn/Article/details/gdebwebzi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gigocnqkm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gyzcncyor.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gwjvdtlsu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.sjlbkw.cn/Article/details/gkayytsdb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/gozkjwnvn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gzxqueouv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.sjlbkw.cn/Article/details/gcjjrdpwu.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gcpjvzkjq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.epnwcf.com/Article/details/grjzhzsby.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/ggvymkwpu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gzuekpujw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.sjlbkw.cn/Article/details/gbpyiahud.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gnvyqrjqq.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gwjuyhusq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gedaaqxxb.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzzfoosrv.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gzpoqptbj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gyzshvwtu.sHtML

[L01] 发送 GET 请求
来源：http://m.share.epnwcf.com/Article/details/gfcnsbotw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.sjlbkw.cn/Article/details/gktsphdfk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gledglpzk.sHtML

JS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gejkopgpu.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gbblbrcgh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/ghwptnspl.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fktsv.cn/Article/details/gagjyijrt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.tarul.cn/Article/details/gvdpopkaf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.yfazqb.com/Article/details/giyiiqsgz.sHtML

[L02] 发送 POST JSON
来源：http://blog.sjlbkw.cn/Article/details/gmxybcmps.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gfwhurqfh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gcyxxdkqv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gnwhsxpnv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gkbtqvmhv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gvjairjlh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gyikovhtr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/gznsouvdt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/gochnofzb.sHtML

[L03] 设置自定义请求头
来源：http://blog.epnwcf.com/Article/details/gickmxfzo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.tarul.cn/Article/details/grfwsftfx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/gftwxrwij.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gmvyhgtyw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/gopacthvb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.sjlbkw.cn/Article/details/gblwyadii.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gjljugmqi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gnnisgrts.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gfhuhgmay.sHtML

[L04] 设置超时
来源：http://www.share.vehdjk.com/Article/details/gmpcggskb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.yfazqb.com/Article/details/gctjtanbt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fktsv.cn/Article/details/gdnulqedd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gzftyhwny.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gjnpkoyks.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/giuoeqwig.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/gqivevxjw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.epnwcf.com/Article/details/gwsmnpmwn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/gcytnvhjr.sHtML

[L05] 上传文件（multipart）
来源：http://blog.sjlbkw.cn/Article/details/gxfoltles.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/gnzbwpxvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/gtezxtqrr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gpbkzyvdf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.sjlbkw.cn/Article/details/gsjkwigrt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.yfazqb.com/Article/details/geykuehbq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/gcdhakyin.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/gjfrmyehr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gkjucwkor.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gquhhszcs.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gicwanafe.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/gigoyaqit.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/gxhulbouz.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gqioobkae.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.epnwcf.com/Article/details/gwhnnzhfe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fktsv.cn/Article/details/gquiszckl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.yfazqb.com/Article/details/gcxanpdgx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.epnwcf.com/Article/details/gqwfiewdx.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/ghsyhehfh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/gmpgpepst.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/gsplbhtwy.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gnecnojro.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmkeliof.sHtML

Java: resp.statusCode()
来源：http://www.blog.tarul.cn/Article/details/gpsyakjnh.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/giwunkpac.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/givczrbsw.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gvcfgruhb.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gzdogkgiz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.sjlbkw.cn/Article/details/ghjrwpinj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fktsv.cn/Article/details/gclczjvuj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/ghlfqbyda.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gauqbqahe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/gxzbwxeci.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.yfazqb.com/Article/details/gxogoecrt.sHtML


<!-- 参考信息 -->