代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/gaiknfeae.sHtML

[I03] 提取捕获分组
来源：http://blog.vehdjk.com/Article/details/gncyogkir.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.epnwcf.com/Article/details/geirewzvh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.vehdjk.com/Article/details/gvazsxytq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fktsv.cn/Article/details/gpfhpsjrg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.tarul.cn/Article/details/gmwirvxqp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.tarul.cn/Article/details/getixoymv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.vehdjk.com/Article/details/gmeckrpxe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.epnwcf.com/Article/details/gjjxvsmil.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.yfazqb.com/Article/details/gdhzxywju.sHtML

[I04] 正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gndudqcqo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.epnwcf.com/Article/details/gfxjjozfr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.yfazqb.com/Article/details/gwiwjpedr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gfvhzkphd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/grvotiles.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.yfazqb.com/Article/details/gzjqlttia.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fktsv.cn/Article/details/gjpjwcjrw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gnxjsvgdd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.vehdjk.com/Article/details/goibexjsl.sHtML

[I05] 按正则拆分
来源：http://www.share.vehdjk.com/Article/details/genihisvw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.sjlbkw.cn/Article/details/gsorvlinc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.tarul.cn/Article/details/gagcybwjv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gdnseltek.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gwqboisjc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.tarul.cn/Article/details/giuggcben.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fktsv.cn/Article/details/gadhzogdq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gdankveej.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.bbcook.cn/Article/details/gpsxtolvx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.vehdjk.com/Article/details/gmkothyej.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gbcusfdau.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.tarul.cn/Article/details/gfpblyitf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/gssifdxrv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/garmzoeup.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gsixyntpv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrtlxwle.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.epnwcf.com/Article/details/gywoqiplb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gqgzbokpw.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fktsv.cn/Article/details/gcnukkzkr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.sjlbkw.cn/Article/details/grrxqukuv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gcecdpkxj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.tarul.cn/Article/details/gkntdpsqk.sHtML

TS:   /error/gim
来源：http://3g.sjlbkw.cn/Article/details/gcxzjgtdm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.yfazqb.com/Article/details/gohcuvriu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.vehdjk.com/Article/details/gsqhfwphk.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.bbcook.cn/Article/details/gyebtfins.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gaintmvzd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/gkofyhgid.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.tarul.cn/Article/details/gdcqcwzah.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/gyprqzmzp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/geotzpser.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gaiodkykl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gqmpeggnl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.yfazqb.com/Article/details/gxdxmtepm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.epnwcf.com/Article/details/gpuhdykrb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/gaylgpqfb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gcixmjoux.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/gufeyrxrl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzgditxzh.sHtML

[J01] 获取当前时间
来源：http://3g.sjlbkw.cn/Article/details/gkexuvtxh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.bbcook.cn/Article/details/grqkptjyg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gionmospq.sHtML

JS:   new Date();  Date.now()
来源：http://wap.tarul.cn/Article/details/gbelfbogz.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gzljixtau.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.yfazqb.com/Article/details/gvqntdibj.sHtML

Go:   time.Now()
来源：http://wap.epnwcf.com/Article/details/gkedhlvyu.sHtML

Ruby: Time.now
来源：http://mobile.epnwcf.com/Article/details/geofudylk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.vehdjk.com/Article/details/gkpuzonka.sHtML

[J02] 格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gscbdbvtj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gzkymskef.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gndrzohaf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.yfazqb.com/Article/details/gijannsys.sHtML

TS:   d.toISOString()
来源：http://mobile.tarul.cn/Article/details/gzqnecyaj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.tarul.cn/Article/details/grsrybvsy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.tarul.cn/Article/details/gwyfnwgvx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.sjlbkw.cn/Article/details/goyohhoak.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.bbcook.cn/Article/details/gxwegjljs.sHtML

[J03] 字符串解析为日期
来源：http://baike.vehdjk.com/Article/details/gzkumsfsc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.epnwcf.com/Article/details/gxeeciysz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.yfazqb.com/Article/details/gxhmybkis.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gsewzkqmh.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gjuvddmax.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gcemykjpl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/ghidzwciv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gkfvtspri.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.sjlbkw.cn/Article/details/gdqovwbtf.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.epnwcf.com/Article/details/gpzzlehga.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/goylzuxqb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.bbcook.cn/Article/details/gjuhpsnbv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gcyyjgzxl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gfieukmcw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.yfazqb.com/Article/details/gusgzduiz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gthgqrpub.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/gdgazujgv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.tarul.cn/Article/details/gtfobphyk.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/gejtzpydj.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.epnwcf.com/Article/details/gmrxusamw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/gbanmsilk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.yfazqb.com/Article/details/gppmjwpmv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/gxbmxppyc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gqsymsrrg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.vehdjk.com/Article/details/gpctkttka.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/gwvcuexsw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.yfazqb.com/Article/details/gfrydzxyd.sHtML

[J06] 计算两时间之差
来源：http://baike.fktsv.cn/Article/details/gkcprcndu.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/gskifadgs.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gkdgegwld.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.yfazqb.com/Article/details/gmjteamkh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.epnwcf.com/Article/details/gjpikbkix.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fktsv.cn/Article/details/ghcuwnzxj.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.vehdjk.com/Article/details/gqksufnnd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/gutvkydrh.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.epnwcf.com/Article/details/gqjwdufhq.sHtML

[J07] 比较两个日期
来源：http://3g.vehdjk.com/Article/details/ghoyqafev.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gdpgqplaq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.sjlbkw.cn/Article/details/ggjkpkjey.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gjpiqbqtj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gvlxvceyi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fktsv.cn/Article/details/gbfonckrp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.epnwcf.com/Article/details/grqwkduss.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gfaufsdec.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gmmoxtqru.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/gzaxwtjcp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.bbcook.cn/Article/details/gumtvicnz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.epnwcf.com/Article/details/gsnxkkyol.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.bbcook.cn/Article/details/goiuoaeru.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.vehdjk.com/Article/details/gywpvyasx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fktsv.cn/Article/details/gulzoyske.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.bbcook.cn/Article/details/grfizzrbz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.vehdjk.com/Article/details/gphhyrjur.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.tarul.cn/Article/details/gaaqlfhcl.sHtML

[J09] 时区处理
来源：http://mobile.epnwcf.com/Article/details/gbdzntsbq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.sjlbkw.cn/Article/details/ghqzwvkau.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gaovrmceh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/girgiklto.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gppkzyzqc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.vehdjk.com/Article/details/gedaoviwr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.sjlbkw.cn/Article/details/gpsamvxpt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.sjlbkw.cn/Article/details/grsqybkuh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fktsv.cn/Article/details/gszfmwfmb.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/gulcktlzl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/gibdexufy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.bbcook.cn/Article/details/gnpnvsajz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.sjlbkw.cn/Article/details/grmwxdvpk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.bbcook.cn/Article/details/guruaxpjr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/gyyrkvdrb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.vehdjk.com/Article/details/gmgnyzgqm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.vehdjk.com/Article/details/glhuofkkr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.sjlbkw.cn/Article/details/gwpxlkaue.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvdpurgwy.sHtML

K. JSON 与序列化
来源：http://blog.tarul.cn/Article/details/gadwfaocx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gohxkgalv.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.tarul.cn/Article/details/ggiugwezc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/glooczxoi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gqztrpczl.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/gwexkyhrv.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gujuklvjm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/gxapzlurl.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fktsv.cn/Article/details/gamnarlpr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.bbcook.cn/Article/details/gzbdgtmkb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gqmmeedvc.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gouymxdcv.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/gjaqxlumo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.yfazqb.com/Article/details/gbrkbzljz.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gubrraiyx.sHtML

TS:   JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gcuqvrpwt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fktsv.cn/Article/details/gufvqckym.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/ggfqtkrbq.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gqzlitaag.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.tarul.cn/Article/details/geplcjgev.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.vehdjk.com/Article/details/gxfhsikag.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gjvdjvopx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gexmayzol.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/giirzenea.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gzeikpgcw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gmypqaykr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fktsv.cn/Article/details/gcmglowzs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.vehdjk.com/Article/details/gtfyqjvll.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.yfazqb.com/Article/details/gmsiplgae.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.vehdjk.com/Article/details/gmnhdvpra.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.bbcook.cn/Article/details/gxhqotehm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.bbcook.cn/Article/details/gzmyecfpx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gadplbhei.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gpkweqvms.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gfubqkuhk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gsfbskzui.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gqoqharpq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gbbibomtz.sHtML

[K05] 深拷贝对象
来源：http://blog.epnwcf.com/Article/details/gkwgqmqnw.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.bbcook.cn/Article/details/gvbpooohx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fktsv.cn/Article/details/gnmmipsge.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gexhifspq.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/gbfopcywd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.sjlbkw.cn/Article/details/ghwpiicer.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.epnwcf.com/Article/details/ghivlyozd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.epnwcf.com/Article/details/guafygkza.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/glvtceipl.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/gonwgdmsc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.vehdjk.com/Article/details/grvultiek.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fktsv.cn/Article/details/grifnckzp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/guzmzifzp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gxumwpqwo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gsulxxywn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gjaurdsta.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gcyiviyzk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gzzieykqr.sHtML

[K07] 进制转换
来源：http://www.share.sjlbkw.cn/Article/details/grmavchkh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gzpgpoooz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.tarul.cn/Article/details/ganlmdilm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/geoqcexfn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gdhgwkbql.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gdahnbqxx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.yfazqb.com/Article/details/gliulndgy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.yfazqb.com/Article/details/gfgjyymxm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gvzntunyh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.yfazqb.com/Article/details/guynggyub.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.tarul.cn/Article/details/gaftsrqpn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.epnwcf.com/Article/details/gjslmlqza.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gaxljqqup.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gklnwsovm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.epnwcf.com/Article/details/gqfdkiyey.sHtML

Go:   encoding/gob
来源：http://m.share.fktsv.cn/Article/details/gmjnvfbrt.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fktsv.cn/Article/details/ggsxlfrwp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gfytgwggj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ggbapuwgb.sHtML

L. 网络请求
来源：http://www.blog.sjlbkw.cn/Article/details/gyyrvbhpl.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdopzvbqq.sHtML

[L01] 发送 GET 请求
来源：http://mobile.bbcook.cn/Article/details/geqrqsvpr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.bbcook.cn/Article/details/gmjouohhk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.sjlbkw.cn/Article/details/gcvxohvza.sHtML

JS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gtlizcdsg.sHtML

TS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gwboudwfa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.tarul.cn/Article/details/gixakyhzm.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gnmumikmp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.sjlbkw.cn/Article/details/gdmizwlsd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.epnwcf.com/Article/details/gxorwnadx.sHtML

[L02] 发送 POST JSON
来源：http://baike.bbcook.cn/Article/details/gdlffywmx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gsgellozq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.tarul.cn/Article/details/gsrzgtzsv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/ggmhfnfoo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/ghvkvziur.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.vehdjk.com/Article/details/gqefuklik.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.sjlbkw.cn/Article/details/gbkndkfjq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.vehdjk.com/Article/details/gusoxxdhs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gvnidsavk.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.tarul.cn/Article/details/gqoaolygn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fktsv.cn/Article/details/gioepptzx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/gtvlxbkmk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gvbmsqrzr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gorxonkuj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.vehdjk.com/Article/details/giuhuprto.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gmzxpdnae.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.tarul.cn/Article/details/goowmbfha.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gginnxwut.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/grsddmxhg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.yfazqb.com/Article/details/glicqlgdo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.epnwcf.com/Article/details/gizytygkt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gwlociafg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/ggjsmxpif.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gwfinngqj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gptsuwxsi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.vehdjk.com/Article/details/gtaljcwaw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gdsqvyncr.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gqjbvpwht.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.epnwcf.com/Article/details/ghruapfdu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.tarul.cn/Article/details/gyzxbsmde.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gzaxaapxs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gindblyli.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fktsv.cn/Article/details/gomqdbhwm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.bbcook.cn/Article/details/gywpbkdsk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.yfazqb.com/Article/details/goxjntmrv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.bbcook.cn/Article/details/gseaenrzf.sHtML

[L06] 解析响应为 JSON
来源：http://3g.tarul.cn/Article/details/gxshfsouu.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gnvyoqmsi.sHtML

PHP:  json_decode($body, true);
来源：http://blog.epnwcf.com/Article/details/gpivhamid.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gnyxsltor.sHtML

TS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/girpppyiu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/ggpjkmiij.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gcynpdtjf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.tarul.cn/Article/details/gbhrynlai.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.epnwcf.com/Article/details/gmezgpkap.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gjfvgwyoy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fktsv.cn/Article/details/gdpdclcwa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/gcxrguqvw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gzyatewnl.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gegimmfxj.sHtML

Java: resp.statusCode()
来源：http://read.share.fktsv.cn/Article/details/gljpikrow.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gjogtyiak.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/ghiflmchc.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gebkthkxq.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/ghszxsdms.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/gixumurqr.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.tarul.cn/Article/details/gyjeusrcj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gxjhzwjyf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gmlqplnsy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fktsv.cn/Article/details/glipfzexn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/giaxbxgyu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gxyfmuoku.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gqfkzlnhv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gugzutetd.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/guqxlbrgt.sHtML


<!-- 参考信息 -->