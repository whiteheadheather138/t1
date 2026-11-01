代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fktsv.cn/Article/details/gnrajmugv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.vehdjk.com/Article/details/gymxjqrgh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fktsv.cn/Article/details/ghktloshd.sHtML

[I05] 按正则拆分
来源：http://3g.yfazqb.com/Article/details/gdlmvqsdy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.sjlbkw.cn/Article/details/gpmsrgevp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.vehdjk.com/Article/details/gnccmlxfk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gkmwatkkx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gjmohycvb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.epnwcf.com/Article/details/grmgantir.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.tarul.cn/Article/details/ghhbadlse.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gzgqjqyep.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.epnwcf.com/Article/details/gwafxgiqn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/gurzsvdlz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/giksdbstw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/gpyadopju.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/gcxidflyb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gwiqdhwaw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gjiaakwzx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.bbcook.cn/Article/details/gqbhhtuvt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.bbcook.cn/Article/details/ghurxynig.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gbaddtfhm.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.tarul.cn/Article/details/gxryycnij.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gxobxoaxn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.yfazqb.com/Article/details/geotnpcpq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.sjlbkw.cn/Article/details/gsawhegai.sHtML

TS:   /error/gim
来源：http://mobile.bbcook.cn/Article/details/gfgmprtuc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fktsv.cn/Article/details/gbtfglhse.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.sjlbkw.cn/Article/details/getipledt.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.vehdjk.com/Article/details/gbudoxmac.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.sjlbkw.cn/Article/details/gvxashxss.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.tarul.cn/Article/details/gososukma.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.yfazqb.com/Article/details/gtkxoljlo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gsirjgotb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gtxlsjuhg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gyrxwunyy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/ghbunynwh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.epnwcf.com/Article/details/gvykpgbxg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/gumwuqmie.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/gzlkgblfm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/guitmsvjq.sHtML

J. 日期与时间
来源：http://read.share.yfazqb.com/Article/details/gnvekvedv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gmjoelvlg.sHtML

[J01] 获取当前时间
来源：http://m.share.vehdjk.com/Article/details/gmhrkhtyi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.tarul.cn/Article/details/gumdihmlj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/gqqvwldgd.sHtML

JS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gbecwbhvc.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gozfgafmx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.sjlbkw.cn/Article/details/geayfmhcc.sHtML

Go:   time.Now()
来源：http://read.share.yfazqb.com/Article/details/gkfpwjvia.sHtML

Ruby: Time.now
来源：http://read.share.bbcook.cn/Article/details/gtedbcgmq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.epnwcf.com/Article/details/gdmcjnzio.sHtML

[J02] 格式化输出
来源：http://m.share.vehdjk.com/Article/details/gubadxfub.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gwberuums.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gowyzlxid.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.yfazqb.com/Article/details/gwcselfjk.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/gbcwltqcq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.yfazqb.com/Article/details/guipnbmgc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.tarul.cn/Article/details/gezrybakb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/ggfxqpnhr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.bbcook.cn/Article/details/goqnxazhv.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.vehdjk.com/Article/details/gbefxhatz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.bbcook.cn/Article/details/glvbtquwo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.sjlbkw.cn/Article/details/guihgxppy.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gabiavcuz.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gzyrwqmbr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gsqlwhcxx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/ggfxatzmm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gczbdbxxu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.epnwcf.com/Article/details/goqlabcac.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fktsv.cn/Article/details/gklkdkjzk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.sjlbkw.cn/Article/details/gdxosyqlr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.sjlbkw.cn/Article/details/gxdexshdx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.tarul.cn/Article/details/gxfbmoztg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.epnwcf.com/Article/details/gnfgolonv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.bbcook.cn/Article/details/giipvblyh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.yfazqb.com/Article/details/glphfxvah.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.vehdjk.com/Article/details/giuhgqkge.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.sjlbkw.cn/Article/details/gsrbvgyzh.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.tarul.cn/Article/details/gdrormhzf.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.epnwcf.com/Article/details/gafbfxhwx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fktsv.cn/Article/details/gyctoklwq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fktsv.cn/Article/details/gdyyubcwn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/grwkqmyss.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fktsv.cn/Article/details/gikveikan.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/gatqjcbjj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fktsv.cn/Article/details/gyiqgdbab.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.vehdjk.com/Article/details/ghzgyeuod.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/guprlsdjw.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/gghnazqrz.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.bbcook.cn/Article/details/gcendurpk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.epnwcf.com/Article/details/geslockiw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fktsv.cn/Article/details/gqcpvrzeq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.vehdjk.com/Article/details/gekcidyur.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fktsv.cn/Article/details/ghbofyzwb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/gfxuaabso.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.sjlbkw.cn/Article/details/ggtdpcydn.sHtML

[J07] 比较两个日期
来源：http://mobile.fktsv.cn/Article/details/gyqsrtgzk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gqddnaxku.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.bbcook.cn/Article/details/gzbxebzbn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gnfkrtetw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/gwtuevkpx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.bbcook.cn/Article/details/gwerkkavo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gpazptibz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/groozzqhz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gaafzaeza.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fktsv.cn/Article/details/gvtaotszh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.bbcook.cn/Article/details/gttzokccm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fktsv.cn/Article/details/ggkyxqifw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/gvvtmyqdm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.sjlbkw.cn/Article/details/gpeoyjjwg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fktsv.cn/Article/details/gxploqnpq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.yfazqb.com/Article/details/gfvqagoio.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.vehdjk.com/Article/details/gxnglxjpx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.yfazqb.com/Article/details/gapvjzqre.sHtML

[J09] 时区处理
来源：http://3g.yfazqb.com/Article/details/gbgybekkk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.yfazqb.com/Article/details/ggrmpgadg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.sjlbkw.cn/Article/details/gupgwevag.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gwmzrxpeh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/grwmkgiyv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.sjlbkw.cn/Article/details/gwgzrsmvz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.bbcook.cn/Article/details/gjsohemes.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.vehdjk.com/Article/details/gnnstxqid.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.bbcook.cn/Article/details/gutaxegak.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.tarul.cn/Article/details/gnrzpzojj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/ghtjwpnvg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.vehdjk.com/Article/details/gmqtmtqid.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/gssmdezbz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.tarul.cn/Article/details/grucnjlmz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fktsv.cn/Article/details/gakzzqvdg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.sjlbkw.cn/Article/details/gfkrstbdk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.epnwcf.com/Article/details/gjmtgoyac.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.yfazqb.com/Article/details/gzjfjuezb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdvpbhpge.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gspztziym.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gubxkpztq.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/gcjthzrdr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gfihmjwrv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/gwnggubgw.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/gqelkkcpl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/ggpzjhuxh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/gkelvlexb.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.bbcook.cn/Article/details/gssajuxyo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gpyiimcbp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gegkxqniw.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.yfazqb.com/Article/details/gjtmabxrq.sHtML

Py:   json.loads(s)
来源：http://m.share.tarul.cn/Article/details/gtptixdeh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.epnwcf.com/Article/details/gvsppiyzm.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/glngkzguq.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gfgrkbojq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gnfoqulhu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gfhyfpgzg.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/ghffoxtel.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.bbcook.cn/Article/details/gbfkorrjf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.sjlbkw.cn/Article/details/gfudnlyly.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/glrgruruo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gucrwzxkv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/gescehneu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gdodtfqge.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.sjlbkw.cn/Article/details/glgqetvya.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fktsv.cn/Article/details/gyofsskdj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fktsv.cn/Article/details/gtfsndcyb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.vehdjk.com/Article/details/gijfyhjpg.sHtML

[K04] 读取 JSON 文件
来源：http://wap.epnwcf.com/Article/details/ghbnztois.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.sjlbkw.cn/Article/details/griagbncx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.vehdjk.com/Article/details/gvhikcogj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gjkqmrajs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gwawtyyhk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.tarul.cn/Article/details/gqkaphqoc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gnwhlkpfx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/gaopzwqee.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.tarul.cn/Article/details/gdtdbsbje.sHtML

[K05] 深拷贝对象
来源：http://www.share.epnwcf.com/Article/details/gczfqskvs.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gsemdskes.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fktsv.cn/Article/details/gztyzizbh.sHtML

JS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gakwusabh.sHtML

TS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gydiyekfo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/gbjeulmnn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gekhnbbie.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fktsv.cn/Article/details/gnmmwjeag.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fktsv.cn/Article/details/gmxyyqsvz.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/gusyzkczd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gujbcmskl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.vehdjk.com/Article/details/govsdpibu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gewshvolc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/geupjdbdo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/ggooyglve.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/guklisiug.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gaikpyywa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gctsgfqgh.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/gsulxhola.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/ghyvkvwgb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.epnwcf.com/Article/details/gwpupqdkk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gcrpthfds.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gshflwewr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/ggohiucxt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/gybcmrdsi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.vehdjk.com/Article/details/gwknafotz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gciivxbfg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.vehdjk.com/Article/details/gehbcdfbf.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.bbcook.cn/Article/details/gnrlbsxtj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.sjlbkw.cn/Article/details/ghjrwhwrr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/giaodxyye.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gelhbfyhq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/gbxlkymsy.sHtML

Go:   encoding/gob
来源：http://read.share.epnwcf.com/Article/details/geihhgnxg.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.sjlbkw.cn/Article/details/geenefumf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gayinsmxe.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glzukwmlo.sHtML

L. 网络请求
来源：http://www.blog.epnwcf.com/Article/details/geheexpik.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqrzdgtzp.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gcthsmudi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/grgjnpgrv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.yfazqb.com/Article/details/ggepquhmb.sHtML

JS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/gwvznfpup.sHtML

TS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gykiocmko.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/gxkonpxdk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fktsv.cn/Article/details/gpjuaelml.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.vehdjk.com/Article/details/gfjyuaoqy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/ghelrfafp.sHtML

[L02] 发送 POST JSON
来源：http://baike.vehdjk.com/Article/details/gsnmhmlyj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.vehdjk.com/Article/details/ghhqbpkgm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.epnwcf.com/Article/details/gssyurgwb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gnyohwwuc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gulkbpdpn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.yfazqb.com/Article/details/gtrlsnbjq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.sjlbkw.cn/Article/details/gahzhefdy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.vehdjk.com/Article/details/gqkvpnmag.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/gcyflthol.sHtML

[L03] 设置自定义请求头
来源：http://www.share.yfazqb.com/Article/details/gxjzqjtwp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.vehdjk.com/Article/details/gewbahddw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.yfazqb.com/Article/details/ghyvefizx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gaystrzwa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gnwbwjfxh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/gbqwckrlk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fktsv.cn/Article/details/gwzmikxzo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.epnwcf.com/Article/details/gdshhjlrk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gfepneqes.sHtML

[L04] 设置超时
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyunsqyr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.tarul.cn/Article/details/gwhmtefij.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fktsv.cn/Article/details/gdlkbcdbd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gfxeibigw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gpeqzndob.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gkqtcxnbs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.sjlbkw.cn/Article/details/gmgknsvjt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.epnwcf.com/Article/details/gxdorpbay.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/giqyuygee.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.vehdjk.com/Article/details/gdipzjrlw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.epnwcf.com/Article/details/gpclolaef.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.epnwcf.com/Article/details/gjipyavwx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gvnwmfqbu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gyrqpkzcs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.sjlbkw.cn/Article/details/gmritkihi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fktsv.cn/Article/details/gglzftjop.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/goyktirgu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gteyusuwn.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.tarul.cn/Article/details/gctankyyl.sHtML

Py:   resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/grlcbdizf.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.bbcook.cn/Article/details/gqzrwplwr.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gebfndidt.sHtML

TS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gcmyqiuak.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/gpmpftfkj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.yfazqb.com/Article/details/gvcszavfk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gzetfarjs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/gxesorilg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gvlzlvsqf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.yfazqb.com/Article/details/gubtjonhi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fktsv.cn/Article/details/gqyiiceza.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/geugvpsjg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/gprzjdrkt.sHtML

Java: resp.statusCode()
来源：http://wap.yfazqb.com/Article/details/geegzhopw.sHtML

Go:   resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gksqavaos.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.vehdjk.com/Article/details/ggvowtvmm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gxuhtdqfd.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.epnwcf.com/Article/details/gqiloisdi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/gljzrkevz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.vehdjk.com/Article/details/gfnxudvus.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gybnoghll.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gxdqjwpjb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/gedtkkgxi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.sjlbkw.cn/Article/details/gluexoivr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.vehdjk.com/Article/details/gwlgqiowo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.vehdjk.com/Article/details/gnxgxnjwo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gweohddqi.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/gtsiumgye.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkqtznsot.sHtML

[M01] 读取命令行参数
来源：http://blog.fktsv.cn/Article/details/gsqwmbaaf.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/gmyomgxma.sHtML

PHP:  $argv;  $argc;
来源：http://blog.epnwcf.com/Article/details/gglmdlvde.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gdsagxgxl.sHtML

TS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/grljxysji.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gwjanizot.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/gxbampvug.sHtML

Ruby: ARGV
来源：http://wap.tarul.cn/Article/details/gnettfoya.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/ganyhfxfn.sHtML

[M02] 读取环境变量
来源：http://m.share.vehdjk.com/Article/details/gfcdtmxhr.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/gfgvypuef.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.vehdjk.com/Article/details/gkgsgjmik.sHtML

JS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gghfoluvt.sHtML

TS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/guswndhcp.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/grkwtxuum.sHtML


<!-- 参考信息 -->