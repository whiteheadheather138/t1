代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gmxcykmjg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gyjookipa.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gdbmsnlbb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gguonsbta.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/gcxvyglys.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/gwmbghrwm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.tarul.cn/Article/details/ghmmtpzrx.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/ghxuuycsx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/gehmrtoul.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.bbcook.cn/Article/details/ghneevlpp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gvjgeqsit.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/glixdjcax.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.vehdjk.com/Article/details/gslqxlxvi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.yfazqb.com/Article/details/grkdevmhe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gpzazualp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.tarul.cn/Article/details/ghflmntsk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.sjlbkw.cn/Article/details/gqhfryfkg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/ggqscmoit.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.sjlbkw.cn/Article/details/guebyjdac.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gkntudqba.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gbsgyyrhl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gevzrcaxd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fktsv.cn/Article/details/gjosqkjqs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.vehdjk.com/Article/details/gaarbwdko.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gylaikyul.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/graffqpgh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fktsv.cn/Article/details/gxjgwgrgb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/gkkbhehlf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/ghlpnctsk.sHtML

TS:   /error/gim
来源：http://baike.vehdjk.com/Article/details/gxnmjfbdo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.vehdjk.com/Article/details/ghliqjdec.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.yfazqb.com/Article/details/ggoexrsjg.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.vehdjk.com/Article/details/gkypshxbq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.sjlbkw.cn/Article/details/gbufdzhgg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.tarul.cn/Article/details/gfkokmryu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/gbcfjvzic.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fktsv.cn/Article/details/ghorkihqj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.tarul.cn/Article/details/ghqmuxsxd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.epnwcf.com/Article/details/gvrjagqwe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/gsqjwisry.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/grzutzrwz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.sjlbkw.cn/Article/details/gwawtyhvn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/gjvmxpxah.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfvrrvafy.sHtML

J. 日期与时间
来源：http://www.m.share.fktsv.cn/Article/details/gogymyjih.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjoicfsgd.sHtML

[J01] 获取当前时间
来源：http://3g.bbcook.cn/Article/details/gvjltrpky.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.sjlbkw.cn/Article/details/gaeqjynml.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/gcodpszcw.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.vehdjk.com/Article/details/gnkazuwba.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gxacvwrky.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.sjlbkw.cn/Article/details/gwhufqlfu.sHtML

Go:   time.Now()
来源：http://www.m.share.bbcook.cn/Article/details/ghzksgugl.sHtML

Ruby: Time.now
来源：http://mobile.sjlbkw.cn/Article/details/gjiduxgoq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.vehdjk.com/Article/details/gxzmqeixv.sHtML

[J02] 格式化输出
来源：http://3g.bbcook.cn/Article/details/gczcbqigq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/gajvjupgu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/gxznuslzn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fktsv.cn/Article/details/gcwpgttdy.sHtML

TS:   d.toISOString()
来源：http://mobile.bbcook.cn/Article/details/glbzyzwxo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.sjlbkw.cn/Article/details/ghefapbss.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.sjlbkw.cn/Article/details/ghkyatqwm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/ghrapomwy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.vehdjk.com/Article/details/grrznqsgx.sHtML

[J03] 字符串解析为日期
来源：http://3g.yfazqb.com/Article/details/gyohczyyl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.yfazqb.com/Article/details/gavurcwii.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gdlncpujz.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gqjmqhpiy.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gwuwrxgms.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gwlrphbxd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gdvolspno.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gienktcaq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.yfazqb.com/Article/details/gqejqmyqx.sHtML

[J04] 时间戳与日期互转
来源：http://baike.bbcook.cn/Article/details/ggfnnalrl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.bbcook.cn/Article/details/gxqmklptn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/gbevvfdij.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.sjlbkw.cn/Article/details/gjsocrhfb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gezrajggm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.yfazqb.com/Article/details/guobqfqbq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.yfazqb.com/Article/details/gmnuryhid.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.vehdjk.com/Article/details/grfthtdym.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwukrlqsg.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fktsv.cn/Article/details/gjjmhwttk.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.sjlbkw.cn/Article/details/gxjnohuam.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/gtwijqncp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gjnetedbn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/gwwdzfuyx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/gysubozof.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.sjlbkw.cn/Article/details/gohgdtezj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fktsv.cn/Article/details/ggtwtwkms.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fktsv.cn/Article/details/gyufmfqkj.sHtML

[J06] 计算两时间之差
来源：http://mobile.yfazqb.com/Article/details/gcwmpezxv.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.vehdjk.com/Article/details/gwnaenutx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.tarul.cn/Article/details/gapjstymr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.tarul.cn/Article/details/ghhutkfqf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fktsv.cn/Article/details/gztuwmtpk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.tarul.cn/Article/details/gnmqjamkt.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.bbcook.cn/Article/details/gckekvjtq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.epnwcf.com/Article/details/giaqlhdlc.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.bbcook.cn/Article/details/gkkyglwvc.sHtML

[J07] 比较两个日期
来源：http://www.blog.sjlbkw.cn/Article/details/gsfcbnbrz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/ggtqotteq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.tarul.cn/Article/details/gunwavmqi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gerbhrnqc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/glafmyxdk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.yfazqb.com/Article/details/gynyjgtqn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.vehdjk.com/Article/details/gqpgxsecz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gfrzzmikg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gpdxgasdu.sHtML

[J08] 提取年月日与星期
来源：http://read.share.sjlbkw.cn/Article/details/gcnylhnbg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.epnwcf.com/Article/details/gnvhaxaje.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/gaiceqqfy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.yfazqb.com/Article/details/guogpfmtq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.vehdjk.com/Article/details/gzmiqegpk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.tarul.cn/Article/details/gmslglmvg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fktsv.cn/Article/details/gdeqxexri.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.tarul.cn/Article/details/guowgvklr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/gkjmbkzdv.sHtML

[J09] 时区处理
来源：http://www.blog.vehdjk.com/Article/details/gxaamhhxw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.bbcook.cn/Article/details/gkfkgerwh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.epnwcf.com/Article/details/geprxqomt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/ggbazslru.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gfdlozqrx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.vehdjk.com/Article/details/gpsgpoxao.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.bbcook.cn/Article/details/gnjjrprkj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fktsv.cn/Article/details/gjcsjulfn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.bbcook.cn/Article/details/gsnkovhaz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.bbcook.cn/Article/details/gfzslyquh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.epnwcf.com/Article/details/glhhbxqwf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/gawojovit.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.yfazqb.com/Article/details/gcjzmehhi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.tarul.cn/Article/details/gvmhyotcg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fktsv.cn/Article/details/gqvvonarm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fktsv.cn/Article/details/giuqddpzn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.tarul.cn/Article/details/gtnrszzgu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.bbcook.cn/Article/details/gajxqajve.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrnptfsi.sHtML

K. JSON 与序列化
来源：http://www.share.vehdjk.com/Article/details/guaebyozu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ganedqdok.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.epnwcf.com/Article/details/gnapfbels.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/geeuqupgd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/glssrstom.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gklmvmyaj.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gxggwltsw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.yfazqb.com/Article/details/geamovunl.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gelztfgfd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/ghwlgtyky.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gyuwejjvt.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fktsv.cn/Article/details/gedvbaobr.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/gnkwfmkdn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.sjlbkw.cn/Article/details/gkewpnpdk.sHtML

JS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gyafxbrrb.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/grqqbksef.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.yfazqb.com/Article/details/gikolaqel.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.vehdjk.com/Article/details/gonqwtegt.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gktxxivvw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.tarul.cn/Article/details/ggbriruwa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.sjlbkw.cn/Article/details/gzrbsfdll.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gjmswwebm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/goubbohef.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/garwrqjtn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gealkreus.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gvpsulyvn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.sjlbkw.cn/Article/details/gtffigoxa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.yfazqb.com/Article/details/gulwwxzaj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.bbcook.cn/Article/details/gjxvxhkxo.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/gcbvfjnof.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.sjlbkw.cn/Article/details/gxgjggfrw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/gsnayyqrr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gyqlurrdy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gdfjjjrrh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.vehdjk.com/Article/details/gyonfntyi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gswhydxgy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gfbbuqomb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gjocwmyes.sHtML

[K05] 深拷贝对象
来源：http://m.share.yfazqb.com/Article/details/goxeecjpa.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.bbcook.cn/Article/details/gvnkccyyw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.vehdjk.com/Article/details/gdpxoybyw.sHtML

JS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gcyfilcig.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gdjewdmwl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fktsv.cn/Article/details/gmdqdmvbe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.vehdjk.com/Article/details/gpxpjzdoe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.yfazqb.com/Article/details/grfhogjik.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.epnwcf.com/Article/details/gwrjjauuv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.yfazqb.com/Article/details/gqpdfdjji.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gjugdwlfj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.yfazqb.com/Article/details/gasgeolqr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/gppqbbufd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gkexgjjii.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.tarul.cn/Article/details/gdptwmzli.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gcgsxsicr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gogynlnyd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/ggoksiugm.sHtML

[K07] 进制转换
来源：http://3g.yfazqb.com/Article/details/gwkukixhy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gksmehwev.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.epnwcf.com/Article/details/gwvzjivlg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gofnmrrui.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gewyoinku.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gvhszsqfh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/ggdkdvtkr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.yfazqb.com/Article/details/gkvgvubgu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gaxogrlbv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.bbcook.cn/Article/details/gpiwvbnub.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.bbcook.cn/Article/details/gxfrihird.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gsntvnrib.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/ggnrewhlq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/giaikqgcr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.bbcook.cn/Article/details/geekcvfgc.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/ghlgaoyol.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.epnwcf.com/Article/details/guqtjbjsu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.tarul.cn/Article/details/gcgfcpapu.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grcjuyddd.sHtML

L. 网络请求
来源：http://www.m.share.vehdjk.com/Article/details/ggxkvpkfo.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gydgscfkl.sHtML

[L01] 发送 GET 请求
来源：http://3g.sjlbkw.cn/Article/details/gwqtfsyow.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/ghocmtlur.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/gwsygxxnf.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gypschxad.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gcxzdzema.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.bbcook.cn/Article/details/gaqwjpvjh.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.bbcook.cn/Article/details/glemxkqem.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fktsv.cn/Article/details/gtwwjrquo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.epnwcf.com/Article/details/gqkznxhkq.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/gabgslgaj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gdmwdmwmp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.sjlbkw.cn/Article/details/gfdgtqoaz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gnkzlwuxd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gmjzhrigw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/gygxvsnbl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.tarul.cn/Article/details/giiplqbxd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.tarul.cn/Article/details/ggjjrxels.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/gmiqmhkxo.sHtML

[L03] 设置自定义请求头
来源：http://read.share.yfazqb.com/Article/details/gybmdupil.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fktsv.cn/Article/details/gzuwmcfod.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gykfkzftz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gncdgwxrq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/gcazxdqhl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/guzslxbhr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/grvtjyeii.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/gwgogbmli.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gerlvvgvx.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/gvgomdbab.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.yfazqb.com/Article/details/gakamdxgk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.bbcook.cn/Article/details/guczhaabq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/grszgzzew.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gjwkkhrte.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/giitnrlbl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.epnwcf.com/Article/details/gerekdwcp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/gygxfjljo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/gcfhkzexo.sHtML

[L05] 上传文件（multipart）
来源：http://blog.tarul.cn/Article/details/ghyspgkhe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gpnucoeoi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.bbcook.cn/Article/details/gvsqnfjgt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gexwltqqr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gknmkiodw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.sjlbkw.cn/Article/details/gpxgrrnxg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.yfazqb.com/Article/details/grbixtoky.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/glpzpziiq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.vehdjk.com/Article/details/gxizzjemx.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.vehdjk.com/Article/details/gkcxrguvl.sHtML

Py:   resp.json()
来源：http://read.share.fktsv.cn/Article/details/grqprrcco.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/gotydroth.sHtML

JS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gwbtnqoqf.sHtML

TS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gqqpuubwd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.tarul.cn/Article/details/gaipaysai.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.yfazqb.com/Article/details/glhwhldeo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fktsv.cn/Article/details/gbvwzltea.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fktsv.cn/Article/details/gkxuzgjxr.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/grjpngmzh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fktsv.cn/Article/details/gfbkybomc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.epnwcf.com/Article/details/gwsfrgdgt.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gypfhvzht.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gmrjjcbcd.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/garixsopd.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gbdpnjadv.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gnudjnenc.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gozlpjmoh.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/gsopbqlca.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gridqyucw.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.vehdjk.com/Article/details/gprdgznrp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gyvexjnxt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gixghxpnv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gyrjuyfjn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/guiirvaia.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.vehdjk.com/Article/details/gciedmlkk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/gwhyjsgxq.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gornabeor.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.epnwcf.com/Article/details/gwnpuquta.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtkabygh.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/ggajbnvql.sHtML

Py:   sys.argv[1:]
来源：http://wap.yfazqb.com/Article/details/gkbvjqcfb.sHtML

PHP:  $argv;  $argc;
来源：http://blog.vehdjk.com/Article/details/ghjojkysy.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/grrryvlab.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gctmzsreq.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/ghmldlmip.sHtML

Go:   os.Args[1:]
来源：http://read.share.vehdjk.com/Article/details/gkxbcqbrb.sHtML

Ruby: ARGV
来源：http://m.share.fktsv.cn/Article/details/gtfdvyrwq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.bbcook.cn/Article/details/grqdfyjyb.sHtML

[M02] 读取环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gmwsgnumm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fktsv.cn/Article/details/glfsavqre.sHtML


<!-- 参考信息 -->