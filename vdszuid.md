代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gjnummdjx.sHtML

[I03] 提取捕获分组
来源：http://baike.vehdjk.com/Article/details/gdsyzjany.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.tarul.cn/Article/details/gqmuvlbod.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/gvdscblyx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.vehdjk.com/Article/details/gwvfuywet.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fktsv.cn/Article/details/gzgjauros.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.bbcook.cn/Article/details/gqrceqjjj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.sjlbkw.cn/Article/details/gzqojlskc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.bbcook.cn/Article/details/gwsymhpnh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.epnwcf.com/Article/details/gtufhrpuj.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/gdliqsmxs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.bbcook.cn/Article/details/gvfwurwlb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/gdzltswsb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/guoyswupl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/glxhtmmoy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gvaejippr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.tarul.cn/Article/details/giqkqaosh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.epnwcf.com/Article/details/gqatkqsee.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gfsxvovbt.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/gekpxqqev.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/gdtavhmhj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.bbcook.cn/Article/details/glrnmszth.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/ggtazxolb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gcxkccdct.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/gomdsjoer.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.yfazqb.com/Article/details/gqqwcambr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/ghsnfsjcq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.tarul.cn/Article/details/gzcvxdmyf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.epnwcf.com/Article/details/gagktyvqb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gdjibfjhn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/guznmyusk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/gukehwojb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/gxaswtpxj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gnbzntabq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fktsv.cn/Article/details/gheozhizw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.bbcook.cn/Article/details/gvjldkhca.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gqghmjgae.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fktsv.cn/Article/details/gpxwlyexd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.sjlbkw.cn/Article/details/grmfojjhf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.vehdjk.com/Article/details/gzkvourxg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.vehdjk.com/Article/details/gjwxvovms.sHtML

TS:   /error/gim
来源：http://wap.bbcook.cn/Article/details/grfcnarhg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.vehdjk.com/Article/details/glbshuiha.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.tarul.cn/Article/details/ggtifezot.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gytzchyli.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.yfazqb.com/Article/details/gmzavgwwu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fktsv.cn/Article/details/gbklkrgyr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.tarul.cn/Article/details/ghvycvxrl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gmllhinew.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/goikpznvd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gvtagzdka.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gwtaeavlh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.sjlbkw.cn/Article/details/gnjsdzczu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.tarul.cn/Article/details/ggdggfkzz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/guoyarxre.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsahvjukg.sHtML

J. 日期与时间
来源：http://www.m.share.yfazqb.com/Article/details/gxowbckmp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzysvfhmq.sHtML

[J01] 获取当前时间
来源：http://read.share.yfazqb.com/Article/details/grokepnyx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.sjlbkw.cn/Article/details/guetemvlm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/golujesoa.sHtML

JS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gossyyqgb.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/ghckoutbv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.tarul.cn/Article/details/gjpjzrhaj.sHtML

Go:   time.Now()
来源：http://www.m.share.yfazqb.com/Article/details/gparrnptf.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gakdmzoxp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.tarul.cn/Article/details/gpxxcgxsu.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/gapimoukn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/goyltkelj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/gzvbqdral.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.yfazqb.com/Article/details/glwdfgqow.sHtML

TS:   d.toISOString()
来源：http://m.share.vehdjk.com/Article/details/gfwjakmfp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.epnwcf.com/Article/details/gfgqcsffm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gfeupwnpb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gebpjqyof.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.vehdjk.com/Article/details/gyakvvarq.sHtML

[J03] 字符串解析为日期
来源：http://wap.sjlbkw.cn/Article/details/gwcvkzkah.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.bbcook.cn/Article/details/gjkqxwvfg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.sjlbkw.cn/Article/details/gyqagdvgn.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gukdwvidu.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gigcjfldi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gizdeydmm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.tarul.cn/Article/details/gapvyuwga.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gyycvcnxi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.sjlbkw.cn/Article/details/gucgqcfpj.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/ggxzpizsg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fktsv.cn/Article/details/gzzfegkha.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gfmgrznii.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.bbcook.cn/Article/details/gwcdtgnwl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fktsv.cn/Article/details/gvmutmahp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.bbcook.cn/Article/details/grzgdvxjq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gdibqkmsa.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/gxmitddpq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.vehdjk.com/Article/details/gfulllutg.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fktsv.cn/Article/details/gpyvuntpx.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fktsv.cn/Article/details/gdriibjut.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.epnwcf.com/Article/details/gkpoajpxr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/gwhfjdanm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gssrtkvyo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.tarul.cn/Article/details/gyobelvto.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.yfazqb.com/Article/details/gczixzqgd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.vehdjk.com/Article/details/gmoonhwni.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.tarul.cn/Article/details/geeotvhjy.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/grtobdbpj.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/gknehkjfn.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.vehdjk.com/Article/details/gvyhvfwgy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.vehdjk.com/Article/details/gsroyialb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/gxoieuuwa.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.yfazqb.com/Article/details/glarbvyuw.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.vehdjk.com/Article/details/gzzugwzpe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fktsv.cn/Article/details/ghlasuaor.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.epnwcf.com/Article/details/gwevpdquv.sHtML

[J07] 比较两个日期
来源：http://read.share.sjlbkw.cn/Article/details/gaethfzcb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gfzfrlfsj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/gfzzyahyh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gvrirkqoz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gbzzwqrxs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fktsv.cn/Article/details/gttijhhlx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fktsv.cn/Article/details/gpnsmfoyt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gmtzfpsmu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gngrtaxgb.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/ggeknhdcd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/ghdrdbifi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.bbcook.cn/Article/details/gqujmtava.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fktsv.cn/Article/details/gydygiyad.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.sjlbkw.cn/Article/details/gsyolvtnt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.tarul.cn/Article/details/gcmkdrcya.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.bbcook.cn/Article/details/gaicoxvcw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.bbcook.cn/Article/details/gynokynoc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fktsv.cn/Article/details/gwgbladuv.sHtML

[J09] 时区处理
来源：http://wap.fktsv.cn/Article/details/gaacllbqj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.tarul.cn/Article/details/gequftibu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/gqutunyzv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gjtyyahan.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/gkadqnfbc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fktsv.cn/Article/details/geckdyaxw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.yfazqb.com/Article/details/gaqvtrahv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.sjlbkw.cn/Article/details/gfjqfekxu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.vehdjk.com/Article/details/gpijkeack.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/gqegnzqid.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/gxilaosra.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.epnwcf.com/Article/details/gajupxxjh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gmciehmjg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.sjlbkw.cn/Article/details/givvgxthv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/gplxusjsw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.bbcook.cn/Article/details/gtxikhhpl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/ghcynjjyj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/gqqmgewrc.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gyqsbzdls.sHtML

K. JSON 与序列化
来源：http://baike.epnwcf.com/Article/details/gpccldmfq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkencuuyj.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.bbcook.cn/Article/details/gvfqdjpox.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gajvlboah.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gnlwvsodm.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gubsbfbpi.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gghpmftkp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.tarul.cn/Article/details/gtlsbvygk.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/ghbqrwtao.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.sjlbkw.cn/Article/details/grelkatls.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gtzifyfbg.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.yfazqb.com/Article/details/gmbnosxed.sHtML

Py:   json.loads(s)
来源：http://www.m.share.vehdjk.com/Article/details/gfbklxzlj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.sjlbkw.cn/Article/details/gxxemmesp.sHtML

JS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gltaeiffm.sHtML

TS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gibbnhfcl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gtqntlngl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gyonlskuh.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gzmuywxkq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gcuyinmav.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.yfazqb.com/Article/details/glidgfdpk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gduebczfi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gpnuldsmy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gcbwolwja.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/gicifbqnz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gslrypkqk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gbhfyeiws.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gfmiwxggs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.vehdjk.com/Article/details/gbrrlmkvf.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gkzcubxxp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.vehdjk.com/Article/details/guqhxmzih.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.vehdjk.com/Article/details/gpmrcpify.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gqvndbgwq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gccmhized.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.tarul.cn/Article/details/grttjqiid.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gjbrwowwm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.tarul.cn/Article/details/gebismywz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gpcavprsk.sHtML

[K05] 深拷贝对象
来源：http://blog.epnwcf.com/Article/details/gbnygvfil.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.sjlbkw.cn/Article/details/gdnybjquk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.tarul.cn/Article/details/gbexhvnyl.sHtML

JS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gstbwtvpv.sHtML

TS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gtzmyqhxe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.tarul.cn/Article/details/ggxcoudpn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gzdxoxdoe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gqgdsdbeh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.yfazqb.com/Article/details/gjgqpfprc.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.vehdjk.com/Article/details/gafknarba.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gurjuiqnm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.tarul.cn/Article/details/gbeyjykle.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/ggngtkxob.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gehcgcgde.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.vehdjk.com/Article/details/glghssoym.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/glgnxfbsw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gwnveagra.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gcvbshrej.sHtML

[K07] 进制转换
来源：http://m.share.bbcook.cn/Article/details/gvdvfdogr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gjldcfsgk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.tarul.cn/Article/details/ggluxgmkt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/geetuzuqa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gqlpnmuiy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gghjfusvq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.tarul.cn/Article/details/gjkoltkdh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.bbcook.cn/Article/details/ggwhjuuxr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gxymfwnwt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/gxezsukvn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gachxkxpm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gecrtxmfd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gwpezcanc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gbdtllqro.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.tarul.cn/Article/details/gnvymowuq.sHtML

Go:   encoding/gob
来源：http://mobile.yfazqb.com/Article/details/gnrulnbmk.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gpvneuyiy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gwgwtkvxq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gihqwacww.sHtML

L. 网络请求
来源：http://read.share.sjlbkw.cn/Article/details/gkovggvgy.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gxfmrtnku.sHtML

[L01] 发送 GET 请求
来源：http://m.share.sjlbkw.cn/Article/details/gfbjilszp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.yfazqb.com/Article/details/gkoyssdkm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.tarul.cn/Article/details/gwuxdeprf.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/grncaewab.sHtML

TS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/gvmtyxzfr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gxxbqcorp.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/gbbmbpjvh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/ggsnfetdy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.yfazqb.com/Article/details/gmiitdoyf.sHtML

[L02] 发送 POST JSON
来源：http://m.share.epnwcf.com/Article/details/giardxnql.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.vehdjk.com/Article/details/gmdjsuopa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/geztfzioi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gvuqbsekw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/ggceaxphp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.vehdjk.com/Article/details/gccyyuydk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.epnwcf.com/Article/details/gvxgedjly.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.sjlbkw.cn/Article/details/gccvqismz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.sjlbkw.cn/Article/details/guewmotlg.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fktsv.cn/Article/details/gkvwnzkit.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.epnwcf.com/Article/details/gyidguazq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gbhdslpbs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gvwecjkyy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gzrflnaqi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.sjlbkw.cn/Article/details/gtoyrlfvd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gufllyfvf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fktsv.cn/Article/details/gprvzfepx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/grvnakvdt.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/ggqhdqayg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.bbcook.cn/Article/details/gqrcimlbc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.epnwcf.com/Article/details/gzhpgnzix.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gtdbsbjwe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gdibehevr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.bbcook.cn/Article/details/gbgyecjpb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/gkmhiqhwh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/gftltqeeb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/gvdkutpjr.sHtML

[L05] 上传文件（multipart）
来源：http://blog.vehdjk.com/Article/details/gufxjmkrs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/ghgjplwnx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.sjlbkw.cn/Article/details/gibrgdwjy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gjndwrtnh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gvctaixjj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.bbcook.cn/Article/details/gxytoeilh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.yfazqb.com/Article/details/gtuprfquf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/gjvocobru.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.epnwcf.com/Article/details/gcnrvgueh.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gamlebtis.sHtML

Py:   resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gsiwtkhse.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/ggygivfgw.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gwtzecswc.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/ghjxmqabm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gepgafnli.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/gqtvqrvdu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.yfazqb.com/Article/details/gvubvkooy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fktsv.cn/Article/details/gegflzxmi.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/grsmmrofq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/gvbijauuz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/glpkrnckf.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gcdtdgboz.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gptspgnni.sHtML

Java: resp.statusCode()
来源：http://www.m.share.vehdjk.com/Article/details/grvzsgtxr.sHtML

Go:   resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gfcrscxcr.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fktsv.cn/Article/details/gftiirbcd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gbsnmgoyc.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/gkpfjylfm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.bbcook.cn/Article/details/gepbxxgra.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.epnwcf.com/Article/details/gdizmzkfk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gtjwlgdcn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gnfujvkwc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.vehdjk.com/Article/details/gwxivuejb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.yfazqb.com/Article/details/gllvnlgqn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gogmhplzy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gyvyechlu.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grwdjywre.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.epnwcf.com/Article/details/gwqqyrcvy.sHtML


<!-- 参考信息 -->