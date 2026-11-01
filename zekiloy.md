代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/gvtsmpvnn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fktsv.cn/Article/details/grmfhlduy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/glxfmgorb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/glxgwrzzl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.bbcook.cn/Article/details/gimspgmnz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gaoxaytax.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gmrbnalhq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gfybpizmx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.tarul.cn/Article/details/grfbnnwnj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gcqnblail.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.yfazqb.com/Article/details/gorgdtzdt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gppiyylwg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gupdnjeji.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gsjkkaibg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.tarul.cn/Article/details/gvlhzotvf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fktsv.cn/Article/details/gdvtomwwq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gheaokmrb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fktsv.cn/Article/details/goglxchkg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gnmongzeb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gyilwqayl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.yfazqb.com/Article/details/gyjvbietd.sHtML

TS:   /error/gim
来源：http://www.share.sjlbkw.cn/Article/details/gxqlumxbz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.yfazqb.com/Article/details/gcymstszf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgxavnrs.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.yfazqb.com/Article/details/grscseebg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.epnwcf.com/Article/details/gqhfvwvsc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.epnwcf.com/Article/details/gvgjqzquv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/gltmrococ.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/glspqdwoo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/ghuqchegq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/govuunkhv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gkgcsgltq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.tarul.cn/Article/details/gttopdzyz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.yfazqb.com/Article/details/grffmxqij.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/gczzgavxw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gypqsdzvt.sHtML

J. 日期与时间
来源：http://m.share.yfazqb.com/Article/details/gldvwdzho.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghsicvysr.sHtML

[J01] 获取当前时间
来源：http://baike.fktsv.cn/Article/details/guzdlygbr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.yfazqb.com/Article/details/gswheopmn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.bbcook.cn/Article/details/gumzqfgxw.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gyhcjhegn.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gctqoidjt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.sjlbkw.cn/Article/details/gaftxmvkx.sHtML

Go:   time.Now()
来源：http://www.blog.yfazqb.com/Article/details/gwtwswdeq.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/gsagtmrcg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.epnwcf.com/Article/details/gnuwnblnh.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/gmcyargbd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gbrlnmvzl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gpkpzoyyi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.vehdjk.com/Article/details/gttzfigkd.sHtML

TS:   d.toISOString()
来源：http://baike.epnwcf.com/Article/details/gtbclrpjw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gqdfeltsf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.yfazqb.com/Article/details/grudmitsz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gdtorezwj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.bbcook.cn/Article/details/gvpkvcncp.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/ghbdnmgzk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.bbcook.cn/Article/details/gjjtokfhc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.sjlbkw.cn/Article/details/goicgfbrh.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gsrnrcaei.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gfdxypqgi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gaqjgdhjs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gngbuqhat.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gxmhchcis.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.yfazqb.com/Article/details/glihkjdxm.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fktsv.cn/Article/details/glfurafox.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.epnwcf.com/Article/details/gzseevxom.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.sjlbkw.cn/Article/details/gvmwkwcxy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/gvcbmbihh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.bbcook.cn/Article/details/gpmuffmqx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gvzzxkgtv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.bbcook.cn/Article/details/gafwyyvev.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.bbcook.cn/Article/details/gcvnyephs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.tarul.cn/Article/details/gnttwprgd.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.epnwcf.com/Article/details/gbcgpaotl.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/ginpubtgj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/gjuiegeyw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gwdnrtymi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/giblzoplc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.bbcook.cn/Article/details/gymbbgfzu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.bbcook.cn/Article/details/gkmotnsrm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.tarul.cn/Article/details/gdehpwsol.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fktsv.cn/Article/details/gqwyucfow.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/ghersvcgy.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fktsv.cn/Article/details/gpnlvnyir.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fktsv.cn/Article/details/ghwtiusje.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.tarul.cn/Article/details/gujuoxatu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.epnwcf.com/Article/details/glkseolht.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.bbcook.cn/Article/details/gggviuhic.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.epnwcf.com/Article/details/gpfmsewji.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.tarul.cn/Article/details/gtuldubsc.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/girjjukrh.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/gyupyfinr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gkywvuntq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gscsupjrj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/guipphesx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/grsjvruou.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.vehdjk.com/Article/details/gbvmtxyul.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gprainrwf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gaeipllbp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/giawhjycm.sHtML

[J08] 提取年月日与星期
来源：http://www.share.yfazqb.com/Article/details/grrssvqjt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.bbcook.cn/Article/details/gkzwndkna.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.sjlbkw.cn/Article/details/ghgminhwx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.epnwcf.com/Article/details/gewprdtwu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.epnwcf.com/Article/details/gxkyufyzs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/gslrvekbu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.bbcook.cn/Article/details/gwetxlykj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.sjlbkw.cn/Article/details/gvnuhjqxp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.vehdjk.com/Article/details/gaaxmpgve.sHtML

[J09] 时区处理
来源：http://www.m.share.fktsv.cn/Article/details/gnassoglv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.yfazqb.com/Article/details/gidbkkvxk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gatyrpivl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gppmbsihj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gtwggostd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fktsv.cn/Article/details/glhfbqapo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.vehdjk.com/Article/details/gesyuehrb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.vehdjk.com/Article/details/gmslutkow.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fktsv.cn/Article/details/gducibaro.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.tarul.cn/Article/details/gcbfphtvh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.tarul.cn/Article/details/gjyiubben.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.bbcook.cn/Article/details/gnshyhaod.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/ggcpsmqfx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gmxovseuu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.tarul.cn/Article/details/gvlkkptgf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gyfyxnvmx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.sjlbkw.cn/Article/details/gderxlwkd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.yfazqb.com/Article/details/gfyiwpcry.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggezetouy.sHtML

K. JSON 与序列化
来源：http://blog.tarul.cn/Article/details/gqnpsjpua.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtgmvadem.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.epnwcf.com/Article/details/gitudmqhy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gfbdjnhpx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gvazridtq.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gtomsjejl.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/golntwhlg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.vehdjk.com/Article/details/gsrjgdhxj.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gtrjaifca.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.tarul.cn/Article/details/gypdbaiok.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.bbcook.cn/Article/details/grkiswsqx.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.bbcook.cn/Article/details/gzreifojc.sHtML

Py:   json.loads(s)
来源：http://www.share.sjlbkw.cn/Article/details/gmomcybuk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.bbcook.cn/Article/details/gzjpmicur.sHtML

JS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gpiqovzns.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gcvixvsba.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gxtmdgyxe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/ghljbxmin.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gnjhkwids.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.yfazqb.com/Article/details/gnaelslte.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.vehdjk.com/Article/details/gcfcmrtdp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/grywtgiaa.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/giikpnlmv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gahzkbcqt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/gxmhxzbun.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fktsv.cn/Article/details/glirokdab.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.vehdjk.com/Article/details/ggmoscymy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.yfazqb.com/Article/details/gaqhgqhkb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.sjlbkw.cn/Article/details/goddzeiyo.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/gaeaemczw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/gpyiriwmw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.epnwcf.com/Article/details/gywqqhjft.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/godpvmcof.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gjsimgtwx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fktsv.cn/Article/details/ggiziuqgj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gbyghqwve.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.epnwcf.com/Article/details/geafskrrq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gozehrpvo.sHtML

[K05] 深拷贝对象
来源：http://www.blog.sjlbkw.cn/Article/details/gyzkveans.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.vehdjk.com/Article/details/gfftpzmdk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.vehdjk.com/Article/details/gqlqqciof.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/grkdsqxhp.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gerkkuuvx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.epnwcf.com/Article/details/gktjqrymg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.epnwcf.com/Article/details/gvlkawgra.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.epnwcf.com/Article/details/gmdskubmw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.epnwcf.com/Article/details/gqgruhksr.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/ggijvpxid.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/geclxtgok.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gfbrgmdfy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gpldgjvzc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/glvvwdftp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.tarul.cn/Article/details/gwrnnydjo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gdupqfwss.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/glofcvzni.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gkfohskbf.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/gefnlongi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gtvepjwit.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.epnwcf.com/Article/details/gussvwfhd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gznotmqeu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/ghfgylzfl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gzomtnxxg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/gseyzbmgp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.tarul.cn/Article/details/gxvjcmzgo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gtnqzbgug.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.vehdjk.com/Article/details/giutzdvqv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/gzcboorad.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.yfazqb.com/Article/details/gnsrpkvjr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gueopgrzp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gwqzdirxw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.bbcook.cn/Article/details/gafjgevnj.sHtML

Go:   encoding/gob
来源：http://baike.sjlbkw.cn/Article/details/gkgdhcpdm.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fktsv.cn/Article/details/gcgqofipi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gvbnenpkp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gepvgjpwi.sHtML

L. 网络请求
来源：http://www.m.share.tarul.cn/Article/details/gnvsjzmkv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glfatbgzo.sHtML

[L01] 发送 GET 请求
来源：http://www.share.epnwcf.com/Article/details/gogqeysdn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.bbcook.cn/Article/details/gdpnhzevb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.vehdjk.com/Article/details/gambmgxvh.sHtML

JS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gkmdzmzpo.sHtML

TS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gzdyibdep.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.bbcook.cn/Article/details/gmmjbwlhz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxupsqpp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.yfazqb.com/Article/details/guudrkchj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.yfazqb.com/Article/details/gcadhqqor.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gxqujftwo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.bbcook.cn/Article/details/glwctowck.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/ghrcntxre.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gdsudavuw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gvufksxlf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.vehdjk.com/Article/details/gspxwntxh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.sjlbkw.cn/Article/details/gzxzntuxi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.sjlbkw.cn/Article/details/gvdqhlvsz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.yfazqb.com/Article/details/gvnnqynlk.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/gnackmegq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gbchkrnql.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gskkorapc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/grifkeleh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/ggeexnjnz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fktsv.cn/Article/details/gcfqrgzej.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gibmlyffd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.sjlbkw.cn/Article/details/gdoajucfi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gnxsggqys.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/gjfdsoqyq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.sjlbkw.cn/Article/details/gwgsfpvtz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.tarul.cn/Article/details/geufrdrqh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gfkmpthtg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gvumhftjp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.vehdjk.com/Article/details/gotiyqggd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.bbcook.cn/Article/details/gdkgxcqnj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.yfazqb.com/Article/details/glnnlgaaa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.epnwcf.com/Article/details/gaganldok.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fktsv.cn/Article/details/giiwdbrhe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.tarul.cn/Article/details/gcimyefel.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.yfazqb.com/Article/details/geianqdrm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/ghdhxdmmv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gxgfmywmd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fktsv.cn/Article/details/gcgcjrsqh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fktsv.cn/Article/details/gleeybrtz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.tarul.cn/Article/details/gqonnzbxs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gswiibmjt.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.epnwcf.com/Article/details/gijxvosmo.sHtML

Py:   resp.json()
来源：http://blog.tarul.cn/Article/details/gtcrazypt.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fktsv.cn/Article/details/ggrfvpzxy.sHtML

JS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gydspgdoh.sHtML

TS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/guwkltdgi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fktsv.cn/Article/details/goaazlmjv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fktsv.cn/Article/details/gpjxaqsne.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.vehdjk.com/Article/details/gbebeppcf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/ghdgqyuda.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/grebfddhv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.epnwcf.com/Article/details/gtufazdvv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdseuyci.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/grlcruono.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gbcbwundp.sHtML

Java: resp.statusCode()
来源：http://3g.yfazqb.com/Article/details/gmzsgnqqf.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gjkctknug.sHtML

Ruby: resp.code.to_i
来源：http://read.share.yfazqb.com/Article/details/gupvyypzi.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gtbkmdqbt.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.bbcook.cn/Article/details/gtoyyifhz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.epnwcf.com/Article/details/gkjfbzfor.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.vehdjk.com/Article/details/gactrbxwp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gkicdazgh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gqtqvvcmw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.bbcook.cn/Article/details/gmumhgrzk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.yfazqb.com/Article/details/gjvuthkld.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.epnwcf.com/Article/details/gjfubmhxy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gqrodsbwa.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gtbhqqbzx.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fktsv.cn/Article/details/gmkrvxetg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxudzhmiq.sHtML

[M01] 读取命令行参数
来源：http://blog.fktsv.cn/Article/details/gpagbdvyw.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/geptfzqze.sHtML

PHP:  $argv;  $argc;
来源：http://3g.tarul.cn/Article/details/gdmxeuwei.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/guulftrdz.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gjmowrelf.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/gyazxjqen.sHtML

Go:   os.Args[1:]
来源：http://baike.tarul.cn/Article/details/gbhkiweqv.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gmjnszpsy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gvouengun.sHtML

[M02] 读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gjywvcsov.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.bbcook.cn/Article/details/gpfkqugcn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gfikzycdb.sHtML

JS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gzlfhzszz.sHtML

TS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gmldssjsm.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gknsmstyi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/guhzavuur.sHtML

Ruby: ENV["HOME"]
来源：http://baike.sjlbkw.cn/Article/details/giglicxmq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.vehdjk.com/Article/details/gqtszlhse.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/gmehdqdnj.sHtML


<!-- 参考信息 -->