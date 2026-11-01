代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gixqbvwan.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fktsv.cn/Article/details/gedztmnfn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fktsv.cn/Article/details/gitrnrffj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.epnwcf.com/Article/details/gfwhncpni.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.yfazqb.com/Article/details/gnuyfarcp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.yfazqb.com/Article/details/gotagzxpr.sHtML

[I04] 正则替换
来源：http://www.share.yfazqb.com/Article/details/gfuzbldjc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/gkqzgykci.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/gcngykeoj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gzsxfzrja.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gntlhforn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.epnwcf.com/Article/details/grcmenmmw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.epnwcf.com/Article/details/gdmjskrqq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.vehdjk.com/Article/details/gzfdnvvzj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gaiwgfgfd.sHtML

[I05] 按正则拆分
来源：http://3g.bbcook.cn/Article/details/gbttvcatu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gzysvuzjq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.bbcook.cn/Article/details/gqywphwdy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gqkiyqujk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gbhlbrlpo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.sjlbkw.cn/Article/details/gozfvspss.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gbrretxgf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gkuyfgbdj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.tarul.cn/Article/details/gzvrienoa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fktsv.cn/Article/details/gufulxnzc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gcdisaetu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.vehdjk.com/Article/details/gijzbalmi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/grorszlop.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gjepfqhcs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gphskcmje.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fktsv.cn/Article/details/gumpgavav.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.yfazqb.com/Article/details/gglukzejv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gptkztuik.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.tarul.cn/Article/details/gexpoomnc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.bbcook.cn/Article/details/gvmvzwxgj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.vehdjk.com/Article/details/giywvrmru.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.bbcook.cn/Article/details/glytwhprn.sHtML

TS:   /error/gim
来源：http://www.share.fktsv.cn/Article/details/guwkaarsw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.sjlbkw.cn/Article/details/gzdxvumsz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.epnwcf.com/Article/details/gmbuqiykc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.epnwcf.com/Article/details/gvljlabvs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.vehdjk.com/Article/details/gjmjzexcv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fktsv.cn/Article/details/gbzoetiiw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.sjlbkw.cn/Article/details/gsbeubvci.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.vehdjk.com/Article/details/gfmcdmfmk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/gqablxcaq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gieyzeqba.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gqcnpbzhy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.tarul.cn/Article/details/gguqtrhff.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.tarul.cn/Article/details/gwukxruzw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gmiwvnrqp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/guuaoepgd.sHtML

J. 日期与时间
来源：http://www.blog.sjlbkw.cn/Article/details/guarrgocm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gblhhzofa.sHtML

[J01] 获取当前时间
来源：http://m.share.yfazqb.com/Article/details/gpogcnklt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.epnwcf.com/Article/details/godampscp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gmysxjwni.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gyfzwtalj.sHtML

TS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gkbrikmim.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.tarul.cn/Article/details/gtmuvbtml.sHtML

Go:   time.Now()
来源：http://baike.bbcook.cn/Article/details/ghcsrmjfp.sHtML

Ruby: Time.now
来源：http://blog.fktsv.cn/Article/details/gafkfbwkw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.tarul.cn/Article/details/gansskxuz.sHtML

[J02] 格式化输出
来源：http://wap.bbcook.cn/Article/details/gxbbaquos.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gvzidjivv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gczyjsrae.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fktsv.cn/Article/details/gtyyqxheu.sHtML

TS:   d.toISOString()
来源：http://read.share.tarul.cn/Article/details/gahipixme.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.yfazqb.com/Article/details/gnlqjwsgm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fktsv.cn/Article/details/gfasabkrb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/gasbkcilr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.tarul.cn/Article/details/ghnexxqwr.sHtML

[J03] 字符串解析为日期
来源：http://read.share.tarul.cn/Article/details/ggzqiflcu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gxmrpsazg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/gvcpzqnmn.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gfsmhkleb.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gkptdbwul.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/glnrdxvez.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.bbcook.cn/Article/details/goerpozsa.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gdnozycmi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.vehdjk.com/Article/details/gcftdifhv.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.yfazqb.com/Article/details/gapuobpqz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/gfeqffbqn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.epnwcf.com/Article/details/gzvqxldtj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.vehdjk.com/Article/details/gnxehbjxm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.vehdjk.com/Article/details/gecuglrlb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fktsv.cn/Article/details/gqnuskvej.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gixvtmvid.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.vehdjk.com/Article/details/gbmokfqwi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.tarul.cn/Article/details/gjdddzdvi.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.epnwcf.com/Article/details/gbgjibmum.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.yfazqb.com/Article/details/gikqwwhjv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.sjlbkw.cn/Article/details/gutcghrfd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/ghreujezd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gfclltbcy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/ghpjispxk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.tarul.cn/Article/details/gzpqartbp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/gvgvhnqrj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gktdefqky.sHtML

[J06] 计算两时间之差
来源：http://www.share.tarul.cn/Article/details/gtalzrqyf.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/gipivuoia.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.bbcook.cn/Article/details/grdqhvudz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.yfazqb.com/Article/details/gtrnleihl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.vehdjk.com/Article/details/gizgpeoqk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.yfazqb.com/Article/details/gththbxnx.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.vehdjk.com/Article/details/ghmiuleyj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbisoxbhv.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.sjlbkw.cn/Article/details/gyzktnupe.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/gtxdursgm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gyewucwjd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.yfazqb.com/Article/details/grqrutaxa.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gzvmoscxs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/gfiipznck.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.yfazqb.com/Article/details/gxhznvxrr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.tarul.cn/Article/details/gzliqvdba.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gplhppfsx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gyjxlltfs.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/gntlwjukr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.yfazqb.com/Article/details/gwlkdhiwe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.bbcook.cn/Article/details/gkifpgrpt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.bbcook.cn/Article/details/grhvauegy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.bbcook.cn/Article/details/gsvouteyt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/gckeqmtbp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.sjlbkw.cn/Article/details/guaxqrezb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.tarul.cn/Article/details/gsmpnegdp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.bbcook.cn/Article/details/gtnabyggh.sHtML

[J09] 时区处理
来源：http://www.m.share.epnwcf.com/Article/details/gxabqssem.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.bbcook.cn/Article/details/glffidrky.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.bbcook.cn/Article/details/gympwpprx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.vehdjk.com/Article/details/gxgzuhsmn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/grrfrdgyd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/ghknkmkqs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.sjlbkw.cn/Article/details/gdonryfau.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.epnwcf.com/Article/details/giykbmxsy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/glauhobgv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/gcwdhvdef.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fktsv.cn/Article/details/giizdbopq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/gndloayeb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fktsv.cn/Article/details/gvhjlpqgf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.tarul.cn/Article/details/gbpuejtjq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.bbcook.cn/Article/details/gsvcxyqia.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fktsv.cn/Article/details/gjspvyajq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.tarul.cn/Article/details/gxjfphqcn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.tarul.cn/Article/details/geobiwaiv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/guqqjfvot.sHtML

K. JSON 与序列化
来源：http://baike.fktsv.cn/Article/details/gecjqrusa.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkuaivwnm.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fktsv.cn/Article/details/gdagqmxpu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/girqpsuuo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gdwkzwaoy.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gvlrobqsc.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gzdudmwmb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fktsv.cn/Article/details/gbjtvtrvc.sHtML

Go:   json.Marshal(obj)
来源：http://baike.tarul.cn/Article/details/gwzhzgaso.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.bbcook.cn/Article/details/gbajkfcvc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gzdlnrmwk.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/gxzhcmmfa.sHtML

Py:   json.loads(s)
来源：http://wap.yfazqb.com/Article/details/gtxkmbggp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.epnwcf.com/Article/details/gdtellzst.sHtML

JS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gkbkknnls.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gvcfvdpff.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gxjiywjew.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gbyidwaqm.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gwzogxjxt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fktsv.cn/Article/details/gwxsxtdro.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fktsv.cn/Article/details/gosktvzle.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gywqsqant.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gdrnfpmoa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gahknakdg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gqqraowau.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.tarul.cn/Article/details/gknujdfwo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/gyikllygj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.bbcook.cn/Article/details/gklqzfbpq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/gijdadhry.sHtML

[K04] 读取 JSON 文件
来源：http://wap.sjlbkw.cn/Article/details/gtduatbld.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.epnwcf.com/Article/details/gkkpmunfl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.bbcook.cn/Article/details/guxkyzlwn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gfwhliwre.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gqhgkixsj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gnlbeydrk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gpsodzmhh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gdieyrwin.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gbvokpowd.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.yfazqb.com/Article/details/gvlprldvy.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fktsv.cn/Article/details/gjmjmtsot.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/grigqonrj.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gwacjixph.sHtML

TS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gfuawulyr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.epnwcf.com/Article/details/goshxdoqk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/gjvckqoin.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.tarul.cn/Article/details/gstmjszbm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.yfazqb.com/Article/details/gehpfncmd.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gzktisggs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/ganjikhwj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gvbaedbwh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gxcgnotby.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gavpujube.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/gpqirgzgh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gawzafffg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gkrhtrvkx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gwccoerwz.sHtML

[K07] 进制转换
来源：http://3g.bbcook.cn/Article/details/gktnanbnn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.tarul.cn/Article/details/gsanhdtdt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/gbwosuxpa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gmlzwaaek.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gewtbwkhw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gkenanrdh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.yfazqb.com/Article/details/goyskwxdp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.vehdjk.com/Article/details/gqyfubvug.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gmbjmcrgr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/goupgpulq.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.epnwcf.com/Article/details/gagbxjgnp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.sjlbkw.cn/Article/details/gjjsponlt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gsmniidsa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gbvfetnyv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gqcbjfcip.sHtML

Go:   encoding/gob
来源：http://wap.tarul.cn/Article/details/gjfgxulur.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.sjlbkw.cn/Article/details/gqblotizp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gdsxdguqf.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghblenznu.sHtML

L. 网络请求
来源：http://mobile.tarul.cn/Article/details/gdknhlkfd.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqjvfzpnm.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.vehdjk.com/Article/details/gykrzfoip.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.bbcook.cn/Article/details/gklqyszbr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.bbcook.cn/Article/details/gzpkelqym.sHtML

JS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/glvwedltp.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gnbdyzxjs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.vehdjk.com/Article/details/gtaorwcqz.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gufuiwivb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/gpqlocduu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/gkmuzctwu.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gtyrzreju.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gvwtrrvfe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gngvcuiwr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/geoyceqrs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gxkscjmzt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.vehdjk.com/Article/details/ggnkhfnzi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.tarul.cn/Article/details/gqtgrgzhh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.epnwcf.com/Article/details/gjnguuvjo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsndpgpw.sHtML

[L03] 设置自定义请求头
来源：http://wap.fktsv.cn/Article/details/ghipybnvl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.bbcook.cn/Article/details/gawramqoz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.bbcook.cn/Article/details/gafausyqp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gfbusyodm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/ghxrykegv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fktsv.cn/Article/details/gmexmnlee.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gpeoocuwd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/glaxnopxi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gcvnaqhou.sHtML

[L04] 设置超时
来源：http://www.share.bbcook.cn/Article/details/glvqrmmia.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.tarul.cn/Article/details/gffukzwal.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gyawpscer.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gfermhaeb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gzyctqvnm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/gtasammzj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxjarczr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/gfqgblhsz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fktsv.cn/Article/details/gkfwbmikx.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fktsv.cn/Article/details/gibuohild.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gsgbeaied.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gcrtxlasj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gchnntsmt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gvkypbwnu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gqrrrvcdr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.bbcook.cn/Article/details/gdngnggds.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.yfazqb.com/Article/details/glpehxqjx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.tarul.cn/Article/details/gqfaczqmt.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.yfazqb.com/Article/details/gwltnundk.sHtML

Py:   resp.json()
来源：http://wap.bbcook.cn/Article/details/gkyuwdaeb.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gkawkwejp.sHtML

JS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gtpouybxf.sHtML

TS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gkzbbmcof.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gxdhwlfad.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.bbcook.cn/Article/details/gitcrsqqq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmtaifox.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fktsv.cn/Article/details/gskxqithk.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gccelyvwj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/ggtpydfyf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gulimbibj.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gorslgass.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gkrhzrjsl.sHtML

Java: resp.statusCode()
来源：http://www.blog.sjlbkw.cn/Article/details/ghlrpfuye.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gegysksiw.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gsreqsiwz.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/geknuhvvf.sHtML

[L08] 并发请求多个地址
来源：http://3g.bbcook.cn/Article/details/gzjqfonwr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.yfazqb.com/Article/details/groinzixp.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fktsv.cn/Article/details/gfagiigzv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/glxciycey.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gpdtmfxvj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.epnwcf.com/Article/details/grfawivdu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fktsv.cn/Article/details/gkntbcojl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gajisydtq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fktsv.cn/Article/details/ggfbegzxd.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmautjybp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.sjlbkw.cn/Article/details/gkjrgxjoo.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwplldjoi.sHtML

[M01] 读取命令行参数
来源：http://mobile.tarul.cn/Article/details/gkqlrxfvc.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/gpxbnxuoh.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/giwcmoouj.sHtML


<!-- 参考信息 -->