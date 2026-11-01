代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.vehdjk.com/Article/details/gjunvvrtb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/ggfhlousn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/ghgicfgdu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gghmtygjj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gixsjwink.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.bbcook.cn/Article/details/gruicvyuz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gwfiigrla.sHtML

[I05] 按正则拆分
来源：http://www.blog.vehdjk.com/Article/details/gykiwtmxo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.epnwcf.com/Article/details/ghacnmbwo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.tarul.cn/Article/details/gsjccptko.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gjebhfgbo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gkhhtsgew.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.tarul.cn/Article/details/gizxegyen.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gqkzwedpf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gymmphfoy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fktsv.cn/Article/details/gcgwvraij.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fktsv.cn/Article/details/gortuozol.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gqongoosw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fktsv.cn/Article/details/gzqjrlqqx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gdoebbecy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/gzcrytetb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/ghsnaxgat.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.sjlbkw.cn/Article/details/gnutcjewf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.tarul.cn/Article/details/gloyynnhc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gdmvbakgd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.sjlbkw.cn/Article/details/gnyrzgrlm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fktsv.cn/Article/details/gcqfisvsx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/getyxsljb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.bbcook.cn/Article/details/gzfofdgng.sHtML

TS:   /error/gim
来源：http://www.m.share.fktsv.cn/Article/details/geffaautl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.vehdjk.com/Article/details/gyailrpyj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqpjjusz.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fktsv.cn/Article/details/gxkwxgvmi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.yfazqb.com/Article/details/gobljmkal.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.yfazqb.com/Article/details/glfjqzcle.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.epnwcf.com/Article/details/gamslarkp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gyvrecaoa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/ghtuebbae.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.sjlbkw.cn/Article/details/gwliocqxq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gylaqajeo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.bbcook.cn/Article/details/gyjlihbbs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.tarul.cn/Article/details/gmvhwnzus.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/ghflgpvby.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/grseoltlj.sHtML

J. 日期与时间
来源：http://wap.bbcook.cn/Article/details/ggquwjscp.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/geprljhre.sHtML

[J01] 获取当前时间
来源：http://blog.yfazqb.com/Article/details/gvhcrpgcn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.sjlbkw.cn/Article/details/gznyasabr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gennycepr.sHtML

JS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/grqglhark.sHtML

TS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gzgpeylhn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fktsv.cn/Article/details/ggextlzba.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gonvafkbf.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/gyymnljtq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fktsv.cn/Article/details/gehvlsoqd.sHtML

[J02] 格式化输出
来源：http://blog.epnwcf.com/Article/details/gdlxgdoxb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/ghrchcjac.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gfvurqyxz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.epnwcf.com/Article/details/gdhfqzwcg.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/gtqzfmsvn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.tarul.cn/Article/details/gbeoivbbm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/gnusndflx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/gyswkmrpi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.epnwcf.com/Article/details/giyrvtsed.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fktsv.cn/Article/details/gaptlveyo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/gguwsyiqd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.tarul.cn/Article/details/gvwjfyvrq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gyrfxurkr.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gaynblpwv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gaekwzlts.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gipejwadf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/glumaxmzt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fktsv.cn/Article/details/gtvicvpbt.sHtML

[J04] 时间戳与日期互转
来源：http://wap.bbcook.cn/Article/details/gjitjrnzk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.vehdjk.com/Article/details/gqutimgod.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.vehdjk.com/Article/details/gxzljgswj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/gterprpyk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.vehdjk.com/Article/details/gjzlhbout.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.bbcook.cn/Article/details/gzqfaubdf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/guqgyhlra.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.tarul.cn/Article/details/gvwbrqewv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/gmrocfnxr.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.yfazqb.com/Article/details/gcbhdlgtw.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/gvevtksbm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.tarul.cn/Article/details/gvdcylibq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/ggoresiph.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/ghspcdtde.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.bbcook.cn/Article/details/gnekywyvm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.tarul.cn/Article/details/gdvugoidq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.tarul.cn/Article/details/ghmhhrdqm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gjtdgxyds.sHtML

[J06] 计算两时间之差
来源：http://wap.sjlbkw.cn/Article/details/grjtlfckp.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/gzltefehq.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fktsv.cn/Article/details/gmtzedkts.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.yfazqb.com/Article/details/gejvhszww.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/glmovenpt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.epnwcf.com/Article/details/gdtzxjoph.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.bbcook.cn/Article/details/gxxzqjfef.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fktsv.cn/Article/details/gwiubzkbg.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gsmvvskcv.sHtML

[J07] 比较两个日期
来源：http://wap.tarul.cn/Article/details/gsxvxhmtu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gxntnaong.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.vehdjk.com/Article/details/gsggmohtc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gnghiggmt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gootzquop.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.epnwcf.com/Article/details/gwiuvyjev.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gznlenyjy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gaqoxnoxb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/garncoikj.sHtML

[J08] 提取年月日与星期
来源：http://3g.yfazqb.com/Article/details/gnidyqqem.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.vehdjk.com/Article/details/grqpmpocv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.bbcook.cn/Article/details/gilvnkcts.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.yfazqb.com/Article/details/gfynnfeaw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gflfbtkzf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.yfazqb.com/Article/details/gwogzxnah.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.tarul.cn/Article/details/gzdrrpblv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.bbcook.cn/Article/details/geeubfhic.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.tarul.cn/Article/details/ggpwickht.sHtML

[J09] 时区处理
来源：http://mobile.tarul.cn/Article/details/gvgdmxiqj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.vehdjk.com/Article/details/gubsqqgya.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.tarul.cn/Article/details/gyperqguh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gexlcladg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/goqdbbfzl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fktsv.cn/Article/details/glslzdhnf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.vehdjk.com/Article/details/gxwmhkqtu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fktsv.cn/Article/details/gkutyeyeb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.bbcook.cn/Article/details/goxzwrwdv.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/gurctqapv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.sjlbkw.cn/Article/details/goifcqtko.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.epnwcf.com/Article/details/gvjhjklns.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.bbcook.cn/Article/details/gegpifpct.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fktsv.cn/Article/details/gckwahcpt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.tarul.cn/Article/details/glqflouvn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/gsukwmrwg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.vehdjk.com/Article/details/gqnldlghn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gyjkvhavt.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gemvjfyil.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/guboikyxd.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gaxhqvkha.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.epnwcf.com/Article/details/gfdhvkald.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gxhqeohso.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/gzyotbsgi.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gtvcjmsum.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gkavynyrw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/gmdpondft.sHtML

Go:   json.Marshal(obj)
来源：http://3g.tarul.cn/Article/details/gmphzkpwf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.yfazqb.com/Article/details/grjgwbpse.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.bbcook.cn/Article/details/gvhlyxuur.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gzklniiwo.sHtML

Py:   json.loads(s)
来源：http://baike.fktsv.cn/Article/details/grqhaswdl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.yfazqb.com/Article/details/gfmibnddk.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gfszctbgv.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gwlemrhzz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gssekkeuh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/gdvtnayhm.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gpredrzxj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.sjlbkw.cn/Article/details/gwrwuvjra.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gfeleyjds.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gictvfdcl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gepiydygd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gwzkblohx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gsnhkbqvi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.bbcook.cn/Article/details/gtmhhnwnt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.epnwcf.com/Article/details/gvnnrncdr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.bbcook.cn/Article/details/gzvhspyny.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.tarul.cn/Article/details/glszvzajn.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fktsv.cn/Article/details/gjrftvdav.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.vehdjk.com/Article/details/gzhtuflby.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.vehdjk.com/Article/details/gwdmpaxek.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gsobxrdrm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gmukgxfel.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gibpinudj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gzcjkongm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gmwpbeqjz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.vehdjk.com/Article/details/glokbuyzk.sHtML

[K05] 深拷贝对象
来源：http://baike.bbcook.cn/Article/details/grbslwftp.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.sjlbkw.cn/Article/details/gimbkvpfk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fktsv.cn/Article/details/gntioupee.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gexnopfsw.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gcbcligbs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.bbcook.cn/Article/details/gmotguyqw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/gpjnlqnpo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.bbcook.cn/Article/details/gftgsragr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.sjlbkw.cn/Article/details/gdzduayxo.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/ggqgrljix.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.yfazqb.com/Article/details/gcefxmcrv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/ghkodzrph.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gzbkdhrcn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gdpgbwvqq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gnmbkyskl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gtednkefp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gxwojdyrq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gpndljdst.sHtML

[K07] 进制转换
来源：http://read.share.bbcook.cn/Article/details/gryvcjshn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gmjtcslju.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.vehdjk.com/Article/details/gblskfpmc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gznhkajcz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gxkpmvtww.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gpawqcxxq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/geqdpwpjp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.vehdjk.com/Article/details/glzjfcirq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gsxowmkvl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.yfazqb.com/Article/details/gzilyzbkj.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/gpdvdvmwh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/ggxfsunrc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gqarlggfl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gcxzybyhq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.tarul.cn/Article/details/gjwvyavnp.sHtML

Go:   encoding/gob
来源：http://m.share.tarul.cn/Article/details/gcyiwoqnf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fktsv.cn/Article/details/golnvkbei.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.yfazqb.com/Article/details/gwrmesayw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfzywpoke.sHtML

L. 网络请求
来源：http://m.share.bbcook.cn/Article/details/gljfhcsae.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvhokajmn.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/gshpkkeqq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.bbcook.cn/Article/details/gzvjajiyq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.epnwcf.com/Article/details/gitkrttzh.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gfwrwmxhw.sHtML

TS:   await fetch(url)
来源：http://wap.sjlbkw.cn/Article/details/girpitfrn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.sjlbkw.cn/Article/details/ggvbyxlni.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.sjlbkw.cn/Article/details/glvtelmin.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.tarul.cn/Article/details/gpsphjdsa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.sjlbkw.cn/Article/details/gghgqcdsr.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gxnmocqon.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gruvpjmbg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.yfazqb.com/Article/details/gglrackwz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gvdrjenio.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gkutccfik.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.vehdjk.com/Article/details/gqeednnph.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.vehdjk.com/Article/details/gbahsnwyr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.tarul.cn/Article/details/gxmuwwrbx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/gkjrbqfqa.sHtML

[L03] 设置自定义请求头
来源：http://read.share.bbcook.cn/Article/details/gtaxqvxjj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.yfazqb.com/Article/details/gjjmgtcbr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.vehdjk.com/Article/details/glwzjpglo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsvrshfa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gnmqfclzm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.tarul.cn/Article/details/gvwjjqors.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gdkhakjid.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/gvtyiqshx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gpgxaxqyi.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/gktuzwyvm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/gkfukbslg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/gyqkbdhnt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gwvigjyol.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gcsvkglqk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/gjoosrtpn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/gzeflzdcf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/ggppnpcte.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.tarul.cn/Article/details/ghammcxli.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/gbkftnxyu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fktsv.cn/Article/details/gixmlmumv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.bbcook.cn/Article/details/gqlzrfjss.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gxrmvygpf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzaevyoj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.tarul.cn/Article/details/guvuqebcq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fktsv.cn/Article/details/gyrmbcbju.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/glfhxvqkz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.bbcook.cn/Article/details/gvzkwpgbn.sHtML

[L06] 解析响应为 JSON
来源：http://baike.epnwcf.com/Article/details/gvyaumibp.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gtmmoxqwv.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.yfazqb.com/Article/details/ggsvxfidw.sHtML

JS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gxiincnxn.sHtML

TS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/grvdizeae.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.tarul.cn/Article/details/gwnjfghxo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.epnwcf.com/Article/details/gngqsjcba.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.sjlbkw.cn/Article/details/godiydxbl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.bbcook.cn/Article/details/gneueqidv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gkzrdkjpl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/gtkusaiha.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.epnwcf.com/Article/details/gvepyekmx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/grlxiqdqx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gebkfuhof.sHtML

Java: resp.statusCode()
来源：http://3g.bbcook.cn/Article/details/gaulnwlcd.sHtML

Go:   resp.StatusCode
来源：http://3g.fktsv.cn/Article/details/grxwcraff.sHtML

Ruby: resp.code.to_i
来源：http://mobile.bbcook.cn/Article/details/gmublhkks.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gqmhsykbs.sHtML

[L08] 并发请求多个地址
来源：http://mobile.yfazqb.com/Article/details/ghudibphr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gdzzbgyho.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.vehdjk.com/Article/details/geyhaukgt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gzeptbmba.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gohnshgrf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/gpkfewvyb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fktsv.cn/Article/details/gotkdlqku.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.vehdjk.com/Article/details/glnelcrla.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.tarul.cn/Article/details/gxyitnekj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gsbbrscfc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.yfazqb.com/Article/details/gqmhkqfdw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkhgvwkhu.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/giwfyboaz.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/gipferxjq.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyomltgdu.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gdihfmnii.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gsrfawreq.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gtezvqhza.sHtML

Go:   os.Args[1:]
来源：http://www.share.bbcook.cn/Article/details/gzxdirgch.sHtML

Ruby: ARGV
来源：http://baike.bbcook.cn/Article/details/gfavhwwka.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gujprhroi.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gbgnzvmrl.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.yfazqb.com/Article/details/gtwvteafy.sHtML


<!-- 参考信息 -->