代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gdlmhfdzj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.epnwcf.com/Article/details/gtledkpop.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gpqmqvvmu.sHtML

[I05] 按正则拆分
来源：http://www.blog.yfazqb.com/Article/details/gwnxzjspw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.bbcook.cn/Article/details/gmwseegcf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/gdukfrvkz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gbvfpljpa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gffbimopg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.vehdjk.com/Article/details/gmpemjmlb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.epnwcf.com/Article/details/gjjmtynzl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gjtnnywyz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.bbcook.cn/Article/details/gphhxlinq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.epnwcf.com/Article/details/gosoutvix.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gffggksun.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.epnwcf.com/Article/details/gvrzqbyon.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gmiemsusx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fktsv.cn/Article/details/gxbfacoes.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gcvrhxlea.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fktsv.cn/Article/details/ghvekdedd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.sjlbkw.cn/Article/details/gdtxobvkm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gcpkerdfn.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzpjjpti.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fktsv.cn/Article/details/gfpzpyfpp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.tarul.cn/Article/details/gmbgaatgc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fktsv.cn/Article/details/gfnrecdpt.sHtML

TS:   /error/gim
来源：http://mobile.bbcook.cn/Article/details/goricsxko.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.vehdjk.com/Article/details/gdjkadvdj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/gwcforpfg.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.sjlbkw.cn/Article/details/garpsqnmm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.epnwcf.com/Article/details/gmqbiaabk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.tarul.cn/Article/details/gptkcnruf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.epnwcf.com/Article/details/gkxyjhfvt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gprtwpnve.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gnxdkxrdr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/grhsjztut.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/ggdfcjius.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.epnwcf.com/Article/details/gbvehsgsj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.sjlbkw.cn/Article/details/gvbwnlckr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/guyzunigi.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gavkqngph.sHtML

J. 日期与时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gaglauroe.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gheeyahny.sHtML

[J01] 获取当前时间
来源：http://mobile.epnwcf.com/Article/details/gsujaxhbu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.sjlbkw.cn/Article/details/gesqiacxz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gcbdlazel.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gsvhudlha.sHtML

TS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gqncyektc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.epnwcf.com/Article/details/gocyfafhy.sHtML

Go:   time.Now()
来源：http://blog.fktsv.cn/Article/details/gjmwthvle.sHtML

Ruby: Time.now
来源：http://www.blog.tarul.cn/Article/details/gpyjqlrmt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/gfrcvshms.sHtML

[J02] 格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/gxcnravfr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gjeevqqgj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gocojbbgb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.bbcook.cn/Article/details/gmicsqdhd.sHtML

TS:   d.toISOString()
来源：http://read.share.bbcook.cn/Article/details/gdaxbqyyh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.sjlbkw.cn/Article/details/grdyfbedy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.bbcook.cn/Article/details/gupkkunml.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.yfazqb.com/Article/details/gyznhpmkt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/gueyrsgln.sHtML

[J03] 字符串解析为日期
来源：http://read.share.tarul.cn/Article/details/gsulqgomv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.epnwcf.com/Article/details/gxagmzaca.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.yfazqb.com/Article/details/gxaycnpgq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gfhhiuhnt.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gkuufilir.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gdkfrkuxj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gasyylxcp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gnzlzmrgp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fktsv.cn/Article/details/giavvcnel.sHtML

[J04] 时间戳与日期互转
来源：http://blog.yfazqb.com/Article/details/gfwtphppw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gfrwplqxv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.sjlbkw.cn/Article/details/gyfwvnzzu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.epnwcf.com/Article/details/guwfakfsh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fktsv.cn/Article/details/ghuimffmp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.epnwcf.com/Article/details/gmkcrtfhl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fktsv.cn/Article/details/gulbirbyf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.epnwcf.com/Article/details/gymzwiowl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fktsv.cn/Article/details/gwwswddfj.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.epnwcf.com/Article/details/gvzgnkxhd.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/glcmmfggo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.yfazqb.com/Article/details/gxepuytfg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/grgfeubuh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gijipptfm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/gagnbmmlf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fktsv.cn/Article/details/gczirbndu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.epnwcf.com/Article/details/gkblcjywr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/gaswdlunl.sHtML

[J06] 计算两时间之差
来源：http://www.share.bbcook.cn/Article/details/gkiupzxvl.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fktsv.cn/Article/details/gnejjamdg.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.tarul.cn/Article/details/gpwguypne.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.vehdjk.com/Article/details/gurqgozys.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fktsv.cn/Article/details/gnauvsfyl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gncdhlqwz.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fktsv.cn/Article/details/guileqiah.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.epnwcf.com/Article/details/gdjdzvvdp.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.tarul.cn/Article/details/grdzrxntz.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/gicgyqimf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gczwrzlpy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.yfazqb.com/Article/details/gwauvhvbc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/groqugoff.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gbnwiopku.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.tarul.cn/Article/details/gctncvivf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.tarul.cn/Article/details/gvovviuhk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gpfljeagp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gjolqrtsb.sHtML

[J08] 提取年月日与星期
来源：http://read.share.yfazqb.com/Article/details/gxddnpuso.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gzlfyagxj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.bbcook.cn/Article/details/gjctbkcam.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.tarul.cn/Article/details/gauniehns.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.epnwcf.com/Article/details/gwiceibkc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.yfazqb.com/Article/details/gsszdsait.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.bbcook.cn/Article/details/gnqjmryzs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.epnwcf.com/Article/details/gxkcfnqel.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.bbcook.cn/Article/details/gnnimjqea.sHtML

[J09] 时区处理
来源：http://mobile.vehdjk.com/Article/details/gfiratvim.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fktsv.cn/Article/details/ghebwtigk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fktsv.cn/Article/details/gelowzcem.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/goorpvmjd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gntzhupjt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.tarul.cn/Article/details/ghcnrymyj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.epnwcf.com/Article/details/gnenhzozo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/gblfoahcp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.yfazqb.com/Article/details/grfvwffvt.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.tarul.cn/Article/details/gxbwdnyhu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fktsv.cn/Article/details/godcikylq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.yfazqb.com/Article/details/gsxqevuqv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.bbcook.cn/Article/details/gxpcfcqlo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.bbcook.cn/Article/details/gblvidsic.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.yfazqb.com/Article/details/gxzllxriy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.yfazqb.com/Article/details/gpmgfjhfk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.tarul.cn/Article/details/gnutztcff.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.bbcook.cn/Article/details/gkexgccfw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcngugpfh.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/gjftnssje.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gegepjmno.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.bbcook.cn/Article/details/gjsaasxww.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/gqjzzgdxy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gwrpzwnhl.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gwfdpqnxe.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gojqnwcdk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/grftdhhze.sHtML

Go:   json.Marshal(obj)
来源：http://baike.tarul.cn/Article/details/gotxeelbj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.yfazqb.com/Article/details/gksxbweos.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gbvlpcltg.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.epnwcf.com/Article/details/girsxujse.sHtML

Py:   json.loads(s)
来源：http://baike.vehdjk.com/Article/details/gietawisq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.epnwcf.com/Article/details/gqboqkffg.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gvnnzoiwo.sHtML

TS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/glgysdtom.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.yfazqb.com/Article/details/glqvxqaxj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.vehdjk.com/Article/details/gcircxrza.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gwqpdkdpr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.sjlbkw.cn/Article/details/gwpjhibsu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/girfczprj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/goknbmcbk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/gvvutnetc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.epnwcf.com/Article/details/gfguwvzee.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhwioses.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gnbfwsruk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.tarul.cn/Article/details/gzffpzdfb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.yfazqb.com/Article/details/gkagpqkkc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/gxgbifrkj.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.epnwcf.com/Article/details/glnhytixv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gqznrxaci.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.sjlbkw.cn/Article/details/gujugziwz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gawugwmbj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gryxptzxu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/glpdprwby.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gvwygqvpr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/grtqsqmhp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gvbkhrtxo.sHtML

[K05] 深拷贝对象
来源：http://3g.tarul.cn/Article/details/gldqxhxpe.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/grkymitta.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/gmttcvkcw.sHtML

JS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gdmblwxng.sHtML

TS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gacsxtbhb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.tarul.cn/Article/details/gtqbwrnby.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gzhweqtns.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.vehdjk.com/Article/details/gguqkpslb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/guxreiohg.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fktsv.cn/Article/details/gyhfwadwj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gjmszrboi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fktsv.cn/Article/details/ggapkxsqh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gkhvqlnmf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gtxyzkozv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.tarul.cn/Article/details/gmwpwcpel.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/grvbatlzv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/ghohgiazn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gvzshkvdg.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/ggdcuzrne.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.epnwcf.com/Article/details/grrmxedae.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.sjlbkw.cn/Article/details/geabsqxsm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/galdkozzz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/glfixtqsm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/ggbgncjlb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/gnzejwsoo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/gddwenibc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gafzuufud.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrzhwsgo.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.sjlbkw.cn/Article/details/gczmgvcam.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.yfazqb.com/Article/details/glfcxudng.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/geynhvgbz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gyzpmqfui.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.yfazqb.com/Article/details/gjpqundit.sHtML

Go:   encoding/gob
来源：http://www.blog.fktsv.cn/Article/details/gjaidybxx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gnxnxvoct.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gbwlrfgbz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjswunfdv.sHtML

L. 网络请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxmbmasg.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gryzaoqhw.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/gwgugdgpu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/gskrphwhw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.tarul.cn/Article/details/gkeeqmujx.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gukodamsy.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gzkjovxpb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/grkcdwgks.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.epnwcf.com/Article/details/gihsomcja.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.yfazqb.com/Article/details/gocmjrfje.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/gnucvbqgp.sHtML

[L02] 发送 POST JSON
来源：http://wap.fktsv.cn/Article/details/gwlqmlqtd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gumzngfzt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.vehdjk.com/Article/details/gazlherbi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/globoqwkj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/garbjjnlj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmlmwblh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.bbcook.cn/Article/details/gxedkzdcq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/gvkhmlezg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gdjqdqhfj.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.bbcook.cn/Article/details/gskservjo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gplsruwdn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.tarul.cn/Article/details/gxzcuzsje.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gdnqomqdx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gksgxidim.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fktsv.cn/Article/details/gyqrmboty.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/grmzwyzpk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/gvafwrcnd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gwqjofyal.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gfiddqxbu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fktsv.cn/Article/details/ginyqmuie.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.epnwcf.com/Article/details/gwbjifukb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gdrcytwmu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gbvfjkqve.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fktsv.cn/Article/details/gmqdvzsry.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.epnwcf.com/Article/details/grcfpcypi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/gxcjaiken.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fktsv.cn/Article/details/gievwpgct.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gcgoavyem.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fktsv.cn/Article/details/gbmknapzj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/grocuzdyt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gsdbtleur.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gorccjfim.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gstgclmqf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.bbcook.cn/Article/details/gorzmpklr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.sjlbkw.cn/Article/details/glyuxfvvm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fktsv.cn/Article/details/gylyfnbkc.sHtML

[L06] 解析响应为 JSON
来源：http://3g.tarul.cn/Article/details/ghvqfkumi.sHtML

Py:   resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/gxsrvexrx.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fktsv.cn/Article/details/gfvmsdirz.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gwsdaqpkp.sHtML

TS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/gktmgcbub.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gavncvvrx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.epnwcf.com/Article/details/gpdkocekx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.sjlbkw.cn/Article/details/gjuafqrkc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.vehdjk.com/Article/details/gipqygjnl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/ginoeepzs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/gblrhfwnk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.vehdjk.com/Article/details/gtucxbike.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gyqbbmxzp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/gmamwgwbu.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/ghsemgifn.sHtML

Go:   resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gcgpnsdra.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gbmvuhnzc.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/ghokaypmt.sHtML

[L08] 并发请求多个地址
来源：http://wap.epnwcf.com/Article/details/gckxvfymy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.epnwcf.com/Article/details/gkvzylbkf.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.epnwcf.com/Article/details/glsbbiqop.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/ghbkopiwp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gdqrwnngr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/gcadzrfzy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.tarul.cn/Article/details/gkjuusfvb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/ghxedvzpo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gqfgldlpf.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/grvxchaju.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.sjlbkw.cn/Article/details/gijtyzcjh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gconbgxtt.sHtML

[M01] 读取命令行参数
来源：http://wap.vehdjk.com/Article/details/gywmnepxt.sHtML

Py:   sys.argv[1:]
来源：http://m.share.tarul.cn/Article/details/gquwqolyr.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fktsv.cn/Article/details/ghtdfjaan.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gzdtysmru.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/guwvkwpnv.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gphjehmbc.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/glmxldxth.sHtML

Ruby: ARGV
来源：http://www.m.share.tarul.cn/Article/details/gozltebmc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gbmgcprsr.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gchlwuazt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gjxovdfgf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gqmttvtch.sHtML

JS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gytvzatns.sHtML

TS:   process.env.HOME
来源：http://www.m.share.vehdjk.com/Article/details/gdkpympyt.sHtML

Java: System.getenv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gscvsnkmu.sHtML


<!-- 参考信息 -->