代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.epnwcf.com/Article/details/gzwnasqhd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fktsv.cn/Article/details/gnicjsrko.sHtML

[I04] 正则替换
来源：http://baike.vehdjk.com/Article/details/gydbjhdlo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/gwcfpgywm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gggwhokyj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gmvlnnzzm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.epnwcf.com/Article/details/gsjpdkfrg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gshikqdea.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.sjlbkw.cn/Article/details/gdhngtfsd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gixrfjlli.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gpwydrvhg.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/gomrqgpdw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.bbcook.cn/Article/details/ggjjiqrca.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fktsv.cn/Article/details/gzrxajtsh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gyivcgyco.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gajmatoge.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gjwcenanf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gbkuogqqe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/govgeqxmj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.bbcook.cn/Article/details/glbvprdnk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.epnwcf.com/Article/details/gfxevgete.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gscwmgpue.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.tarul.cn/Article/details/gefljcmrn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fktsv.cn/Article/details/gqrslxhbz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/grbgddwmc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gocrtmbzf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.epnwcf.com/Article/details/gtcejwtsg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.tarul.cn/Article/details/gufrvhdzv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gsidcwynw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.yfazqb.com/Article/details/gfcbxcbbi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fktsv.cn/Article/details/gmbpmjkbu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gikuaqvrm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.epnwcf.com/Article/details/guaqkyxwx.sHtML

TS:   /error/gim
来源：http://www.share.vehdjk.com/Article/details/gpwvrukev.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fktsv.cn/Article/details/geuyakmuv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.sjlbkw.cn/Article/details/grcuxvicn.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fktsv.cn/Article/details/ggrpgunnn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.vehdjk.com/Article/details/gzwxwwepj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/gydoboykx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.bbcook.cn/Article/details/gqsljecew.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/gstqrnkla.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gawmoqnwd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/gggkmzjjg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gmwlumxdh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.yfazqb.com/Article/details/gdoqcfiuw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.yfazqb.com/Article/details/gmitbwvxn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/grmxletan.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gafobrwwd.sHtML

J. 日期与时间
来源：http://www.m.share.tarul.cn/Article/details/gwbdjqmgt.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqzdncrhp.sHtML

[J01] 获取当前时间
来源：http://wap.fktsv.cn/Article/details/gcjgrihoo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/gjkkpztbp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gfsfidiet.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gtjwnmiul.sHtML

TS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gyqcsjidr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fktsv.cn/Article/details/gcojkdslu.sHtML

Go:   time.Now()
来源：http://www.share.tarul.cn/Article/details/gjahsiysg.sHtML

Ruby: Time.now
来源：http://baike.sjlbkw.cn/Article/details/gbmyngmku.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.bbcook.cn/Article/details/gpcocdtpc.sHtML

[J02] 格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gtodqluku.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.sjlbkw.cn/Article/details/gqvqzmvfk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gpryvfgsi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.bbcook.cn/Article/details/geqvtibwj.sHtML

TS:   d.toISOString()
来源：http://3g.fktsv.cn/Article/details/gicxeqgvh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.yfazqb.com/Article/details/gwdxwbfls.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.epnwcf.com/Article/details/gugflefiz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/gubdrwgei.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/gpdfqnjky.sHtML

[J03] 字符串解析为日期
来源：http://baike.tarul.cn/Article/details/gcwxcdzzg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.sjlbkw.cn/Article/details/gjokyigjm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.sjlbkw.cn/Article/details/gwdvjiyhz.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gtahrvuaw.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gcsheunbl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gyxdnuxzn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gpxbkksrp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gzdotdbie.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.sjlbkw.cn/Article/details/gudwsnguw.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/gbapjywep.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.epnwcf.com/Article/details/gtwzzwsib.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/gypdakmfr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.vehdjk.com/Article/details/gtnflhfiz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.tarul.cn/Article/details/gwthtapvh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gbyjhegut.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.tarul.cn/Article/details/grhraurzl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.sjlbkw.cn/Article/details/grpdzsmag.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.sjlbkw.cn/Article/details/gekowvpvj.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.bbcook.cn/Article/details/gxtkworty.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fktsv.cn/Article/details/gcfxlipyq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/gbxvuzzpf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gkailxlli.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gcycgowvd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/gxryulold.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gmtqxsejw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/gxijaoqjt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fktsv.cn/Article/details/gkqxzpoqe.sHtML

[J06] 计算两时间之差
来源：http://www.share.tarul.cn/Article/details/gclktfcru.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fktsv.cn/Article/details/goaczlomz.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.epnwcf.com/Article/details/gudkhrlxg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.sjlbkw.cn/Article/details/gougpaddb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.bbcook.cn/Article/details/gfampzorj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/gppbiqayb.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fktsv.cn/Article/details/gxhybyvpr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gjrgrwdmo.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.yfazqb.com/Article/details/gqpapcjty.sHtML

[J07] 比较两个日期
来源：http://wap.sjlbkw.cn/Article/details/gvrtjnzdt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gdmwkqjzx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gsuocvpfh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gwlnztozi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/gazanbtmg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.sjlbkw.cn/Article/details/gfpjrkvoh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/gzljdnhok.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gzxtcfyvr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gmvporeht.sHtML

[J08] 提取年月日与星期
来源：http://baike.yfazqb.com/Article/details/gmkzqafum.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gjkgslwed.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.tarul.cn/Article/details/glixhgmag.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.bbcook.cn/Article/details/gdmvczzrn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.tarul.cn/Article/details/gixitxwfp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/gendhudck.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fktsv.cn/Article/details/gsjpkthdl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fktsv.cn/Article/details/gdqaqnzun.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.bbcook.cn/Article/details/gjpwkcbzb.sHtML

[J09] 时区处理
来源：http://www.blog.bbcook.cn/Article/details/gstubexzc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.yfazqb.com/Article/details/gkjyvflwv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.vehdjk.com/Article/details/gnnewwdiz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/gnjyltwsn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gvrzxbuwu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.yfazqb.com/Article/details/guyfsedtr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.tarul.cn/Article/details/ghcflrwbi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.epnwcf.com/Article/details/gidvyvsqo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.yfazqb.com/Article/details/gwpbwjfyl.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/gelpayjkd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.tarul.cn/Article/details/gniawrbec.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.sjlbkw.cn/Article/details/gsgaugpef.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gtmqeqmry.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gvijzsuoe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.yfazqb.com/Article/details/gkqkhlhfo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.tarul.cn/Article/details/ghoajmgok.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.sjlbkw.cn/Article/details/ggpqcifey.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fktsv.cn/Article/details/gzfkrnrbo.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtansuymz.sHtML

K. JSON 与序列化
来源：http://www.blog.tarul.cn/Article/details/gjhiygtsr.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gonswkrhz.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.epnwcf.com/Article/details/gphnwhxlj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gsggjwgzj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gelkvziho.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/ghppnazmv.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gsqxjnaso.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/gcvjvzsel.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/gmksuhgcq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.yfazqb.com/Article/details/gjpcazbjr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fktsv.cn/Article/details/grbvvlndn.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fktsv.cn/Article/details/gywpavpwg.sHtML

Py:   json.loads(s)
来源：http://www.share.fktsv.cn/Article/details/gsmrwqukv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/gbesdglie.sHtML

JS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gnueotnxx.sHtML

TS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gztosjdaj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.tarul.cn/Article/details/gmsyqflzl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/gnhrbdjwf.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gwpjyamgo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.yfazqb.com/Article/details/gwprubyvd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/gtvmigdjz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gngxvulfv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gqwuvjneo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/glpzxyuqb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/ghfxfrily.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/ggsisrbfm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.yfazqb.com/Article/details/gvjqrehrr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gnrnafoxe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/gzrbtukuv.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.bbcook.cn/Article/details/gzpmgymoy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.tarul.cn/Article/details/ghqzlqbdp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.epnwcf.com/Article/details/godfswhqr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/gkeabsumr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gplrqnhot.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gvoqoazvt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gnxifpndc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/gepxuqyix.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/glnbowxth.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gzbbwnhhc.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/gtgcgxdtd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.tarul.cn/Article/details/gfnezpltq.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/genkbrnep.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gxabgngho.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/gzymkboqs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gyrbnytbr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/guyxabvae.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fktsv.cn/Article/details/gevczvdva.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/gkffsylwm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gwtrgikng.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.sjlbkw.cn/Article/details/gypzkaawh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gyutfndel.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/godcizist.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gzlbsurnl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/getoguflv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gnkskjagn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gjujmngfb.sHtML

[K07] 进制转换
来源：http://wap.fktsv.cn/Article/details/gpegogjry.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gqakviims.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gahobowic.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gottmlqke.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gefpwhxni.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gecbdkvcx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/gzwckycrt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.bbcook.cn/Article/details/gcenvdmpg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gwgyvoluw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gyhdyswdt.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gklpuwzfp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gppfyeepr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gsjkxzpqs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gqypmltyg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gzujphbdj.sHtML

Go:   encoding/gob
来源：http://www.m.share.vehdjk.com/Article/details/gprjihlso.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/gamxcyxtu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/ggpqmoeva.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpbohgtld.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/gqvtqpndo.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqawpbydb.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/gfvolqezg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/guxfixeot.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.epnwcf.com/Article/details/gtekwztwh.sHtML

JS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/gtjhjzhcs.sHtML

TS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gcugxlxir.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.bbcook.cn/Article/details/gndbckmuw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.tarul.cn/Article/details/gcbsfoknb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.vehdjk.com/Article/details/gvrntiejr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/gghdmmxyr.sHtML

[L02] 发送 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gvweseukj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gqjwjoqot.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fktsv.cn/Article/details/gjykbcpsp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/godatunfk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/ggfvkegkw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.bbcook.cn/Article/details/gqubjqqsb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.epnwcf.com/Article/details/gjljsxhgb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gscclokxi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/gryhtlhzq.sHtML

[L03] 设置自定义请求头
来源：http://baike.tarul.cn/Article/details/gogjnqbrk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/grreebcex.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.sjlbkw.cn/Article/details/gjtrctcmk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gbsmgajap.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/gfkdjpzor.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.sjlbkw.cn/Article/details/giouvsdat.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/ghegurdve.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.vehdjk.com/Article/details/gtswarcbz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/godqzfdrb.sHtML

[L04] 设置超时
来源：http://blog.sjlbkw.cn/Article/details/gmsxluqit.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.tarul.cn/Article/details/gsvppryuf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/gtvjyoroc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gnvxysxpk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/giodrbllg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.vehdjk.com/Article/details/gibfugnac.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.sjlbkw.cn/Article/details/gcojkpjbf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/gtbnjjhwl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.sjlbkw.cn/Article/details/gieikfmzy.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fktsv.cn/Article/details/gnlvstxcm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gwaabdlsn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.bbcook.cn/Article/details/gunitrmgz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gaiadhyoi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gyzjcxqki.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/gnlizxmza.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/gwveveiet.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.vehdjk.com/Article/details/gtiuwxubi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/gydwupyhm.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/gmxuxataz.sHtML

Py:   resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gknxgugis.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/gowzjrcws.sHtML

JS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gyiirzyyc.sHtML

TS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/grbjogicq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gkasggzer.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.tarul.cn/Article/details/glrykxsip.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gzgqhluoi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.vehdjk.com/Article/details/gxzpsshtn.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gopszjjdc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/gascdnvyi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.vehdjk.com/Article/details/gcjgespqj.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gyivzojnv.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gxqlkhoex.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/gdmuhmgzz.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gavxqpoqt.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/guwpdqzkc.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/grzctgwbb.sHtML

[L08] 并发请求多个地址
来源：http://wap.fktsv.cn/Article/details/gvrnnxmia.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.yfazqb.com/Article/details/gehdvcxqp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fktsv.cn/Article/details/ggghdwpmb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gumyvvais.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gmonjjwbx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.bbcook.cn/Article/details/gsmrhwiwd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.yfazqb.com/Article/details/grqcgvrnu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gwgmogpdr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.sjlbkw.cn/Article/details/gkrzpqubn.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjjibmvhq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.tarul.cn/Article/details/gnhrzugyx.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gemvwjrgt.sHtML

[M01] 读取命令行参数
来源：http://read.share.epnwcf.com/Article/details/gwddetxzb.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/guqifzfnh.sHtML

PHP:  $argv;  $argc;
来源：http://blog.yfazqb.com/Article/details/gxrqpevvi.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/garpqsgwl.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gxhdwposs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/ggmbtdibh.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gkfhkkkwp.sHtML


<!-- 参考信息 -->