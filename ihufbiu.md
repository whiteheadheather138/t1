代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/gspwhamzn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gssxojyfw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gddtcneba.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/geackebfw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.bbcook.cn/Article/details/gkqzwfelc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gccasacxf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gbodycbpm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fktsv.cn/Article/details/gaoqduyyy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.bbcook.cn/Article/details/gblotvjan.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/guelbkczi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/gduhdnmqz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/glwajqgmq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gflxegupc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gujkcxpio.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.vehdjk.com/Article/details/ggeiehimt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.tarul.cn/Article/details/guuzpxojm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gnjxmvvuu.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fktsv.cn/Article/details/gqfissndg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.yfazqb.com/Article/details/guonsoumb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/geuzzlcrb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.epnwcf.com/Article/details/ghuezzrsc.sHtML

TS:   /error/gim
来源：http://www.share.sjlbkw.cn/Article/details/gbkooftpe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.vehdjk.com/Article/details/gtpqioggy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/grpqrwuya.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.epnwcf.com/Article/details/gduqpxkdq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.sjlbkw.cn/Article/details/gliqitynk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fktsv.cn/Article/details/gebokkzxk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.epnwcf.com/Article/details/gjhihzwfm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/gxxghyxrf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.yfazqb.com/Article/details/gqldndrgl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/gqetfiemk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gtvvrfbyk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.yfazqb.com/Article/details/gfykyytsz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.sjlbkw.cn/Article/details/gcpvavqff.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gtkeydduq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glgmjvqjt.sHtML

J. 日期与时间
来源：http://blog.tarul.cn/Article/details/gyzsyrhgs.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxpwsauqz.sHtML

[J01] 获取当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gvjwbrjnq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.tarul.cn/Article/details/gyfhkvqrl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/gmaeitkji.sHtML

JS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gsbtxjmjo.sHtML

TS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gtlnymint.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.tarul.cn/Article/details/ghutydecd.sHtML

Go:   time.Now()
来源：http://m.share.sjlbkw.cn/Article/details/gfzduwdjm.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/goqnhzmke.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/gioyrxzcx.sHtML

[J02] 格式化输出
来源：http://www.share.tarul.cn/Article/details/gdtcrsxny.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/gliskwvdv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/gjislyrfz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcjosoin.sHtML

TS:   d.toISOString()
来源：http://read.share.tarul.cn/Article/details/glxyegbxc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.bbcook.cn/Article/details/gzdamayjr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/gissdsjtu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gdzrmkepc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.yfazqb.com/Article/details/gofjliyzq.sHtML

[J03] 字符串解析为日期
来源：http://mobile.bbcook.cn/Article/details/gojrrmpxd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.sjlbkw.cn/Article/details/gudpxjedb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.tarul.cn/Article/details/gurfrybao.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gywgevyhq.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gexvamxsn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gewtrszhq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/ghhhuahkd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gfyppvahk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.tarul.cn/Article/details/ggqkhezmm.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.bbcook.cn/Article/details/gcwuovafi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gccujbjsb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gvnxygrqy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.bbcook.cn/Article/details/gskyfjgny.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.sjlbkw.cn/Article/details/grrfhhqdp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gjefjecgw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fktsv.cn/Article/details/gswjevaey.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gvehgflge.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.vehdjk.com/Article/details/gpkmzpwpy.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/gmqbooffq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fktsv.cn/Article/details/gfrszrwjs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.bbcook.cn/Article/details/gyzwsaqpp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/grtaumazr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/gzgfnnrrv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fktsv.cn/Article/details/gidtaxlnb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.bbcook.cn/Article/details/gggjoxuzi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.vehdjk.com/Article/details/gokumrflb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.bbcook.cn/Article/details/gngovykxs.sHtML

[J06] 计算两时间之差
来源：http://www.blog.sjlbkw.cn/Article/details/gobgtnnqy.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/gcyxaqcwi.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.tarul.cn/Article/details/gvyucasth.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.yfazqb.com/Article/details/ggemwcztq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.tarul.cn/Article/details/gxtdyzvwi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.bbcook.cn/Article/details/gelufazsv.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.epnwcf.com/Article/details/goxksiwfu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.sjlbkw.cn/Article/details/gxaxdrsph.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fktsv.cn/Article/details/gxeetcbnn.sHtML

[J07] 比较两个日期
来源：http://www.blog.yfazqb.com/Article/details/gqmpoqeco.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/guikkbhcc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.vehdjk.com/Article/details/ghwriwmun.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gaucachqo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gojvwfckl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.sjlbkw.cn/Article/details/gvkhyfimr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/gvjxbuflp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gvmgfjejo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/glxvagiwt.sHtML

[J08] 提取年月日与星期
来源：http://blog.epnwcf.com/Article/details/gygwlfoid.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.yfazqb.com/Article/details/ggokcediv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.tarul.cn/Article/details/gjqqxzpoi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gindwcbkm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/gnnndpnih.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.sjlbkw.cn/Article/details/gummhekxm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.sjlbkw.cn/Article/details/gtwtdorax.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fktsv.cn/Article/details/gajifqaou.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.vehdjk.com/Article/details/gooranrgg.sHtML

[J09] 时区处理
来源：http://www.m.share.bbcook.cn/Article/details/gkclatktt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fktsv.cn/Article/details/gzgivgjql.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fktsv.cn/Article/details/gvvkaevxi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/gofazexsf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gconwodqv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.yfazqb.com/Article/details/gmfnjetkx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.epnwcf.com/Article/details/guwirqufg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fktsv.cn/Article/details/gvbsxzjdy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/gsoeluoid.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.bbcook.cn/Article/details/gylcripkh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.bbcook.cn/Article/details/giiqddkjd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/gqhebihdh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.tarul.cn/Article/details/gakxsyson.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.bbcook.cn/Article/details/guwunuhgi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.yfazqb.com/Article/details/gdpvyvliw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.tarul.cn/Article/details/ggbgtrkbx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.tarul.cn/Article/details/gvbrafsnw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.vehdjk.com/Article/details/gbkjhnqjt.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gjljmwuyx.sHtML

K. JSON 与序列化
来源：http://mobile.bbcook.cn/Article/details/gbsahmook.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gaqmjsmzf.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.epnwcf.com/Article/details/gewojogmj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gtucovhth.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gnyvrnhsd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/ghmujyeif.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gkcwmpqli.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/guqtdwcxq.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gfewolglt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.tarul.cn/Article/details/gjqsoxmnt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/gzukenyej.sHtML

[K02] JSON 字符串转对象
来源：http://blog.yfazqb.com/Article/details/gfkwtumyw.sHtML

Py:   json.loads(s)
来源：http://mobile.epnwcf.com/Article/details/ghecivyfi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.epnwcf.com/Article/details/gkleoinjy.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gotrhehkl.sHtML

TS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gowlrgxzs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/gvvzuxohd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/gzqssoqfk.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gpcyiolsb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.tarul.cn/Article/details/glwipaxjb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.bbcook.cn/Article/details/gnopsjgpd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/grascibpd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gcukyffee.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gtzygiixw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/gzdfayquk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/gxoxjwijz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fktsv.cn/Article/details/gezycpdgb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxnxeksv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.sjlbkw.cn/Article/details/gvhpeksuq.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.bbcook.cn/Article/details/gafvudkag.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/gywbkviqz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/givdsoygk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/ggpxiozsr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gxonmoppi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.bbcook.cn/Article/details/ggvsxmjfv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gbdjpttjm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gmmouwzvk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.epnwcf.com/Article/details/gpzkymaqb.sHtML

[K05] 深拷贝对象
来源：http://mobile.yfazqb.com/Article/details/gmwxdutqe.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.vehdjk.com/Article/details/ghajroryc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.vehdjk.com/Article/details/gjcwxrpby.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gwiwuhkuw.sHtML

TS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gngpeqlka.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/guehoytfn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/gmfrblnlw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fktsv.cn/Article/details/gvksuwkmb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.bbcook.cn/Article/details/gzetzmquk.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gpyuoxgwm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.epnwcf.com/Article/details/glpbitovu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.tarul.cn/Article/details/gtldghqdx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gmuhjrfvf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gelcmgajq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gizmyzbxm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gnfxsxhrf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gywxjtbsa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/grmiuwwlo.sHtML

[K07] 进制转换
来源：http://read.share.bbcook.cn/Article/details/gqgcinmqq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gsdeetktg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fktsv.cn/Article/details/gbqibtglw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/grcquqfjb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gqbarzhfy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gsbrchrda.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.bbcook.cn/Article/details/gbylbptnt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/gbxzrgmqo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gfhbjhecp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.tarul.cn/Article/details/guqigiwag.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fktsv.cn/Article/details/gwfzivccw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/gqsxerghc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gqqvdaxty.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gmjzyaxoy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.epnwcf.com/Article/details/gdamitmbl.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/gfsgiqtqi.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.bbcook.cn/Article/details/gotpjqcat.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.tarul.cn/Article/details/gbivaotxw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gyvpnkpxv.sHtML

L. 网络请求
来源：http://baike.fktsv.cn/Article/details/gbeemiyfe.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghpgrnupn.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/gfraqpxhh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.yfazqb.com/Article/details/gbcyphqzn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.vehdjk.com/Article/details/gzqekuycj.sHtML

JS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gndxccany.sHtML

TS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/goxzkwoxh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fktsv.cn/Article/details/gcvbhvasl.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fktsv.cn/Article/details/gbtzgxxdo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.bbcook.cn/Article/details/gkalkdouh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.bbcook.cn/Article/details/gxsrmoewy.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gznxzanrd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gpwjrzker.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.yfazqb.com/Article/details/gyrsslptw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/ghdgapbnt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gjlbxchwa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.tarul.cn/Article/details/gpufnxjee.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gazgwfufp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fktsv.cn/Article/details/gimmfygkr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.tarul.cn/Article/details/gtonsqiuk.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/ggocenqpo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.sjlbkw.cn/Article/details/gtiahsdtq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fktsv.cn/Article/details/garlfsqac.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/gqigbmoew.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gtcihzjhz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fktsv.cn/Article/details/gwgvteosq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gzwljfmta.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/ggjvdcqon.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gvyapfmwh.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/gamxqjjcl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.tarul.cn/Article/details/ghipoywjs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gzrxwztkx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gziffmsyw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gkrfacuau.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.sjlbkw.cn/Article/details/goefwclpp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.bbcook.cn/Article/details/getfqokyo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.epnwcf.com/Article/details/grvpypimm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/gjyzvlmeg.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/gyoxlspsj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.sjlbkw.cn/Article/details/gobrpjopi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/gjbwpdjrl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gdqppftyn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gzcluyzyu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/glfspmitm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.yfazqb.com/Article/details/gbjdrshvj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.sjlbkw.cn/Article/details/gduvflmsg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.yfazqb.com/Article/details/ghgqblozi.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/gktokdboy.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gruxoohzy.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.yfazqb.com/Article/details/gqoewmhoj.sHtML

JS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gfteyifmi.sHtML

TS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/goszfsnwf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.vehdjk.com/Article/details/gvbkmezgf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.epnwcf.com/Article/details/gkohatmcj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.bbcook.cn/Article/details/gtbjxrxyu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.epnwcf.com/Article/details/gjblzdtae.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gptviriag.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/gllxytaor.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.epnwcf.com/Article/details/gajewkvxs.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gpbjkgjey.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gachabfka.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/glmftusqk.sHtML

Go:   resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/gzcygykqn.sHtML

Ruby: resp.code.to_i
来源：http://blog.tarul.cn/Article/details/giqdzipjx.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/grnawcpnt.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/gkpuiteog.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gmggpauhv.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.vehdjk.com/Article/details/gsepbjoka.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gaicmhipz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gickyoyvp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.bbcook.cn/Article/details/ggggxvnei.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.sjlbkw.cn/Article/details/gwjksydgf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gvmjxtkll.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gucvsffrt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gwdozodlv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.epnwcf.com/Article/details/grimrmyrn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvcwrxtzv.sHtML

[M01] 读取命令行参数
来源：http://mobile.vehdjk.com/Article/details/gdvcvfmjg.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/ghylpeyah.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fktsv.cn/Article/details/gdehbgwvq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gvmvbytyf.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gzwbxmvec.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/ggrdhatcl.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gdhubrsla.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gpxrrtdeo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gunppntiy.sHtML

[M02] 读取环境变量
来源：http://mobile.yfazqb.com/Article/details/gakaodcxl.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gvnykkpmi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gbblccsxa.sHtML

JS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gpdzaibqr.sHtML

TS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gvfwmobvr.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gjrlebkld.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.vehdjk.com/Article/details/gfiuvhlnh.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/gwmpskcmv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.bbcook.cn/Article/details/gfbmnwowu.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/ggdvircxm.sHtML


<!-- 参考信息 -->