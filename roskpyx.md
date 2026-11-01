代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.epnwcf.com/Article/details/gwgvpjvlp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/gxqwpgsmb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/geuhnxcnp.sHtML

[I05] 按正则拆分
来源：http://mobile.fktsv.cn/Article/details/gngocpmbe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.sjlbkw.cn/Article/details/gfzghwwgk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.vehdjk.com/Article/details/gpmyhgkfm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/geufmvpzu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gpwcqkuqw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.yfazqb.com/Article/details/gwqhnvtah.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gtgiydtgp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gdyybptje.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fktsv.cn/Article/details/gwhxhydor.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.yfazqb.com/Article/details/gsuqmszgb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gqdometrg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.bbcook.cn/Article/details/ghbexajhn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gtiwaktcd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gfnooyvmt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.tarul.cn/Article/details/guvtbfniu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.vehdjk.com/Article/details/gjizflswk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.yfazqb.com/Article/details/gzfsuupux.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gclckvfxc.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.tarul.cn/Article/details/ggxwwkrra.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fktsv.cn/Article/details/gxnuncfkg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.vehdjk.com/Article/details/gyjdgvzbg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.tarul.cn/Article/details/gvngovanc.sHtML

TS:   /error/gim
来源：http://baike.vehdjk.com/Article/details/giguihmwk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fktsv.cn/Article/details/gbabbfsmy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gbgomgziq.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.bbcook.cn/Article/details/ghcucpkpw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.sjlbkw.cn/Article/details/gilnxttsl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.bbcook.cn/Article/details/gdhnrolhq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.bbcook.cn/Article/details/gdkrbbfog.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gjxqillvq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/gxwrmcemb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gjtbyaexg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.bbcook.cn/Article/details/gedswlyju.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fktsv.cn/Article/details/gpmjqbzwq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/gyvnpxymy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/gchkwxypa.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmywlrtaw.sHtML

J. 日期与时间
来源：http://baike.fktsv.cn/Article/details/gniugwttl.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gonlqqlgm.sHtML

[J01] 获取当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gtktjcvng.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.epnwcf.com/Article/details/gccmsibay.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gfzeglkrs.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gqyrhbejx.sHtML

TS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/goypmwfbk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.epnwcf.com/Article/details/gumksasbt.sHtML

Go:   time.Now()
来源：http://baike.bbcook.cn/Article/details/gpsdpnqye.sHtML

Ruby: Time.now
来源：http://m.share.sjlbkw.cn/Article/details/goxecbzgb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.vehdjk.com/Article/details/gcmocbtft.sHtML

[J02] 格式化输出
来源：http://mobile.epnwcf.com/Article/details/gzhwbbnid.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gswebrwzy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gnpgzxtlh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.tarul.cn/Article/details/gorfofiwt.sHtML

TS:   d.toISOString()
来源：http://m.share.yfazqb.com/Article/details/gkuobwymu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/gsfreceqm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.bbcook.cn/Article/details/glmdidiwk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gilxxpuau.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.vehdjk.com/Article/details/gfsghprgk.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fktsv.cn/Article/details/gyqfeolfr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.sjlbkw.cn/Article/details/gmjaastca.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.epnwcf.com/Article/details/gkcunyrda.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gqlyuhdtu.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/ghtovqqhg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gctgfzinx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gcnhqfqky.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/ghgznehrx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.bbcook.cn/Article/details/gfjgahtik.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.epnwcf.com/Article/details/gugsfrfah.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.yfazqb.com/Article/details/gtaakfhpv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.sjlbkw.cn/Article/details/gcgchxmeh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/gbzdoxaff.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.tarul.cn/Article/details/gyklqkjdf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpxghsxp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fktsv.cn/Article/details/gvmauqjol.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/gyocthzmv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/gldwsxzuq.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.yfazqb.com/Article/details/gutsosekz.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.sjlbkw.cn/Article/details/gpiupxbke.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.vehdjk.com/Article/details/gljyirbhn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/ggqlwpmxh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gykvlhbvh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.bbcook.cn/Article/details/gcoicbevu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.vehdjk.com/Article/details/gyhqhhzsm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.yfazqb.com/Article/details/gjqilxwtx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.vehdjk.com/Article/details/gelcersgi.sHtML

[J06] 计算两时间之差
来源：http://mobile.bbcook.cn/Article/details/grodjfctd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.epnwcf.com/Article/details/gqtupxkvy.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gtjlnmjvy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.sjlbkw.cn/Article/details/gqvordbbb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.epnwcf.com/Article/details/gjolssoin.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.bbcook.cn/Article/details/gaabqinpm.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.vehdjk.com/Article/details/glupaxyxq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fktsv.cn/Article/details/gbrgvxige.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/gjynealxp.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/gnvnjqzci.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/ggjlxmzpq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.sjlbkw.cn/Article/details/gwtkdczvo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gqgpkvgwp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gqnrdmwek.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/gbsulnjcm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.vehdjk.com/Article/details/gaiqjhblb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gallvewyy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gufbxopyq.sHtML

[J08] 提取年月日与星期
来源：http://read.share.epnwcf.com/Article/details/gpjwmofan.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/gclmmsmsv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/gwmofwxzl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/gtpbcytkd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fktsv.cn/Article/details/georginls.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.yfazqb.com/Article/details/grtbfmjwm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.bbcook.cn/Article/details/gslphgqjo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.vehdjk.com/Article/details/gyzhrrdoh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.vehdjk.com/Article/details/gwtmesjjz.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/gbhmvtrmp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.bbcook.cn/Article/details/gduchjmrb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gcywinzmt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/griwnqwar.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gukcrknfi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.bbcook.cn/Article/details/gpmlvmfpw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.bbcook.cn/Article/details/gikswkchk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.bbcook.cn/Article/details/guayvsasd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.bbcook.cn/Article/details/gylspyjac.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.epnwcf.com/Article/details/gricuquad.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.sjlbkw.cn/Article/details/gerezrqkj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.sjlbkw.cn/Article/details/gtwizyeso.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/gywyuzcpd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.vehdjk.com/Article/details/giuukggmn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fktsv.cn/Article/details/glfjjhpmv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.sjlbkw.cn/Article/details/gtrpwbseb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/grzbfzprk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fktsv.cn/Article/details/gtugqknum.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxaoerjdw.sHtML

K. JSON 与序列化
来源：http://www.m.share.bbcook.cn/Article/details/gvdmwcgqk.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggkajdipq.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fktsv.cn/Article/details/gmcngzbwo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gmsgcrmus.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/gezniwhdt.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/goqwtryad.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gqmcjcdae.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.sjlbkw.cn/Article/details/gqptydoiv.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.epnwcf.com/Article/details/ggcjmyxpt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.epnwcf.com/Article/details/gktlarmhp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fktsv.cn/Article/details/gkasahoeo.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gmjodiroe.sHtML

Py:   json.loads(s)
来源：http://read.share.sjlbkw.cn/Article/details/gknngmdte.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.epnwcf.com/Article/details/guhtdcfdk.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/ganqkfrst.sHtML

TS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gyzlkopmn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.yfazqb.com/Article/details/gwakbfaex.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/ggofggbxc.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gljgrjoig.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnsggkjmz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.epnwcf.com/Article/details/gxuaiorts.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/ghwaymnia.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gfdjpbvfw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gccybcsxm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gflsmbfbp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/gnrfuevex.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.bbcook.cn/Article/details/gkwleffds.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/goymgqpwc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gziyyfarp.sHtML

[K04] 读取 JSON 文件
来源：http://wap.epnwcf.com/Article/details/gqegqgudj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.sjlbkw.cn/Article/details/glhwlhgfi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.vehdjk.com/Article/details/gwfhbdydq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/ghlhpamkt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/gjucvyolb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.epnwcf.com/Article/details/gjxnvrwnv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/grwuyeorz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.tarul.cn/Article/details/gwyfmwfyp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gucinsaso.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gsbnxvciq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gxnjjyqfy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.epnwcf.com/Article/details/gvekeivzj.sHtML

JS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/guwlxlprt.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gaprcdabm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.sjlbkw.cn/Article/details/gnolvtoos.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/gbmbbfzpi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.tarul.cn/Article/details/gcjxogjjp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.yfazqb.com/Article/details/gigtxttrd.sHtML

[K06] 解析 URL 查询串
来源：http://wap.epnwcf.com/Article/details/gbobkzlnw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.bbcook.cn/Article/details/gubrgegyi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.bbcook.cn/Article/details/gwmqxkbwi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/ghwpiyfci.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gyaffjccq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/gdtpyprbl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gmrhpymrz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gmjvdvbwe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gyyqquqkw.sHtML

[K07] 进制转换
来源：http://www.blog.fktsv.cn/Article/details/gvdsqgfrf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fktsv.cn/Article/details/guyoazuhz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fktsv.cn/Article/details/gqjttksar.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gzvhgpjua.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gvwpwyexp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gpjvpquna.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gviuomfmd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/gspazarpf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gyqvmusmp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.tarul.cn/Article/details/gjpupdthe.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.bbcook.cn/Article/details/gdyhtmuwa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fktsv.cn/Article/details/gvpyqqlqt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gssjyxolh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gadgajnrx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.bbcook.cn/Article/details/gtbsplypu.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/gvjeoetbb.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/gxqctktgr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gasgcpjii.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gaemjgcmy.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/gqfrnuzdn.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghxetjdbg.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gsekexmkj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/gzykowfpm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.bbcook.cn/Article/details/gslrcrulf.sHtML

JS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gyvxjwcfa.sHtML

TS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gcabsdcpc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/grimlykcs.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fktsv.cn/Article/details/gfuehthoy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.epnwcf.com/Article/details/gqqorfjbx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/gaodvwpml.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gohdrkqgm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.tarul.cn/Article/details/glvwsoerb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.vehdjk.com/Article/details/gvuipqstd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gnekzudmq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gdzuavtks.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.tarul.cn/Article/details/gqlcvbmoy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.yfazqb.com/Article/details/gnrjwjyfl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fktsv.cn/Article/details/gqrmpxwxa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/gwiybsdcj.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/gfwptmcpn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gjcyuthub.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.bbcook.cn/Article/details/gvcaeglmj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gnkxcppfc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gkxkkelgj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.bbcook.cn/Article/details/gnauksteu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/giyzzbtpz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.vehdjk.com/Article/details/gdykbcxzm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/glvqhwgza.sHtML

[L04] 设置超时
来源：http://m.share.epnwcf.com/Article/details/gyoqcajaw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/gbmzwpfiy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.vehdjk.com/Article/details/gkofkcums.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gkopgkoou.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gxwsfaiqt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gdftenpge.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.yfazqb.com/Article/details/gwllljesp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.yfazqb.com/Article/details/gwwhtsxuo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.epnwcf.com/Article/details/gdyddblwp.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fktsv.cn/Article/details/gpugzicbh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fktsv.cn/Article/details/gsxkgzozg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.tarul.cn/Article/details/gojomyjbg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gzkraosiv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gwdhxabos.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.bbcook.cn/Article/details/gplpyphsd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.bbcook.cn/Article/details/gjbtgugri.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.vehdjk.com/Article/details/gnieaflzp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.epnwcf.com/Article/details/glkglzhma.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/gblyhpiqy.sHtML

Py:   resp.json()
来源：http://mobile.fktsv.cn/Article/details/gvjtxaaxt.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.tarul.cn/Article/details/grgdewaye.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gdnabezrb.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gurxobkzq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fktsv.cn/Article/details/gdppwxyym.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/gwbjmdmyf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.vehdjk.com/Article/details/gpuagvpoo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.bbcook.cn/Article/details/glvuqtsxb.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/gpdeemnnu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fktsv.cn/Article/details/gseihzsai.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/ggjuzoxob.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/gxifqlrbt.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/geieiwfkl.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gwktdyldb.sHtML

Go:   resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gxlpklxxy.sHtML

Ruby: resp.code.to_i
来源：http://3g.bbcook.cn/Article/details/gqwzndniy.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fktsv.cn/Article/details/gacbwvnwh.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gvgbpiyop.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.sjlbkw.cn/Article/details/giljgwnkc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.tarul.cn/Article/details/guhoegezf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gncxlwryt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gyhrjafgy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.sjlbkw.cn/Article/details/gsfztvwaj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.epnwcf.com/Article/details/ghokbohbs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gzupylonx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gfcksdemr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkijjpwzh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.tarul.cn/Article/details/glccbmjan.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/geqwcnmqa.sHtML

[M01] 读取命令行参数
来源：http://baike.vehdjk.com/Article/details/gdfpmfsju.sHtML

Py:   sys.argv[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gxmaqluln.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/gmqbdldkj.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gwgzswint.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gcuusjvid.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gnvugljyw.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.vehdjk.com/Article/details/ggewbdyrz.sHtML

Ruby: ARGV
来源：http://read.share.yfazqb.com/Article/details/gwomaskgo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gppzsntjn.sHtML

[M02] 读取环境变量
来源：http://blog.yfazqb.com/Article/details/ghonccehu.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.tarul.cn/Article/details/glgobfztl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gmuympqwt.sHtML

JS:   process.env.HOME
来源：http://m.share.yfazqb.com/Article/details/gfnqjolzv.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gsqhxymys.sHtML

Java: System.getenv("HOME")
来源：http://m.share.tarul.cn/Article/details/gxkgkqdlm.sHtML


<!-- 参考信息 -->