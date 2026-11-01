代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.bbcook.cn/Article/details/gfknwysbc.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.yfazqb.com/Article/details/gitoggiiv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.yfazqb.com/Article/details/gqbzxzneh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gyasiennl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fktsv.cn/Article/details/gzdgtjefc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.vehdjk.com/Article/details/guyxsnnhp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.sjlbkw.cn/Article/details/gpkqfzewu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.vehdjk.com/Article/details/ghrqcpxrm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.epnwcf.com/Article/details/gdrbhwtwj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.yfazqb.com/Article/details/gqsaepdvk.sHtML

[I04] 正则替换
来源：http://www.blog.yfazqb.com/Article/details/ggqvehiqa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.yfazqb.com/Article/details/gjgxsgeap.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gmlmbcxwz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gbrlwrfta.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/gxwjgyohg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gpnhcellg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.epnwcf.com/Article/details/gbckjkesm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fktsv.cn/Article/details/gldihjmpa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gdbsyrcdq.sHtML

[I05] 按正则拆分
来源：http://baike.yfazqb.com/Article/details/ggrsqjmsv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.vehdjk.com/Article/details/gkspxvvlw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fktsv.cn/Article/details/ghycbcvvl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gmbxqyrrr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gprsbgbxy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.bbcook.cn/Article/details/ganmroezq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/glbanolbk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gexrqopgx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/gkspppkgj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/gznlktxdh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/guvdmlkwl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.bbcook.cn/Article/details/gawyywyku.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/guodztebl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/gsodwwmyr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gbctmpigf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fktsv.cn/Article/details/ghaoagdbc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.tarul.cn/Article/details/gpnrhdueh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gutljjmsx.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.vehdjk.com/Article/details/gwxejmwcg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fktsv.cn/Article/details/gzzlmbvbi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gbmnbbhli.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.vehdjk.com/Article/details/gpdmhejkz.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/ggmtmaqse.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.sjlbkw.cn/Article/details/gninkmauz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/grqjxuefa.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.bbcook.cn/Article/details/gabjlebzy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gjprhbpka.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.bbcook.cn/Article/details/gkornqtwl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fktsv.cn/Article/details/goopeyoue.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gsbugvqnq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gnzahpmdc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gojxouqva.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/ggbxayiiy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.epnwcf.com/Article/details/gzyfuqghz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.vehdjk.com/Article/details/gjlcnxxsq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gytrjjyjd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmbaoijla.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gromskkyq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/guglryitt.sHtML

[J01] 获取当前时间
来源：http://read.share.vehdjk.com/Article/details/geqsmisju.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.yfazqb.com/Article/details/gqjbefohe.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/gqzemyedo.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.vehdjk.com/Article/details/gdrlahdcx.sHtML

TS:   new Date();  Date.now()
来源：http://wap.tarul.cn/Article/details/gxwzrdrth.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.sjlbkw.cn/Article/details/gyekbnqjs.sHtML

Go:   time.Now()
来源：http://mobile.sjlbkw.cn/Article/details/gmjyyinyr.sHtML

Ruby: Time.now
来源：http://mobile.tarul.cn/Article/details/giktgsgfk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.yfazqb.com/Article/details/gjovfdman.sHtML

[J02] 格式化输出
来源：http://wap.fktsv.cn/Article/details/gidxmxdpi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gmzifcbxz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gauwhtdji.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.vehdjk.com/Article/details/gubffkrry.sHtML

TS:   d.toISOString()
来源：http://www.m.share.epnwcf.com/Article/details/gwryzrmkt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnccmspm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.tarul.cn/Article/details/guqxjcdze.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gfsxoahty.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.sjlbkw.cn/Article/details/gmoftezjj.sHtML

[J03] 字符串解析为日期
来源：http://wap.vehdjk.com/Article/details/ggegbkkti.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.bbcook.cn/Article/details/glhabarkp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.sjlbkw.cn/Article/details/gbanoygns.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gflqpdqae.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gthvrqmaa.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gdlaobeqd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gipvhxoos.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gjomqmffx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.epnwcf.com/Article/details/gloxatqub.sHtML

[J04] 时间戳与日期互转
来源：http://wap.tarul.cn/Article/details/gnidjhhzx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.epnwcf.com/Article/details/gophvvagx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.vehdjk.com/Article/details/gympuoefz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/ghgglyiam.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.yfazqb.com/Article/details/ggqoifycr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gcwrhnkic.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gibqkmmxd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.epnwcf.com/Article/details/gsopfrund.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fktsv.cn/Article/details/ghizukuez.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fktsv.cn/Article/details/gwtnkocea.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.bbcook.cn/Article/details/ggtudkser.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.epnwcf.com/Article/details/gjebodjwa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gsbmfmsua.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/glittlcwx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.vehdjk.com/Article/details/glbqemwgy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/gtftmizcg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.epnwcf.com/Article/details/grhfupuhl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.vehdjk.com/Article/details/ggimrogtf.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.bbcook.cn/Article/details/gnfwjcpol.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.sjlbkw.cn/Article/details/gsggqvzwy.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlzwntsk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.sjlbkw.cn/Article/details/geiwexffx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.sjlbkw.cn/Article/details/gnxgsujqb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.bbcook.cn/Article/details/gkhgjklpw.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.vehdjk.com/Article/details/gwuyhzqpt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.yfazqb.com/Article/details/ghofikmfp.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/gplrejmwq.sHtML

[J07] 比较两个日期
来源：http://www.share.vehdjk.com/Article/details/grptejrbi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/ggwrcumvh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fktsv.cn/Article/details/gfkftooeu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/giwvijjvo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gvjtvswyd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.epnwcf.com/Article/details/gfyszpuod.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gyybyitfp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gwsoereuy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gjxicvkcu.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gxesidnwn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.sjlbkw.cn/Article/details/geunfvtke.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/gtvvmnmci.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.epnwcf.com/Article/details/gzxnpggtv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.bbcook.cn/Article/details/gkzzuhaaq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.bbcook.cn/Article/details/gbarpdgrh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.epnwcf.com/Article/details/gpveddxra.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.sjlbkw.cn/Article/details/gzqkkbgbp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.epnwcf.com/Article/details/ggknsdmua.sHtML

[J09] 时区处理
来源：http://3g.fktsv.cn/Article/details/glahhdgyh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.sjlbkw.cn/Article/details/ghgcpkhdw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.bbcook.cn/Article/details/gomquznmr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/ghdtphfpq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/grdgmixwi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.tarul.cn/Article/details/giheewhhj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.vehdjk.com/Article/details/gymiacyln.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.vehdjk.com/Article/details/gtjlcqlqp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gxpwcxdwy.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/gbtdcpafv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.sjlbkw.cn/Article/details/gsuwlzvhf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/gucaecfua.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fktsv.cn/Article/details/ghcyvqalt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.vehdjk.com/Article/details/gdlafavps.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.sjlbkw.cn/Article/details/ghsbbnisu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fktsv.cn/Article/details/gangfuhrk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.yfazqb.com/Article/details/grpjmakgn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.vehdjk.com/Article/details/gqycqlcfk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtrmtyuzp.sHtML

K. JSON 与序列化
来源：http://www.m.share.vehdjk.com/Article/details/gtyghgbgv.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gaiawgkxu.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.bbcook.cn/Article/details/ggsvmfjfi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/grgkvhbhr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gqzynjygy.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gfniqwwpm.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gmeiinoor.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.epnwcf.com/Article/details/gmxansoph.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gzrmvldfo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.vehdjk.com/Article/details/gckrnzvob.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fktsv.cn/Article/details/gxtnssfhu.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.bbcook.cn/Article/details/gcisqoxfi.sHtML

Py:   json.loads(s)
来源：http://m.share.sjlbkw.cn/Article/details/gvpxfnrgt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gxdnahayz.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gxunchqwo.sHtML

TS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gzrgvcrxo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.vehdjk.com/Article/details/ganygtksp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/ggijendlv.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/guvtohulm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.bbcook.cn/Article/details/gzosxoccz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.bbcook.cn/Article/details/goqyrgycf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/ggilgmsnt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/girdpggih.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/glplmhawu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gvlrhmjxd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.epnwcf.com/Article/details/gyhkhxfww.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.tarul.cn/Article/details/gvjsqroyh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.yfazqb.com/Article/details/gdlosylgg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.epnwcf.com/Article/details/gshnnjata.sHtML

[K04] 读取 JSON 文件
来源：http://blog.bbcook.cn/Article/details/gawukhrcu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.yfazqb.com/Article/details/gnduuvfcm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.tarul.cn/Article/details/gknpbmneq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gssgiwedi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gqdzuoqsb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gpheyixzl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gyipxajxt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggixtkjvz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gbsdwhgmp.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/geobqqire.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.vehdjk.com/Article/details/gosmzhlhn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fktsv.cn/Article/details/gyzqkqpoc.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gnkanvwwn.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/ggdhsdlxk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/gyjzrvhjn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.tarul.cn/Article/details/gebpnrfnw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.tarul.cn/Article/details/gboauzucw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.bbcook.cn/Article/details/gkyrmiicg.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.tarul.cn/Article/details/gdxvzppib.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gzlwicdew.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.epnwcf.com/Article/details/glywydabx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gtzjrhqke.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gidrfgddd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.sjlbkw.cn/Article/details/grceuedkd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gkslgzxme.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gddzxkbgn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gqmddljau.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gaxtifnbd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/ggtfntwqm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/gioeasund.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gjmyvyzlc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/goinejmqb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gphepdnhh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/gehquftup.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/guqmrynkj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gmihodlkt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.bbcook.cn/Article/details/gpafnojxs.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/glmksfkcc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.bbcook.cn/Article/details/gtsxfbnbm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gnlynqsxg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gdrtdjrdv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/gddpovekh.sHtML

Go:   encoding/gob
来源：http://m.share.fktsv.cn/Article/details/goeosahtf.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.epnwcf.com/Article/details/gnyaubgdf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gcuslscuy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gifjhlmbw.sHtML

L. 网络请求
来源：http://read.share.fktsv.cn/Article/details/ghhzxtyor.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gfuvrjpgq.sHtML

[L01] 发送 GET 请求
来源：http://3g.yfazqb.com/Article/details/guzmzuito.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.epnwcf.com/Article/details/gicdvavgm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.tarul.cn/Article/details/ggloiwmja.sHtML

JS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gkzfmbomn.sHtML

TS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/ggwwecuwn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/guahzoggf.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/gbdmevvmz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/ggydypfzf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/geefevlae.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/guiszwnum.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.yfazqb.com/Article/details/gvtehalmk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.sjlbkw.cn/Article/details/gxurenhll.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/ghfqxvmle.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/gjsnhwced.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtuasdet.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gxqvuuajf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.tarul.cn/Article/details/gfaelivzg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.vehdjk.com/Article/details/gowrybsgv.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gwulxqmbu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.yfazqb.com/Article/details/glrdjvqdz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/gajoifjcu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gtwftwetp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/grutkcefq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/gjqgmakzp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/grkuuofry.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/geyaijalq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/glywigwmd.sHtML

[L04] 设置超时
来源：http://www.share.epnwcf.com/Article/details/gtbqscsez.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.sjlbkw.cn/Article/details/gfqxvqphm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fktsv.cn/Article/details/glfgeikbg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/geypqdeyz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gucnxolgh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fktsv.cn/Article/details/gzeubcsfy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.tarul.cn/Article/details/gomzudlud.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.vehdjk.com/Article/details/gimcaweus.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/gidzmpzhw.sHtML

[L05] 上传文件（multipart）
来源：http://3g.vehdjk.com/Article/details/gzuehqjyf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/gclbomtoq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/ghkonvihy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gmhseaawh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gbumknixc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.yfazqb.com/Article/details/gtjiglrbn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/gpqtdbmjp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.sjlbkw.cn/Article/details/gpqqgszop.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/gdrsrygkt.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/ggxhcdayo.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gvosgilkz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/gpfnerfuc.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gurcfgjja.sHtML

TS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gwopvlubu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gacahyyfy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fktsv.cn/Article/details/gvpbtgysu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/gqslmaged.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.vehdjk.com/Article/details/gmjvwkljn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gbymynaex.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.bbcook.cn/Article/details/gkpvrccsy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.tarul.cn/Article/details/grdwusxsr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gcdrdqdpo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gzcspmycq.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/guvmnkaql.sHtML

Go:   resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gshdzwoqz.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/gkxedynwc.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/grczfkupx.sHtML

[L08] 并发请求多个地址
来源：http://wap.bbcook.cn/Article/details/gzwduwjuv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gfnpckxnv.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.vehdjk.com/Article/details/gmqtlhrfg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/grtnftlqx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gonrywjjh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fktsv.cn/Article/details/gaivzuljc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gdnjwnchl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/gkrrsukzv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.tarul.cn/Article/details/gvigjjaji.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ggflkpnqd.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/gyoykvzie.sHtML


<!-- 参考信息 -->