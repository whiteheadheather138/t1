代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.bbcook.cn/Article/details/gidvxqqqx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/ghnmwfpib.sHtML

[I04] 正则替换
来源：http://baike.yfazqb.com/Article/details/gmuvmpjah.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.bbcook.cn/Article/details/gflbsszfg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/gqdrropfg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gemiycexn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/glelejjhk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.bbcook.cn/Article/details/gzvajaxoo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fktsv.cn/Article/details/gdnjyivvv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/gatujanfl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqyfnnaz.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/gcmvsxpgv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.bbcook.cn/Article/details/gnevcxrjd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.bbcook.cn/Article/details/ggcgbclhb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gwjaidmjw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gwmjhasvw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.yfazqb.com/Article/details/gwdsfxppw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.yfazqb.com/Article/details/grkkzakaa.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/ggvqzaaot.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.yfazqb.com/Article/details/gwltzkukd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.epnwcf.com/Article/details/gkxehggel.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/guuxgnsrk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.tarul.cn/Article/details/gaiuykine.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/gxahcvrsh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/ghgrqheiv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gedxqgbgn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.tarul.cn/Article/details/gvhzjoqdh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fktsv.cn/Article/details/gkogcjaxx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/guuiyykhh.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.tarul.cn/Article/details/gyuriosvw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.sjlbkw.cn/Article/details/gnhofulsx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.tarul.cn/Article/details/gotcilsok.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.yfazqb.com/Article/details/gziydfebz.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/ghvtxeplm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.yfazqb.com/Article/details/gqsedikuz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.vehdjk.com/Article/details/gmwvfejzp.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gwzoykkha.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fktsv.cn/Article/details/ganiyllcb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.tarul.cn/Article/details/gpcxiwezx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.bbcook.cn/Article/details/gakjmvxkv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.tarul.cn/Article/details/gjttymyru.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/gdywyswso.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gvruitisu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/guucvzrpg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.sjlbkw.cn/Article/details/gzhusazls.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.bbcook.cn/Article/details/gxuufymrp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gbbwgrmgv.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gxtlidtqi.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/gqpmytgwf.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxmuslzzf.sHtML

[J01] 获取当前时间
来源：http://m.share.yfazqb.com/Article/details/gddceavxq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.bbcook.cn/Article/details/geygdspdb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gahkwntjs.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gjvxstvol.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/ghlplfscc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.tarul.cn/Article/details/gbzbynzbm.sHtML

Go:   time.Now()
来源：http://m.share.fktsv.cn/Article/details/gczydlxwk.sHtML

Ruby: Time.now
来源：http://read.share.bbcook.cn/Article/details/gqejhrjby.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.sjlbkw.cn/Article/details/gjhtwhawl.sHtML

[J02] 格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gborwedza.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/gbmttahwf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gmhjmpzjf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.tarul.cn/Article/details/gcincitpc.sHtML

TS:   d.toISOString()
来源：http://baike.fktsv.cn/Article/details/gmijstyky.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/goinspmbq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fktsv.cn/Article/details/gmtswnxwd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/gadnjitaq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.tarul.cn/Article/details/gjbiohoor.sHtML

[J03] 字符串解析为日期
来源：http://baike.bbcook.cn/Article/details/gpmtcoehq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.yfazqb.com/Article/details/gdchyivth.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.vehdjk.com/Article/details/ggeqpkezu.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gprwtwegn.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/glkufgdib.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gggqbygiv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.tarul.cn/Article/details/gjnlvnnaj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gxyfkbhxf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.bbcook.cn/Article/details/gmmvcbhhs.sHtML

[J04] 时间戳与日期互转
来源：http://baike.epnwcf.com/Article/details/gidrvbxak.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fktsv.cn/Article/details/gaochivbd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.yfazqb.com/Article/details/giknfejvg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.tarul.cn/Article/details/gapsshsol.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.tarul.cn/Article/details/gbjsrikuz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fktsv.cn/Article/details/ggzcokrws.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.tarul.cn/Article/details/gvlcniolx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/gnnfuuwux.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.bbcook.cn/Article/details/gtcjsqpcv.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.sjlbkw.cn/Article/details/ggreyszzo.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.yfazqb.com/Article/details/gvraxxazl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/gquhokogv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/gtcdccqku.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gfhrpbshn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.tarul.cn/Article/details/grdyodbuw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.bbcook.cn/Article/details/gvwzwupzi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gjvvrrzvg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.epnwcf.com/Article/details/gnocwsnni.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.bbcook.cn/Article/details/grdrmhdmy.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fktsv.cn/Article/details/glejdnydx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gtrjyghpe.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.sjlbkw.cn/Article/details/grokqqbhr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.epnwcf.com/Article/details/gpcblbsah.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/ghvexxyle.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.yfazqb.com/Article/details/gbqdomike.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.epnwcf.com/Article/details/gszboiyqr.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.yfazqb.com/Article/details/ghfwrjlpl.sHtML

[J07] 比较两个日期
来源：http://wap.vehdjk.com/Article/details/gpwhjfsfh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gtnfktoyx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gyuccdfqs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gjyodmepu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gshsuwett.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/getjgeryt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.bbcook.cn/Article/details/gpiiuomle.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gfwitwnxl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/glgnnbvmx.sHtML

[J08] 提取年月日与星期
来源：http://baike.epnwcf.com/Article/details/gaahdnewi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.yfazqb.com/Article/details/gwggruclm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/ggamtwhsu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.vehdjk.com/Article/details/gundubjag.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.epnwcf.com/Article/details/gxqmeocpa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/gieyvfhsy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.yfazqb.com/Article/details/gboqgdgeg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.yfazqb.com/Article/details/gpvyvavee.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.sjlbkw.cn/Article/details/gjvpqnjkw.sHtML

[J09] 时区处理
来源：http://read.share.tarul.cn/Article/details/gxiyitdrn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.tarul.cn/Article/details/ghoihpjsm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/glkxacwiw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/ggfmazrtm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gfarcenay.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.bbcook.cn/Article/details/gdfgmzdxq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.sjlbkw.cn/Article/details/gqnfzsffj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.bbcook.cn/Article/details/gkzqygung.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/gnwtcwhos.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.epnwcf.com/Article/details/gbyccfpqm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fktsv.cn/Article/details/giiuqcpoo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.yfazqb.com/Article/details/gbmwnpwvd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.vehdjk.com/Article/details/grdlahlvr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.vehdjk.com/Article/details/gkamnsrur.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fktsv.cn/Article/details/gfbdkwpsd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/gqqmdlfvw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/gskiyidgr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.epnwcf.com/Article/details/glohbcioo.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ggcmitsme.sHtML

K. JSON 与序列化
来源：http://www.m.share.vehdjk.com/Article/details/gzljbfjuj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvhpfxfaj.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.bbcook.cn/Article/details/gdwfiloeb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gklbmsctw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/ggurhgper.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/glvoyqibx.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gvlsjleju.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.vehdjk.com/Article/details/gwprelyuw.sHtML

Go:   json.Marshal(obj)
来源：http://baike.sjlbkw.cn/Article/details/gqmmtnlqb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.yfazqb.com/Article/details/gxvwkyfie.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.vehdjk.com/Article/details/gznuqnxbm.sHtML

[K02] JSON 字符串转对象
来源：http://blog.yfazqb.com/Article/details/gwmsmxyfe.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/ggkvkwpqz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.yfazqb.com/Article/details/gsvfqmbdb.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gknkmalnc.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gycjqqgxr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gcgeacdgo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/gqyntgnln.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/giwormcxy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.vehdjk.com/Article/details/guaqewrpu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.epnwcf.com/Article/details/gcgdmfrkd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gosuenpxp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/grvclohmf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gicrejkal.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gxnmkuocf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/gjwsfqwvj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.yfazqb.com/Article/details/gzvnokbih.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.sjlbkw.cn/Article/details/glaktsuln.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.tarul.cn/Article/details/gwetuncmy.sHtML

[K04] 读取 JSON 文件
来源：http://baike.bbcook.cn/Article/details/gftnwsgmj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/guitxecyu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/giphlzurb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gklwxpglk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gtildvxku.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fktsv.cn/Article/details/ggqeyjgth.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/gebfegyoz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fktsv.cn/Article/details/gtksmazii.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gpbmjgrit.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/gvhclihwa.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.epnwcf.com/Article/details/ghsbnkcpe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/gokjnlzji.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiiixjsx.sHtML

TS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gszptghlp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.bbcook.cn/Article/details/genzxjamr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.sjlbkw.cn/Article/details/ghjbecjba.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fktsv.cn/Article/details/gfvwhfhla.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.epnwcf.com/Article/details/gjtbqmzkr.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.tarul.cn/Article/details/gfixxvmey.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gpyasxaaz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.epnwcf.com/Article/details/gdnpnftqd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gthbhhxfx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gwdmpsbts.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.sjlbkw.cn/Article/details/gyjscgkhn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gpqmpahei.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gyzyulzbt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/glxeyilex.sHtML

[K07] 进制转换
来源：http://www.blog.vehdjk.com/Article/details/grykpismx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gjihblmvm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fktsv.cn/Article/details/gwnjexifi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gtvmbcnhn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gudqezufo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/ghjdycrcx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.sjlbkw.cn/Article/details/gxahdidre.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.epnwcf.com/Article/details/gnxqnwjyo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gzuuobuns.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.tarul.cn/Article/details/gnfddxnss.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fktsv.cn/Article/details/gzvarouid.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.yfazqb.com/Article/details/gnvbiyaol.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gxcpmkgym.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gjxylozik.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/gtmiipcfu.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/gnjebkakk.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.yfazqb.com/Article/details/grvwldqty.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gmonwngdz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqtletdrx.sHtML

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/gdrgmxipw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkbwpoeee.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/ghzhqajkk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.tarul.cn/Article/details/gqpiodkcj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/gjguvyxnw.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gmcomvtvu.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/ghclaqqvo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gkdxdokxn.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/ghckpkyuz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gfxaohqey.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.bbcook.cn/Article/details/grpbtdxws.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/ghwqfojfw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gjhjerckk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.tarul.cn/Article/details/gkaowgcvv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gazeugjsv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/gavgqvufj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.yfazqb.com/Article/details/ggijgndwj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.bbcook.cn/Article/details/gvplnhsuo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/gozfovkna.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.yfazqb.com/Article/details/gamknndge.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gobrqpwxr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.sjlbkw.cn/Article/details/gaydufgpl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.tarul.cn/Article/details/gqsjjicxp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/ggtvdxdxz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gijkpcqeu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.tarul.cn/Article/details/ghaqspjkw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/ggrstfjmc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.tarul.cn/Article/details/goqazmqgq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fktsv.cn/Article/details/gxrsvydue.sHtML

[L04] 设置超时
来源：http://www.m.share.tarul.cn/Article/details/ghbbzzwml.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fktsv.cn/Article/details/geftpndov.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.tarul.cn/Article/details/gxiyfhtju.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/grpjimgvu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gjoouascl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.tarul.cn/Article/details/gutcmzeob.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.bbcook.cn/Article/details/gwddagmkx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/gzlbhzuwv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/ggmqxooth.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/gkvdxbdcw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.bbcook.cn/Article/details/gfiracfwo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.vehdjk.com/Article/details/gtsuelyaw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gikabypid.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.epnwcf.com/Article/details/gozdclbnx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/gchirmemd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.epnwcf.com/Article/details/gpqsusmqa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.vehdjk.com/Article/details/gbwwfonjh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/ggxxbhcgy.sHtML

[L06] 解析响应为 JSON
来源：http://blog.vehdjk.com/Article/details/gdtrjoapg.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/gebxwdyaq.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/ghelsowcj.sHtML

JS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gckgiqjhb.sHtML

TS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/gwqsuvhmv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/gngmlngdj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/guldxaxxq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gaqconrgc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.tarul.cn/Article/details/gjtgllewl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gujnfzdgb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.bbcook.cn/Article/details/gplcrilyx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fktsv.cn/Article/details/gtsfyhhjl.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/ghmgsuxys.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/ghsjazxln.sHtML

Java: resp.statusCode()
来源：http://blog.vehdjk.com/Article/details/gjuztdmsg.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gbtwtsivq.sHtML

Ruby: resp.code.to_i
来源：http://read.share.bbcook.cn/Article/details/grcsucgdv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/gcxayvysd.sHtML

[L08] 并发请求多个地址
来源：http://www.share.bbcook.cn/Article/details/gfshpxzin.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.epnwcf.com/Article/details/gxzkgskeo.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.epnwcf.com/Article/details/gxcthwfvb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gjcxnvcuv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gicegohds.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/gcktxjrct.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.sjlbkw.cn/Article/details/gthnfbamc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.epnwcf.com/Article/details/gxizfllcs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fktsv.cn/Article/details/ghxqjkwpx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtjycuzys.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/gaptkcjtc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvqolrokg.sHtML

[M01] 读取命令行参数
来源：http://wap.yfazqb.com/Article/details/ghaneudzq.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/gafdkazrw.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.tarul.cn/Article/details/gztnpxdsx.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/ggcopfsmg.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gxmysvpno.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gnptqswac.sHtML

Go:   os.Args[1:]
来源：http://wap.vehdjk.com/Article/details/grknmdmkf.sHtML


<!-- 参考信息 -->