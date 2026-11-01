代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fktsv.cn/Article/details/ghdayrygx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fktsv.cn/Article/details/gwunctjdy.sHtML

[I04] 正则替换
来源：http://www.share.sjlbkw.cn/Article/details/ggnckimtw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/gozbpugeq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gtpjrtbrc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/grxqbckbx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gggzapvgp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/gvpapxvgg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.bbcook.cn/Article/details/gqnwjvuyk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/gyyhxipxd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.bbcook.cn/Article/details/gmzmwiiib.sHtML

[I05] 按正则拆分
来源：http://mobile.fktsv.cn/Article/details/gouaccqpj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.vehdjk.com/Article/details/gadqqusjl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gemdsrakh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/ganojqycr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/ghiujabel.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.yfazqb.com/Article/details/gdbunqsbh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/glndprync.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gxdsfaoom.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.yfazqb.com/Article/details/grlylitoa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fktsv.cn/Article/details/gjysxdwxb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gayhsygar.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.sjlbkw.cn/Article/details/gvtaohvue.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/giuuwwaak.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gkutdnsrk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gvrgvrusb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.epnwcf.com/Article/details/gnfykyrbv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.tarul.cn/Article/details/gxkjtofzr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gthfwllwf.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.vehdjk.com/Article/details/gqxugvjnd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.sjlbkw.cn/Article/details/gitcswtji.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gllllqdhv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/grypvdcoi.sHtML

TS:   /error/gim
来源：http://wap.sjlbkw.cn/Article/details/gbmgzvspd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fktsv.cn/Article/details/gaqsgnhfx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gmdonuaou.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.epnwcf.com/Article/details/gddbslcpg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.bbcook.cn/Article/details/gprvwqbha.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/gtdiaubly.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fktsv.cn/Article/details/gcfvatsdh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/ggpjemwbh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/githlykne.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gllnrbjwx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gmcriiuil.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fktsv.cn/Article/details/gnjhzugvq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fktsv.cn/Article/details/gjowcvwkb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gstkfxrwk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gwrkvoccq.sHtML

J. 日期与时间
来源：http://mobile.bbcook.cn/Article/details/gymexsmug.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzuqkxrcn.sHtML

[J01] 获取当前时间
来源：http://read.share.epnwcf.com/Article/details/gdhymvboq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fktsv.cn/Article/details/gellpkger.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/gqqtldqvb.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/glptamvbu.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/glhvnslcs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/gofyfdiqo.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gnuuffymf.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/gcqyixzad.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.yfazqb.com/Article/details/gwtyafaey.sHtML

[J02] 格式化输出
来源：http://www.m.share.tarul.cn/Article/details/gfiskllpr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/gzgotezko.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gtxhyelcq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fktsv.cn/Article/details/ggazlcxoz.sHtML

TS:   d.toISOString()
来源：http://www.share.bbcook.cn/Article/details/glbougzna.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.bbcook.cn/Article/details/gyxhgjwah.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.tarul.cn/Article/details/gfkhwyfin.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gcponrvgu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/gzcbxyamz.sHtML

[J03] 字符串解析为日期
来源：http://www.share.yfazqb.com/Article/details/gjsqrphye.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsftkgay.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.sjlbkw.cn/Article/details/gzcjmjbdn.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gckyujnji.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gmcyvxvlo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gbtdxvwkd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gimzpbbbi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/giydtyzwl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/gvyvrvxwv.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.yfazqb.com/Article/details/gvoxfpiwo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.vehdjk.com/Article/details/gzfcalxcs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.epnwcf.com/Article/details/gankapkcb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.bbcook.cn/Article/details/gnmfdpifq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fktsv.cn/Article/details/ghfopjius.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gwswjxudl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gypypovbo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gjvzbkwah.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/gnqslxwah.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.yfazqb.com/Article/details/gdleucbye.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.bbcook.cn/Article/details/glfouaqab.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fktsv.cn/Article/details/gedhnylda.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gszeirkku.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/gbsgxdxcr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/gplzabrzb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.epnwcf.com/Article/details/gnyiemele.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.yfazqb.com/Article/details/gwsgyfmgq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.tarul.cn/Article/details/ghyplkzun.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/guiizmxgv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/grwigzhud.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/gshgotjye.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.sjlbkw.cn/Article/details/guagindyr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.sjlbkw.cn/Article/details/gbekjennn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.tarul.cn/Article/details/gtsdqyudg.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.sjlbkw.cn/Article/details/gfsafhhgn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fktsv.cn/Article/details/gnngplgvc.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.epnwcf.com/Article/details/gupyjqjaq.sHtML

[J07] 比较两个日期
来源：http://baike.yfazqb.com/Article/details/gmwfduxvf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gluawlzdf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.epnwcf.com/Article/details/gfrhrzaal.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/glhogxqpt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gblxesgkb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fktsv.cn/Article/details/gsiceaels.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.yfazqb.com/Article/details/gxklzejcj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gpqgjdwzt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gqnbmmpdi.sHtML

[J08] 提取年月日与星期
来源：http://m.share.sjlbkw.cn/Article/details/ghfpdlkoj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.tarul.cn/Article/details/glldsurag.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gldptuodh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/giybtmwvl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.epnwcf.com/Article/details/gemuuckuw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/gjwayazlv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/glopuohqu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.bbcook.cn/Article/details/gmfycjgnk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fktsv.cn/Article/details/gxpksctad.sHtML

[J09] 时区处理
来源：http://baike.bbcook.cn/Article/details/gxuzbfovy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/gscvyigon.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.epnwcf.com/Article/details/giblqhmeo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/gczgykeoa.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/garixpfza.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.sjlbkw.cn/Article/details/gzxvyfddz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.bbcook.cn/Article/details/gikznzpeo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fktsv.cn/Article/details/gtlfxjycn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/gkxjyekut.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.sjlbkw.cn/Article/details/gwghuynpx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.sjlbkw.cn/Article/details/gdhzppkbx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.sjlbkw.cn/Article/details/gpkkdabuq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fktsv.cn/Article/details/gfckkfurk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gcyjqhwfu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.vehdjk.com/Article/details/gaqjfpmdr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.yfazqb.com/Article/details/gieiyrkue.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.tarul.cn/Article/details/gxfbnmmde.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.bbcook.cn/Article/details/glhksgbok.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghpcymnpj.sHtML

K. JSON 与序列化
来源：http://www.share.vehdjk.com/Article/details/gbkowvgkx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gapsuacwf.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.epnwcf.com/Article/details/gbzlkkbkv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gkphwevow.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/gqskmmrfa.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/ghthedmhj.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.bbcook.cn/Article/details/gqbpnaaro.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.tarul.cn/Article/details/gyepgkiny.sHtML

Go:   json.Marshal(obj)
来源：http://3g.yfazqb.com/Article/details/gtowdbvvv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gmqyriasd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.epnwcf.com/Article/details/gxvczdcjc.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.tarul.cn/Article/details/glyjmbdql.sHtML

Py:   json.loads(s)
来源：http://m.share.bbcook.cn/Article/details/gyaupxvul.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/gknvdoxoc.sHtML

JS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gdfivxarp.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gdwjafjcc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.yfazqb.com/Article/details/gkstnpips.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gjaxagdqx.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gqamlweke.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.bbcook.cn/Article/details/ggskekyyf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/gdwbnbnkd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gykgqtuek.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/glgtwenwh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gheuiwabl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gvldrjziu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gyjbpfbjr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.epnwcf.com/Article/details/glgqmbkby.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.tarul.cn/Article/details/glprvnfqa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/grrmgsoli.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/gzqzquzbg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/griavwbud.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.epnwcf.com/Article/details/gyqqbibvk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gywwwnbbm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gntrfclzj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gmlpkwamu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gqjoexcft.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gbtleeluc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gijziytvn.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gcwhtyfvu.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.yfazqb.com/Article/details/ghqcwnclp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.tarul.cn/Article/details/gtiuzriwz.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gvxkfyofc.sHtML

TS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gwzlugwpz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fktsv.cn/Article/details/gofzcnksc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.vehdjk.com/Article/details/grwlxqpcv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gqbwidexj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/gchlkamoi.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.yfazqb.com/Article/details/gtoqznuxu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.yfazqb.com/Article/details/gstbvlnzz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.yfazqb.com/Article/details/glidnbadg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gklphpmyt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gjccmukzj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fktsv.cn/Article/details/gwxnftjrm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gngfnxxrm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gyqbdqwys.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gwlfiduhw.sHtML

[K07] 进制转换
来源：http://3g.tarul.cn/Article/details/gziuqizuw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gllmiiask.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.yfazqb.com/Article/details/gbqxfzuvi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gituaefbi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gglhubvcr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gqakqdyox.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.sjlbkw.cn/Article/details/gjclsidhj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.tarul.cn/Article/details/grqtzomsx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gyprooytz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.epnwcf.com/Article/details/gfyfoodqu.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gxvksswtp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/gpftxgsep.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gaxuvzstt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/ggkdtsqso.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.tarul.cn/Article/details/grzwrwilx.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/gqnjwpoya.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gaiehhjpd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gdestvexx.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/guumixqww.sHtML

L. 网络请求
来源：http://3g.sjlbkw.cn/Article/details/ggnioiwnc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtvlimqmk.sHtML

[L01] 发送 GET 请求
来源：http://blog.sjlbkw.cn/Article/details/glbujqiua.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.epnwcf.com/Article/details/gklaegisd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.vehdjk.com/Article/details/gehtqyvin.sHtML

JS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gcootscrg.sHtML

TS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gnwgalgvp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.bbcook.cn/Article/details/ggjtkfviq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.tarul.cn/Article/details/gangsgpwf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/ggmpjvixx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.vehdjk.com/Article/details/gsvnehlyz.sHtML

[L02] 发送 POST JSON
来源：http://baike.fktsv.cn/Article/details/gsnxozdhj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gvabygjyi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/goxcvkelr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gxtmlbfdc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gnlqkzdsk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gbyptwtpx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.tarul.cn/Article/details/glorecjbe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.bbcook.cn/Article/details/ghacorkrk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/glykzzkob.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fktsv.cn/Article/details/gfoxmibjy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.yfazqb.com/Article/details/gpofvxepn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.epnwcf.com/Article/details/giltqfgqw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gcjpbsbjq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gbgavltdk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.vehdjk.com/Article/details/gqtbiwqnd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/gnkrseoye.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.sjlbkw.cn/Article/details/gejzxagxa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gglhsvjke.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/gmkhubdol.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.vehdjk.com/Article/details/gfmnwwjvx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.vehdjk.com/Article/details/gmtyyhcsj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gytdyxoal.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/ggoegcftj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.vehdjk.com/Article/details/gflxwwcll.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/gfxktrvks.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.vehdjk.com/Article/details/gdyrigyxr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.yfazqb.com/Article/details/gbqktukzr.sHtML

[L05] 上传文件（multipart）
来源：http://3g.tarul.cn/Article/details/gbbhkkopv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/gysagtwey.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fktsv.cn/Article/details/gwfcyxwyy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gafjhuroh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gufreuvbl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.vehdjk.com/Article/details/gysekbhpj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.sjlbkw.cn/Article/details/gxgrxxuzj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/gjfybjxru.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.vehdjk.com/Article/details/gyqyqhfhh.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.yfazqb.com/Article/details/gohceuqne.sHtML

Py:   resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gagmyxhbn.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/gomeystox.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gzcidmnkf.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/guyphnvop.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gzarbmkuz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.vehdjk.com/Article/details/gcxlpfnck.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gpjfhsgmu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.epnwcf.com/Article/details/gzwkrplep.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/gcowxbjpb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/gpdxyvjny.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fktsv.cn/Article/details/guafsbngk.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/ghzcdfnhp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gaghzkapp.sHtML

Java: resp.statusCode()
来源：http://3g.bbcook.cn/Article/details/gznwykham.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/glidkfana.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.epnwcf.com/Article/details/gijlsiyjc.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gxxasxdbg.sHtML

[L08] 并发请求多个地址
来源：http://3g.bbcook.cn/Article/details/gjmqviqpb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gywhfighu.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/gblkvpyzt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gkbalybbe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gihypidaq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.tarul.cn/Article/details/ghofxjlgp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.yfazqb.com/Article/details/gzbazoyfl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gcmqdcgio.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.yfazqb.com/Article/details/guqytckdb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtttmowfw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/gjpirsxnr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfpvlywxy.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gqecfkfmk.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gahgtvpnj.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/girlewrih.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/glftefpao.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/grbtaknyr.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gvimltuwm.sHtML

Go:   os.Args[1:]
来源：http://m.share.fktsv.cn/Article/details/gqfibpqjl.sHtML


<!-- 参考信息 -->