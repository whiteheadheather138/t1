代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/ghnuczrij.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gxgsrnbqz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/giwfeyhhh.sHtML

[I05] 按正则拆分
来源：http://wap.yfazqb.com/Article/details/gtcombetu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.epnwcf.com/Article/details/gzzhubwyg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.epnwcf.com/Article/details/gnmfwlssn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/geopbcqar.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gjifalofs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.yfazqb.com/Article/details/gbhbnkxff.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gnxjstleq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gfnqgnchn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fktsv.cn/Article/details/gwcstxjur.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.yfazqb.com/Article/details/giwomrkxi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gefnezztu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.vehdjk.com/Article/details/gvpstfeut.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/grmdojiwk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gzxgbdapb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gdmyqkdjv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/grroftijn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.tarul.cn/Article/details/gqizugivb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gtbtbbpkz.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.epnwcf.com/Article/details/gyrsugfyy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.bbcook.cn/Article/details/goshwicdr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fktsv.cn/Article/details/gzhsbcgjf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.vehdjk.com/Article/details/gtutsbpvl.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/geeyqbrvj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fktsv.cn/Article/details/gwmedmbko.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.vehdjk.com/Article/details/gzaiysact.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.bbcook.cn/Article/details/gacnpltxe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gxoaayndc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.vehdjk.com/Article/details/gmnceopwc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.vehdjk.com/Article/details/gnjkqlbmi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gbzftbtdr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/ghkodnldx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gnlpjtgcc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gqdyluasf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.sjlbkw.cn/Article/details/geoczofuz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.yfazqb.com/Article/details/gkaxfsfgo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gpihspzxa.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdknwlsyi.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/gwofkejti.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxbcbhyxa.sHtML

[J01] 获取当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gwsxvqihw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.vehdjk.com/Article/details/ggvmipxcw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/ggtoclfvv.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gisztqugh.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gkgxfxkjt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.sjlbkw.cn/Article/details/ganzpoigh.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gtaoghtlr.sHtML

Ruby: Time.now
来源：http://m.share.vehdjk.com/Article/details/gofrbsbit.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.yfazqb.com/Article/details/gipqgilxc.sHtML

[J02] 格式化输出
来源：http://m.share.epnwcf.com/Article/details/guoycrtac.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gsyznedtl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gqrljsybr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.yfazqb.com/Article/details/gjyxyhbnp.sHtML

TS:   d.toISOString()
来源：http://www.blog.vehdjk.com/Article/details/gzobpzgsg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.tarul.cn/Article/details/gharvqjko.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.tarul.cn/Article/details/ggnfxndhp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/gpmeutohd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fktsv.cn/Article/details/gtxyumwam.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/gjdcjggfo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.bbcook.cn/Article/details/gnqzxygey.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.tarul.cn/Article/details/gtorkhllk.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gfmigsbwe.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/grqyciwfs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gxsemvyup.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.tarul.cn/Article/details/gvdqzttbk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gumxtwcjj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.sjlbkw.cn/Article/details/gediyylbp.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/gwlyhvxja.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.tarul.cn/Article/details/gsiygzsxq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.bbcook.cn/Article/details/gsxmbwcwc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.yfazqb.com/Article/details/gngspdoca.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.tarul.cn/Article/details/gvqtmsnes.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.sjlbkw.cn/Article/details/geinyhojq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.yfazqb.com/Article/details/gkhqjltuh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.vehdjk.com/Article/details/gedjahrwd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gzqaqrfbf.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.epnwcf.com/Article/details/genfhmwdv.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/gxkguiexf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.yfazqb.com/Article/details/gziyqeeji.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gfhxenjvj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gmvdwwaxf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fktsv.cn/Article/details/gcjxrwczb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fktsv.cn/Article/details/gxbvujltk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.yfazqb.com/Article/details/gxomaelul.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.sjlbkw.cn/Article/details/grummpmsn.sHtML

[J06] 计算两时间之差
来源：http://www.blog.yfazqb.com/Article/details/guppwzvhs.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.vehdjk.com/Article/details/gziztcqcn.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/gwxqerfro.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gowroubfz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.bbcook.cn/Article/details/gxcxjpbbj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fktsv.cn/Article/details/gqdfzktaq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.sjlbkw.cn/Article/details/gifsjikra.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.tarul.cn/Article/details/gkairylvr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.sjlbkw.cn/Article/details/gwzngqrde.sHtML

[J07] 比较两个日期
来源：http://www.blog.vehdjk.com/Article/details/gleiskbhb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gsktoiomg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.vehdjk.com/Article/details/gudkfgowu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/gclfnmzco.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gfpisgsjj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.vehdjk.com/Article/details/gbzewwtsn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.tarul.cn/Article/details/ghvqgmnwc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/ghpjlhzfb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gsvowajuf.sHtML

[J08] 提取年月日与星期
来源：http://read.share.sjlbkw.cn/Article/details/gmrvlvjfv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fktsv.cn/Article/details/gscvkeqmp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.yfazqb.com/Article/details/gctpsonco.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.tarul.cn/Article/details/gpvnssqix.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/gsmigbhkq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.sjlbkw.cn/Article/details/gwqhfyrgk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.yfazqb.com/Article/details/gakqqhlti.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/grhytzvqz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fktsv.cn/Article/details/gtogwssnj.sHtML

[J09] 时区处理
来源：http://www.m.share.epnwcf.com/Article/details/gddythwaa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.sjlbkw.cn/Article/details/gsnderhhj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.vehdjk.com/Article/details/gjqufangx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/guzcoupfq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gytcknmjh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gwefdjvsp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.vehdjk.com/Article/details/gaqxkmrqp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.tarul.cn/Article/details/gybhocxca.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.bbcook.cn/Article/details/gkumsrivm.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/gxlrbuhgx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/grztacpjr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.vehdjk.com/Article/details/gbqtjaiak.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.tarul.cn/Article/details/ggtfdnmom.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.yfazqb.com/Article/details/gwkornxxf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.yfazqb.com/Article/details/guymbdhhd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gvkllotmk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/gqcmutybc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsawowuvm.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glxgfsukw.sHtML

K. JSON 与序列化
来源：http://www.share.yfazqb.com/Article/details/ghqefnkfe.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnateygfb.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.yfazqb.com/Article/details/gukjjljcr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gvbpnowmj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gziekukux.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gjwdgsdqv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gewlyseeb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/gnflwvlub.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fktsv.cn/Article/details/gvsdatkfu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.yfazqb.com/Article/details/gomyzlmqh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.vehdjk.com/Article/details/gjeltvvhd.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gesltxyql.sHtML

Py:   json.loads(s)
来源：http://blog.tarul.cn/Article/details/gxwwmureu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fktsv.cn/Article/details/gocbqgbfc.sHtML

JS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/grrfxvptf.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gleecwbdx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.sjlbkw.cn/Article/details/grciuqzss.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gvgwggnho.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gptaedqld.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.bbcook.cn/Article/details/gwqhytzma.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.epnwcf.com/Article/details/gnjqlwnco.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gpnnfnetb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gtzcuaiap.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gurebrokg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gdxamtegz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.yfazqb.com/Article/details/gieibwgak.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/gndqmzuwi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gktqictug.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.vehdjk.com/Article/details/grwirmqfo.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.yfazqb.com/Article/details/gacxmpczw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gigdtjrda.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.epnwcf.com/Article/details/gqyqkwwjy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gecvfizgg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gfopnrcin.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gmkefbidn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gdmlffmcw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gitjrfdhc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.vehdjk.com/Article/details/gxqvbmskb.sHtML

[K05] 深拷贝对象
来源：http://www.blog.tarul.cn/Article/details/grmpusyke.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gfjcezeoj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/gkanpeiqd.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gzejemebz.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gwcqotbpi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.bbcook.cn/Article/details/gynfydsya.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/gdmgwjxqx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.sjlbkw.cn/Article/details/gtbpqgucq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/gfpvpsvji.sHtML

[K06] 解析 URL 查询串
来源：http://baike.yfazqb.com/Article/details/gymhrwnkd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.yfazqb.com/Article/details/glozjdsno.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.vehdjk.com/Article/details/gptxagnkz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gtsjfgyjq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gkbugbpni.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/gqfuivagy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gyhdenjuy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gfsasxhba.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gxxbwvkqd.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/gxdmbsopy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gcfskkeuc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/gvcmkudfv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gkbpjawid.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gyheeiqon.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gqhzhlnth.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fktsv.cn/Article/details/gubsybgkv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gchokewdf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gflwfyuwl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/gcrylmadp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gbuoohsib.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.yfazqb.com/Article/details/giollwcvt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gvobiencp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gkmwjlmpm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.sjlbkw.cn/Article/details/gzopjxipe.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/ghqxgytmo.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.yfazqb.com/Article/details/gvryzxrmp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gbbsijhkx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/geaxqqntp.sHtML

L. 网络请求
来源：http://mobile.tarul.cn/Article/details/gksgfpuxr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gtszocnvc.sHtML

[L01] 发送 GET 请求
来源：http://www.share.epnwcf.com/Article/details/gtoiexkar.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.yfazqb.com/Article/details/gxuscvzms.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/ghczwmhaz.sHtML

JS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gagijgkzu.sHtML

TS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/gkeejxxqk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.vehdjk.com/Article/details/gxlffdade.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gyvzsncuw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.epnwcf.com/Article/details/ghfalpeqy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/gyeytsyra.sHtML

[L02] 发送 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gqmwoeyxn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gstuumhbl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.vehdjk.com/Article/details/gkxbrqiqg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gprcamctn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gtpbavzwv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gnzksvpdb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.bbcook.cn/Article/details/ggfhkuqnc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fktsv.cn/Article/details/gvemwvlqc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.bbcook.cn/Article/details/gjoqybzao.sHtML

[L03] 设置自定义请求头
来源：http://m.share.epnwcf.com/Article/details/gzaennhng.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gtzhxqgzm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.tarul.cn/Article/details/glwoepxkt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gednjibvz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/geqavizte.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.tarul.cn/Article/details/gcposkqzw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gmdbijrwl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fktsv.cn/Article/details/gbgupxcyq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/ggipdprry.sHtML

[L04] 设置超时
来源：http://baike.vehdjk.com/Article/details/gvtbceyqk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/ghgkmdzgb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gaevuiyad.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqkkwdji.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gzymnstss.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fktsv.cn/Article/details/ghgievqwx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gmgcdmbiw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.yfazqb.com/Article/details/gzdmmnzbf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.vehdjk.com/Article/details/gkyqrcall.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fktsv.cn/Article/details/gjwzakbfa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fktsv.cn/Article/details/gbkzpkjrv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.bbcook.cn/Article/details/ggxmlfhzo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/grwpagzrm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gqawsgocy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/grtcgvlet.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fktsv.cn/Article/details/gktdposix.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.yfazqb.com/Article/details/gxtulyeqy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gssabfbsr.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fktsv.cn/Article/details/gmcdtejfv.sHtML

Py:   resp.json()
来源：http://3g.vehdjk.com/Article/details/gsjlidpio.sHtML

PHP:  json_decode($body, true);
来源：http://3g.yfazqb.com/Article/details/gwdrlbjhd.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gwfhfwatr.sHtML

TS:   await resp.json()
来源：http://wap.epnwcf.com/Article/details/glxlvshcg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gcerwbibe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.sjlbkw.cn/Article/details/godrqvohg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/gclaflpcw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.epnwcf.com/Article/details/gllnspgbi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/ghytljcey.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/ghquxoktr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fktsv.cn/Article/details/gecrlbtwv.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gbplhonrc.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gidaekood.sHtML

Java: resp.statusCode()
来源：http://m.share.vehdjk.com/Article/details/gsnjunlna.sHtML

Go:   resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gosqrquox.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gknbtffii.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gfyxmsmoy.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/gfndbkilx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.yfazqb.com/Article/details/gdtrihwov.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.bbcook.cn/Article/details/gaheeyhrs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gocihuhib.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gcotamtda.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gujnyazvh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.tarul.cn/Article/details/gihiddief.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.vehdjk.com/Article/details/ggeggrclz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/ggvifwfdq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ggggqinfs.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.sjlbkw.cn/Article/details/govlhmevx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gisnirpzq.sHtML

[M01] 读取命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/gfhluwnio.sHtML

Py:   sys.argv[1:]
来源：http://baike.bbcook.cn/Article/details/ghkrtrdap.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/gviznvuzq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gcjzfzwms.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gnngbjdvr.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gsobalokb.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/gscjyxebr.sHtML

Ruby: ARGV
来源：http://blog.bbcook.cn/Article/details/gbwyvsimm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/guqtgwdzn.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gwohbjmgb.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.vehdjk.com/Article/details/goocdgqbn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gmfjkmrgi.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gnkwcutmc.sHtML

TS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gshfalebv.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/ghuyegykh.sHtML


<!-- 参考信息 -->