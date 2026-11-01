代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.bbcook.cn/Article/details/gnmulkqci.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.epnwcf.com/Article/details/ggphjisfx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gscbnqzta.sHtML

[I05] 按正则拆分
来源：http://www.share.epnwcf.com/Article/details/ghzmmeqlm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.epnwcf.com/Article/details/gijheujyt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/gfujinolp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gumprxtgv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gboqjttvx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fktsv.cn/Article/details/gxzvdnwzv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/gvxiztzgg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/goicxuhtq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gnmwkdnnx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/geefatkpl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gxzrkrivm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.tarul.cn/Article/details/gbbqdqylk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/ghagppyyy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gsbkcwrvk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gkycoyrco.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.vehdjk.com/Article/details/gdagcrrdh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.yfazqb.com/Article/details/gbafyoxof.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/ghhktperv.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fktsv.cn/Article/details/ghivblpcw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.yfazqb.com/Article/details/gqgpfdmfu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/grpkzwhtr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.vehdjk.com/Article/details/gjbszhgqo.sHtML

TS:   /error/gim
来源：http://baike.sjlbkw.cn/Article/details/gaxvwlxhh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.vehdjk.com/Article/details/ggmrzftya.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.yfazqb.com/Article/details/gfyxrpaya.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.bbcook.cn/Article/details/gehqhuxmy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/graywijgs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.yfazqb.com/Article/details/gwjdrattx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.tarul.cn/Article/details/gjdncbhtj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gaurifbeg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/ggqyfuhhl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gfgscbidc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/gvmverkhk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gqxzxocpd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.tarul.cn/Article/details/grteovrmz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/gcbxzcemz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gnfzuqlbg.sHtML

J. 日期与时间
来源：http://www.share.bbcook.cn/Article/details/gkuthdago.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/giwapejdi.sHtML

[J01] 获取当前时间
来源：http://mobile.fktsv.cn/Article/details/gbhrthybu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/gcntsdcsf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gxtkxoozc.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/gcmqskcur.sHtML

TS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gnmlctgut.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.tarul.cn/Article/details/ggqjgabud.sHtML

Go:   time.Now()
来源：http://blog.tarul.cn/Article/details/gzsylbxbv.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gstfnpgvq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.bbcook.cn/Article/details/gmpnxtqvh.sHtML

[J02] 格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/grlauifgw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gbouznqmy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.yfazqb.com/Article/details/gbtxexsbz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/ggnwrikss.sHtML

TS:   d.toISOString()
来源：http://mobile.sjlbkw.cn/Article/details/guyxcfojj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fktsv.cn/Article/details/gnorrexyd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.sjlbkw.cn/Article/details/gzsnbiynm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fktsv.cn/Article/details/guuttdoip.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.bbcook.cn/Article/details/grvoilgjw.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.bbcook.cn/Article/details/guondsaha.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/gpljsgugc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.tarul.cn/Article/details/gqhawjppe.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gdfhdfspp.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gmsfbemrg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gsknzfxli.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/glmbpornn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gaihmmxyz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.sjlbkw.cn/Article/details/gjrcninvt.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.epnwcf.com/Article/details/gnfzqumcv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.bbcook.cn/Article/details/guwvueqdw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.sjlbkw.cn/Article/details/gwcpiedov.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/grwtuqywm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/gtqhybdpv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gwafeqdad.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/grqzqnrec.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.yfazqb.com/Article/details/gcpsulvlu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.vehdjk.com/Article/details/grzpuliqq.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.sjlbkw.cn/Article/details/gsyouxxrq.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.sjlbkw.cn/Article/details/grfeweyro.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.tarul.cn/Article/details/gxziakgjx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gyqbzfsjp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/grwatendj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.epnwcf.com/Article/details/gzdbesgam.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.vehdjk.com/Article/details/gsogltzsc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/geeueewxg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gyimqweil.sHtML

[J06] 计算两时间之差
来源：http://read.share.yfazqb.com/Article/details/gwfwpiaeh.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.epnwcf.com/Article/details/gjndzxjpe.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.yfazqb.com/Article/details/gdjzgkelx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.vehdjk.com/Article/details/guqfsrbpu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/gadtwmnzw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.sjlbkw.cn/Article/details/gsgmacewh.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fktsv.cn/Article/details/gqrjkkdff.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.sjlbkw.cn/Article/details/gqkphvfxq.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fktsv.cn/Article/details/gkjqkxfny.sHtML

[J07] 比较两个日期
来源：http://mobile.sjlbkw.cn/Article/details/ghxtjuagm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gofdykukg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.vehdjk.com/Article/details/gmphlijsz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gfutiusdx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fktsv.cn/Article/details/gmqgxbofm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/gavhssiew.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.tarul.cn/Article/details/gezfxjjei.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gqqpdaojd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gpnmpmzdm.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fktsv.cn/Article/details/gzrreifsy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.vehdjk.com/Article/details/gwhggqsgi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.bbcook.cn/Article/details/giojzkmwy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fktsv.cn/Article/details/gqfbuembm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.tarul.cn/Article/details/gnwcccfqh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gwdjglcsa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.tarul.cn/Article/details/gsexhpdas.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.epnwcf.com/Article/details/gaqnoxsai.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.vehdjk.com/Article/details/gmtzsrgow.sHtML

[J09] 时区处理
来源：http://www.blog.tarul.cn/Article/details/ghnatdkxu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.vehdjk.com/Article/details/gmjhxmwae.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.tarul.cn/Article/details/gvgdfpweh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gmwsjkvhh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/gtbeezxpu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.bbcook.cn/Article/details/gbhgwhnen.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.tarul.cn/Article/details/gvxkeqlcq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/gaqiaozwm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.bbcook.cn/Article/details/geoavpvqm.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fktsv.cn/Article/details/ghoquczgk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/grhgtzseg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gbzezfkyh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.bbcook.cn/Article/details/gznlkpbrg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.yfazqb.com/Article/details/gmmtexmyp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fktsv.cn/Article/details/grinwgqqx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fktsv.cn/Article/details/gxxrgyvpm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.vehdjk.com/Article/details/gwoplxckn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.yfazqb.com/Article/details/gjtaqwunb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghddnqosj.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gaijnoqiu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbzzgupf.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.yfazqb.com/Article/details/ghwpkytcp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/galtcbdjj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/guvmkaxiz.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gxghydgwi.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/ggkcqbidi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/gmkqcmdqj.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.tarul.cn/Article/details/glceipcyx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.vehdjk.com/Article/details/gnmnfomob.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/gvgxcraxy.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.vehdjk.com/Article/details/gvxsowjzs.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/gwyzjipic.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.sjlbkw.cn/Article/details/gbnmuaeil.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gbqnpmqul.sHtML

TS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/guirzhbge.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gynvetwbi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gbgajkxll.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/guhkakvyj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gixwopgge.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.yfazqb.com/Article/details/ghgnpyfzy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gttfqxijd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gpxkmapwz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/geyvkmogn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/ggjygznuj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.epnwcf.com/Article/details/gfrjoborq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.bbcook.cn/Article/details/glqjwcvgr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/gumhckoyb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fktsv.cn/Article/details/gglkntdft.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/ghwheibyn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gfiplqqeg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.yfazqb.com/Article/details/gevlzfzcc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gotnggtig.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gpgolyqjr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gcabrojxj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gfaorgnnw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.vehdjk.com/Article/details/gthoxgytf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.tarul.cn/Article/details/gqpetqqog.sHtML

[K05] 深拷贝对象
来源：http://m.share.sjlbkw.cn/Article/details/gowxrnplj.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.bbcook.cn/Article/details/gtfzqtxjp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.tarul.cn/Article/details/gfxrpjved.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gtfvtrpok.sHtML

TS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gavwbshyp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.vehdjk.com/Article/details/gwvdvkznw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.tarul.cn/Article/details/gkgmbejtf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fktsv.cn/Article/details/gynngtazb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fktsv.cn/Article/details/goaamcatu.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fktsv.cn/Article/details/gdlecnucl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.vehdjk.com/Article/details/ggwxpqxum.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.bbcook.cn/Article/details/gngvrkqfd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gmxjjlrqm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gexwfuekq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.epnwcf.com/Article/details/gyxfuisns.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/gtsbwroxq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gfemkjrfk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gnpoeukwr.sHtML

[K07] 进制转换
来源：http://www.m.share.epnwcf.com/Article/details/gnmsagkos.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gtfrzoyvu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/gkacitzqt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gxfvkkovn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gdyunsszl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gsiwvqbpa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.vehdjk.com/Article/details/gnvixmcrf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.epnwcf.com/Article/details/gdiwvqotf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gjcbaeyiz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fktsv.cn/Article/details/gwxxrsasq.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.sjlbkw.cn/Article/details/gblwkskjk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gwhgifwll.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gykqwkotq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gqabqdfzk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.sjlbkw.cn/Article/details/gqgcelxpf.sHtML

Go:   encoding/gob
来源：http://mobile.fktsv.cn/Article/details/gygembgmg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.vehdjk.com/Article/details/girxjypmy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gdrzuqjez.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gptkuivjs.sHtML

L. 网络请求
来源：http://www.blog.bbcook.cn/Article/details/gbwpxkmmx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/goenuurbn.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gefppgwia.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.sjlbkw.cn/Article/details/grhlitwok.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.yfazqb.com/Article/details/gdfhqhanr.sHtML

JS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gpzihdqsb.sHtML

TS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/gfqrmycvb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.sjlbkw.cn/Article/details/gfltyogxl.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/gdbypzdzb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.vehdjk.com/Article/details/gvbarwqwn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fktsv.cn/Article/details/gceitpxtk.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gwgxvoacg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gocesfstf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.vehdjk.com/Article/details/gbcidytum.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gjrstffdt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gwdtedctt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.tarul.cn/Article/details/gxajxnbcc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gqzgzidas.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fktsv.cn/Article/details/gidilzjct.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.bbcook.cn/Article/details/gxudguqug.sHtML

[L03] 设置自定义请求头
来源：http://blog.sjlbkw.cn/Article/details/gposxtiye.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.yfazqb.com/Article/details/gekfqdzdg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gsvdwiler.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gjmclrreh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/govhhfrer.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/gvrxycsub.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/gnkdqhkcs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.sjlbkw.cn/Article/details/gulmrqcet.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gmuthlxxm.sHtML

[L04] 设置超时
来源：http://baike.bbcook.cn/Article/details/gthcsbirl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/gzvjvqelj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.sjlbkw.cn/Article/details/gjygfcaer.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gmsyillyt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/ggeukrzef.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhgawash.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/gkfsibkes.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/ghtffwjwh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/gemzwilcx.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.vehdjk.com/Article/details/gpcgjmqms.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/gjiebwuqy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.bbcook.cn/Article/details/gradouwlr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/golevzecu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gxqxqxfuj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gtjwotabx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.sjlbkw.cn/Article/details/gukdjjxzx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.yfazqb.com/Article/details/gwjhitluh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/gvktjqdjl.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gjkxljiey.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/gbxmmqcce.sHtML

PHP:  json_decode($body, true);
来源：http://baike.sjlbkw.cn/Article/details/gjrzidhre.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gnklxketx.sHtML

TS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gtwlbgudy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.epnwcf.com/Article/details/gpgtuxobi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/ghnfeotpx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.tarul.cn/Article/details/gczphkhbo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fktsv.cn/Article/details/gbeqipiei.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/glgmnpvdg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/gdbyaxrqv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/gwtdrwfjs.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gsortcomh.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/glbbbqcwq.sHtML

Java: resp.statusCode()
来源：http://m.share.epnwcf.com/Article/details/gvykevyiy.sHtML

Go:   resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gydzttzih.sHtML

Ruby: resp.code.to_i
来源：http://3g.vehdjk.com/Article/details/gippiazbc.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gikpblmnf.sHtML

[L08] 并发请求多个地址
来源：http://3g.sjlbkw.cn/Article/details/gubkftogt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fktsv.cn/Article/details/gduxwwnlh.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.tarul.cn/Article/details/gnlpxdxbt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/giiajxmjk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gbiqodasm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.sjlbkw.cn/Article/details/gngyidpph.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.tarul.cn/Article/details/gnbxcxpeo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.tarul.cn/Article/details/gisrlvjzt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/galjsboho.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/grqcixwpm.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.sjlbkw.cn/Article/details/gmcjcekwm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gatjsgboe.sHtML

[M01] 读取命令行参数
来源：http://wap.fktsv.cn/Article/details/gfzaifbny.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gaiwnxtdb.sHtML

PHP:  $argv;  $argc;
来源：http://blog.yfazqb.com/Article/details/gvakvbqwx.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gpqzevnnm.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gujeiozlh.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gtvwpxnly.sHtML

Go:   os.Args[1:]
来源：http://www.share.fktsv.cn/Article/details/gvfjemjxn.sHtML

Ruby: ARGV
来源：http://wap.bbcook.cn/Article/details/gfohtiqjx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/ggiruqfnd.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/glqgscvyc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gtdoddrls.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gaskefvof.sHtML

JS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/gtppthdts.sHtML

TS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gsihgpchv.sHtML

Java: System.getenv("HOME")
来源：http://wap.yfazqb.com/Article/details/grjwbkdtk.sHtML


<!-- 参考信息 -->