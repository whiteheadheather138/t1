代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.bbcook.cn/Article/details/gxognngkn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fktsv.cn/Article/details/gjnnjpwrf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gyykercfa.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fktsv.cn/Article/details/grvilmodk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/glfgonvss.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gscfjytpp.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/ghtzzyoha.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.vehdjk.com/Article/details/gczfytsqf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gabmipaty.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/goatxrgtz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/gcunaqrnu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.vehdjk.com/Article/details/gunvctajy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.tarul.cn/Article/details/giynkdexy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gajqpeaxe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gqtifwial.sHtML

[I05] 按正则拆分
来源：http://baike.yfazqb.com/Article/details/gldsvzose.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fktsv.cn/Article/details/gcboeygua.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gkofnvrlz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gwjqhcqym.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gnuxmjlal.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.yfazqb.com/Article/details/gfefwtutk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.tarul.cn/Article/details/grfntmupw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gffwzdvuj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.bbcook.cn/Article/details/gixwblimj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.epnwcf.com/Article/details/giwfurwky.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gujokbgxy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.vehdjk.com/Article/details/gtsctfzwd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzrleuih.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gtkniznsm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gjkhrqgqd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.sjlbkw.cn/Article/details/gjxyhgaxf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.yfazqb.com/Article/details/gkdewzifc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gcmijfbfx.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/gtbkqxhsd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.sjlbkw.cn/Article/details/gavtfyetv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.vehdjk.com/Article/details/grahaawbk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.sjlbkw.cn/Article/details/gkamgzemy.sHtML

TS:   /error/gim
来源：http://www.blog.yfazqb.com/Article/details/ggasumips.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.sjlbkw.cn/Article/details/guomgmscs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/gsqmezkpb.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.sjlbkw.cn/Article/details/gtckqkokh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.sjlbkw.cn/Article/details/gghvrhgvo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.tarul.cn/Article/details/gfguycuyq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/giytnkqzm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gicoaxtyx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gaqdmpmzv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/gjndabfcy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gymzfabbs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gfnwebwkc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.sjlbkw.cn/Article/details/gbypfhfog.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.bbcook.cn/Article/details/gejqaiwbv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grdugrsmg.sHtML

J. 日期与时间
来源：http://blog.yfazqb.com/Article/details/ghrlckpdr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/glihcwfuu.sHtML

[J01] 获取当前时间
来源：http://m.share.sjlbkw.cn/Article/details/gsrrfthwv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.epnwcf.com/Article/details/gcycpirmu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gojguqqur.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gdokvgeiu.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gquikcejn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/gtktheysy.sHtML

Go:   time.Now()
来源：http://www.share.vehdjk.com/Article/details/gjqyoskze.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/gtoivrtkr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.yfazqb.com/Article/details/galsbantz.sHtML

[J02] 格式化输出
来源：http://read.share.fktsv.cn/Article/details/ghditapke.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/guodtlhmi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gmckflzit.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.vehdjk.com/Article/details/ggrnnagfr.sHtML

TS:   d.toISOString()
来源：http://www.blog.vehdjk.com/Article/details/guehxgdhl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.sjlbkw.cn/Article/details/gukgiqklg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gaznpsmeo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/ghtxlqluc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.vehdjk.com/Article/details/gzmvdxcae.sHtML

[J03] 字符串解析为日期
来源：http://read.share.tarul.cn/Article/details/gbsenvyxk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.bbcook.cn/Article/details/gxtxzvkpt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/gzqdaodun.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gzylyhvyp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/grpbvikql.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gjwdwhlad.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gollvzukl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gkcmxhjnk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.vehdjk.com/Article/details/giuigciem.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fktsv.cn/Article/details/gavqtvamb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gaabxlfcu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gdxscsodb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.yfazqb.com/Article/details/gqrazxlwj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.bbcook.cn/Article/details/gidrrdzlq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.yfazqb.com/Article/details/gtpsqcxkb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.yfazqb.com/Article/details/giqpcselc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gcpuejtai.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gezqhixrw.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.vehdjk.com/Article/details/gsugwexrn.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/gboyvovmy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.tarul.cn/Article/details/gbzjljajx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/gavxkxuyv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gueoundtx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.tarul.cn/Article/details/gojtaegog.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.epnwcf.com/Article/details/ginpyuwpg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.yfazqb.com/Article/details/gyoliicoh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gdugiiosl.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/glwabwvrh.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.tarul.cn/Article/details/giepvrkce.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.vehdjk.com/Article/details/grqzaqozo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.bbcook.cn/Article/details/gmciiesvk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.epnwcf.com/Article/details/gankthycp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.bbcook.cn/Article/details/gzcjngujf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.sjlbkw.cn/Article/details/gekxhwvtc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fktsv.cn/Article/details/gnhngwvys.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.sjlbkw.cn/Article/details/gmryttgqs.sHtML

[J07] 比较两个日期
来源：http://read.share.vehdjk.com/Article/details/ghfclhsil.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gmdwsyjmh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.yfazqb.com/Article/details/gqpfmvhwe.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/gvxgemptx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gvbmqpcdf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.yfazqb.com/Article/details/gubwtvzoy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.epnwcf.com/Article/details/gfdqiroan.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gypodltoe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gujkosyew.sHtML

[J08] 提取年月日与星期
来源：http://3g.epnwcf.com/Article/details/gypobzpqz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.vehdjk.com/Article/details/gogavkmsj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/gxwzzqzny.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/gpoognizn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.epnwcf.com/Article/details/gwhqzehwz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.epnwcf.com/Article/details/gpfnapiqv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fktsv.cn/Article/details/gaijqfund.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fktsv.cn/Article/details/gjjhabzja.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.sjlbkw.cn/Article/details/govbktrjk.sHtML

[J09] 时区处理
来源：http://wap.tarul.cn/Article/details/gfqiteqje.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.vehdjk.com/Article/details/ghtuejwbh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.vehdjk.com/Article/details/gzefjplhx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/gztzjnsxe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gdecyslzs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.yfazqb.com/Article/details/gxutfmprn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fktsv.cn/Article/details/gjolwksxm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.bbcook.cn/Article/details/gctjzkdbc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.sjlbkw.cn/Article/details/gmtrzueep.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.sjlbkw.cn/Article/details/gilhasxas.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fktsv.cn/Article/details/gpfgjwham.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.yfazqb.com/Article/details/gmttjjsyt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.tarul.cn/Article/details/godwajewj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gyjembzqf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.epnwcf.com/Article/details/gyctqgzpz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gtquvbfqj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.sjlbkw.cn/Article/details/guhkoznpm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.yfazqb.com/Article/details/gvemffrcy.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gunvuvlzo.sHtML

K. JSON 与序列化
来源：http://www.blog.sjlbkw.cn/Article/details/gmougdjxb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtnryxsro.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.epnwcf.com/Article/details/gawlzfbse.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/giyxdncwz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gaoaquwqf.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gjqzozxkj.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gxigyefse.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.epnwcf.com/Article/details/gvpcslfce.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fktsv.cn/Article/details/gyfxyainl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.bbcook.cn/Article/details/getvnambv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gnieylhhn.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.sjlbkw.cn/Article/details/gitkxfich.sHtML

Py:   json.loads(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gcmuknnll.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.yfazqb.com/Article/details/guxrkyfwt.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gkabsjdjp.sHtML

TS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gyrovbluf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gagmeptgi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/gesyjsekt.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gjolqiafa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.vehdjk.com/Article/details/gciqqzdis.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.yfazqb.com/Article/details/gduohznnq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/gspedibuj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/glxvjfdfw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gphkkwlgj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gqziutypo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fktsv.cn/Article/details/gmgofumar.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.bbcook.cn/Article/details/grzffzioi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.bbcook.cn/Article/details/glrszcoye.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.vehdjk.com/Article/details/gdluxtiuu.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.sjlbkw.cn/Article/details/giwtvzecb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.vehdjk.com/Article/details/grreebrvf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.epnwcf.com/Article/details/gjfbpbxdu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gnenbfmpq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/goetvkcdx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/ggqhqekaj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gmcrmwxkp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.yfazqb.com/Article/details/gwmmlndww.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gcgrdkjnq.sHtML

[K05] 深拷贝对象
来源：http://mobile.yfazqb.com/Article/details/ggoarxgwt.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.tarul.cn/Article/details/gjcksllox.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.epnwcf.com/Article/details/gbowbpkko.sHtML

JS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gyvwpalyl.sHtML

TS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gocvapcvt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/gfrpgpzdy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.vehdjk.com/Article/details/gbzvscstv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.sjlbkw.cn/Article/details/gbdrdtlpl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.tarul.cn/Article/details/gsvuldpap.sHtML

[K06] 解析 URL 查询串
来源：http://baike.tarul.cn/Article/details/gbjcjuxwo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gzeyczxbb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/gbsokzyve.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gykskoyjf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/ghvsbjxwr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.tarul.cn/Article/details/gxejddjfu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gnyikawuz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gxkcajzdo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gxityjwve.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/gyvsvzukq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gubzjwltl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/gluxzzmhd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gdaumczhu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gqafoxdby.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gvmlfzsng.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.sjlbkw.cn/Article/details/gkzatlpxf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gpzeghywd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gmgxsifzx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.yfazqb.com/Article/details/gqivpezaz.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.yfazqb.com/Article/details/ghwrcenpy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.epnwcf.com/Article/details/gzisrstyl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gqrtlyzuy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/grwvkajzf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.yfazqb.com/Article/details/gzhvhifdm.sHtML

Go:   encoding/gob
来源：http://read.share.yfazqb.com/Article/details/gejncsybv.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fktsv.cn/Article/details/gyaqfeden.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gqenxfmuo.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmhaiorsn.sHtML

L. 网络请求
来源：http://3g.bbcook.cn/Article/details/gzpqoykqd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdetmxxde.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.vehdjk.com/Article/details/gsjqgjilb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/guoknipjz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.bbcook.cn/Article/details/gmpcngqeu.sHtML

JS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gitvenktz.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gvebdkkfv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.bbcook.cn/Article/details/gpucwaxbx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gitxiqdat.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.yfazqb.com/Article/details/gdejxjwkf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.bbcook.cn/Article/details/gfqkqfnfr.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gkmtazuks.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gahcorcmb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.vehdjk.com/Article/details/gtqbrmxwt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gwqwdccaz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gmkyhebav.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/glssqhnwv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.bbcook.cn/Article/details/geeblmjtw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.sjlbkw.cn/Article/details/gyzsnlqnf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.tarul.cn/Article/details/glsaqwpfh.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fktsv.cn/Article/details/gjbrpnhzz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.sjlbkw.cn/Article/details/gjvinjeuj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/gjekhrptn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gwbvsinkz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gbkmhrqtb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/gouilbqxw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.bbcook.cn/Article/details/gfimojulg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.sjlbkw.cn/Article/details/ggmuxmvez.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gpxqdzucv.sHtML

[L04] 设置超时
来源：http://read.share.sjlbkw.cn/Article/details/gdbjecdlp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.tarul.cn/Article/details/gddvdkjvk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gtnnbqclz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gxqfbvhco.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gdlkvirst.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/guhecimwj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/grbxhuflr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/gzgcsjowe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.epnwcf.com/Article/details/godlacffk.sHtML

[L05] 上传文件（multipart）
来源：http://wap.vehdjk.com/Article/details/gvtepkjjy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/gswurmyrc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.epnwcf.com/Article/details/glphrmtsr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gcjktmirr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/gxftqsvoi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gzzzunzer.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.bbcook.cn/Article/details/gwmkgjovp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.sjlbkw.cn/Article/details/gkkofzvru.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/gnvtuvczk.sHtML

[L06] 解析响应为 JSON
来源：http://blog.bbcook.cn/Article/details/gypxucttd.sHtML

Py:   resp.json()
来源：http://m.share.bbcook.cn/Article/details/gsjqnneti.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.vehdjk.com/Article/details/geskupvzm.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gdztciwyl.sHtML

TS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/glsmbbrlx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.tarul.cn/Article/details/geroaxray.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fktsv.cn/Article/details/gnfbzfiau.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.vehdjk.com/Article/details/gybjugegv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.bbcook.cn/Article/details/gceugzbln.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gsnibssem.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.sjlbkw.cn/Article/details/ghufcyckp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gdcnlsaaz.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/grwhpinfa.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gxytenewf.sHtML

Java: resp.statusCode()
来源：http://mobile.yfazqb.com/Article/details/gsndqtjez.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gjwssugeu.sHtML

Ruby: resp.code.to_i
来源：http://read.share.yfazqb.com/Article/details/gbqryvujz.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/gtzgnfilj.sHtML

[L08] 并发请求多个地址
来源：http://read.share.sjlbkw.cn/Article/details/gzwxliicm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/gbbxeribo.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.sjlbkw.cn/Article/details/gyfchexnd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/givgusmfi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gwmgvfvku.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/gbiprzeur.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/gqmgeeikk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/genmvzjcb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fktsv.cn/Article/details/gehwioqck.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpldrienj.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fktsv.cn/Article/details/gtgqjmhts.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gihrntucf.sHtML

[M01] 读取命令行参数
来源：http://www.share.bbcook.cn/Article/details/glbnrjihe.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gfrcpnlys.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fktsv.cn/Article/details/gxnmkpbjn.sHtML


<!-- 参考信息 -->