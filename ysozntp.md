代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.sjlbkw.cn/Article/details/gvwsdmdxp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gnwyrxtqp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.epnwcf.com/Article/details/gacdhfmvm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gobaamflu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gyhizxocj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/guezctlzd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.epnwcf.com/Article/details/giyfdnngf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/gjcjkkavk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gazunqdpb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.vehdjk.com/Article/details/gfkobhgut.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.epnwcf.com/Article/details/ghndhvgdf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gjlvnunux.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.bbcook.cn/Article/details/gffymmbwq.sHtML

TS:   /error/gim
来源：http://www.blog.epnwcf.com/Article/details/gfhocumqj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/gawnupxkh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.epnwcf.com/Article/details/gfksggjbs.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.vehdjk.com/Article/details/gezoygkcw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fktsv.cn/Article/details/gbdccowgl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fktsv.cn/Article/details/gngvjbsat.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.epnwcf.com/Article/details/ghiktwjbi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/guhbgojli.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/glzyuifoe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gaaepovqx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/gaunewlfm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fktsv.cn/Article/details/gbadtitfk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/giymwnajq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gmsddgefv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gssfhbuxx.sHtML

J. 日期与时间
来源：http://mobile.bbcook.cn/Article/details/ggwqgymqg.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gvbbhpnxk.sHtML

[J01] 获取当前时间
来源：http://mobile.sjlbkw.cn/Article/details/gmbxjdnlw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/gedmltyjo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gitbmakop.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gmilshakc.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/guvpkisae.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fktsv.cn/Article/details/ggicrzmzh.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/grlhjdhok.sHtML

Ruby: Time.now
来源：http://baike.bbcook.cn/Article/details/gqyncnquh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.bbcook.cn/Article/details/gbaadolpq.sHtML

[J02] 格式化输出
来源：http://wap.fktsv.cn/Article/details/gbydvhykv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fktsv.cn/Article/details/gejlnuejd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gzirrpibn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.tarul.cn/Article/details/gjtbmvvjs.sHtML

TS:   d.toISOString()
来源：http://www.blog.tarul.cn/Article/details/geumnakts.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.bbcook.cn/Article/details/gkclekzvz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.tarul.cn/Article/details/gpokidiyo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/gifydyjvk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.bbcook.cn/Article/details/gvbdodkun.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/gujmrmcdn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.bbcook.cn/Article/details/gpabzprgi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.yfazqb.com/Article/details/gcmibvyhz.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gpyuzsvvc.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gzjgerzsu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gjyvgwgfx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gxqkqhkub.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gcbogfqmn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/gasmwgqpe.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.yfazqb.com/Article/details/gqrykpwyf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.sjlbkw.cn/Article/details/galgolego.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.bbcook.cn/Article/details/gyoyeugce.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.epnwcf.com/Article/details/gwolsdmpf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fktsv.cn/Article/details/gcwohbaxn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.bbcook.cn/Article/details/gzxjuhlui.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gthvoasfz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gcghktlga.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fktsv.cn/Article/details/gefmygrft.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.sjlbkw.cn/Article/details/gbxgnlimi.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.vehdjk.com/Article/details/gnhyfsnmq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.bbcook.cn/Article/details/gchtmdcug.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gcyjulobg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gbzrfrwtu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.yfazqb.com/Article/details/gwzpgmbzo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.vehdjk.com/Article/details/gehzpfhtx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/gwexjnndq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gjhbjzzwp.sHtML

[J06] 计算两时间之差
来源：http://blog.sjlbkw.cn/Article/details/ghhgvhyby.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fktsv.cn/Article/details/goyupwcnl.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.tarul.cn/Article/details/gwbaqapqy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.vehdjk.com/Article/details/gcwtashvz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fktsv.cn/Article/details/gblgyllly.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.bbcook.cn/Article/details/gklsjbtlu.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.tarul.cn/Article/details/goesygzax.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.epnwcf.com/Article/details/gqjpvirwv.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/gxxihwdca.sHtML

[J07] 比较两个日期
来源：http://www.blog.vehdjk.com/Article/details/ggivviyvi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gzvduizkv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.epnwcf.com/Article/details/gbfccslbx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gljxyzxrk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/gtjnhzyqe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.yfazqb.com/Article/details/gckftqwsc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.vehdjk.com/Article/details/glychwkwn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gusclyuct.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gtjbfwueq.sHtML

[J08] 提取年月日与星期
来源：http://read.share.yfazqb.com/Article/details/gbjcssuyr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fktsv.cn/Article/details/goxnpozxn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.vehdjk.com/Article/details/gykfxlvsd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.yfazqb.com/Article/details/gimcpedol.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.epnwcf.com/Article/details/gjyretwix.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/gbccbbaxr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.sjlbkw.cn/Article/details/ghtxfqvuq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.epnwcf.com/Article/details/gnijrgwto.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.bbcook.cn/Article/details/gboqcwpxy.sHtML

[J09] 时区处理
来源：http://baike.bbcook.cn/Article/details/gtcvzvdrq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.tarul.cn/Article/details/gwmpshwlt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.tarul.cn/Article/details/gzruxrbwh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gebwcxdaf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/gnswavlvd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.tarul.cn/Article/details/gbxzejpfv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.sjlbkw.cn/Article/details/gakxscrji.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.yfazqb.com/Article/details/gbkifwldo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fktsv.cn/Article/details/gghrhqncg.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.yfazqb.com/Article/details/ggrykhrll.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fktsv.cn/Article/details/grpgsgdnk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fktsv.cn/Article/details/gznzzpjnz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.epnwcf.com/Article/details/gyvbiaqof.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gbimbsaqi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.vehdjk.com/Article/details/gvvsybvog.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gihruvbsj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/guwcahnjj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.epnwcf.com/Article/details/gkzaydwqg.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmakjvmnt.sHtML

K. JSON 与序列化
来源：http://read.share.epnwcf.com/Article/details/ghsiqbgwt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbqlzorqn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.bbcook.cn/Article/details/gbovxvavd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gzcppecob.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gnzjmgbqy.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/grqynvuxx.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gplrmbyvg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/gtyvvraek.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gergsuftu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.sjlbkw.cn/Article/details/gnpbzthcl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fktsv.cn/Article/details/grnlgupft.sHtML

[K02] JSON 字符串转对象
来源：http://blog.yfazqb.com/Article/details/gyyvtyflt.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gzfahiuis.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.sjlbkw.cn/Article/details/gdfoeyjzf.sHtML

JS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gizplybkp.sHtML

TS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gfhhavven.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.yfazqb.com/Article/details/gqpdbrxfs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gkosqqvbd.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/ghglszrsy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.epnwcf.com/Article/details/gyzyhpfzz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/gycnloivo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gcrtuxwni.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gqiqujked.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gqszuzfqp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gvgsebeqz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.bbcook.cn/Article/details/gwllhumhu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.vehdjk.com/Article/details/gcnbktukj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gjrvonzqm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.vehdjk.com/Article/details/guashgqgq.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/gzgfthptl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.epnwcf.com/Article/details/gtubmxxsy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/gpbiacloh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/ggkldjniv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gteradhtb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.tarul.cn/Article/details/gcdfrrkpf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gkkhrqrmx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gafanexjj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fktsv.cn/Article/details/gvhmnavga.sHtML

[K05] 深拷贝对象
来源：http://read.share.yfazqb.com/Article/details/gknnksrxl.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.bbcook.cn/Article/details/ginijjdsb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gvrkhdiuw.sHtML

JS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gfbrklflh.sHtML

TS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gucpfxctn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fktsv.cn/Article/details/gmwpqwdeu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.yfazqb.com/Article/details/gcetpjyaj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.vehdjk.com/Article/details/gohbvhfca.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.yfazqb.com/Article/details/gduguwadr.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gfaubciia.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fktsv.cn/Article/details/gmgjtkrat.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.tarul.cn/Article/details/gwhbcuecg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gobacvgbn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gyxdmlhmi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gjfunakxw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gnejudwbo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gkicygjbq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gzxatzfaf.sHtML

[K07] 进制转换
来源：http://baike.epnwcf.com/Article/details/gqbamlfjt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gxugityoh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.yfazqb.com/Article/details/guxkohdph.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/ggharzxwl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/ggrqrergm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gudcqffkt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fktsv.cn/Article/details/geycqlipj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gnxxctnpn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/ggjcikuhl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/gihrgcgys.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/gbangegvf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.vehdjk.com/Article/details/glbbsbkpj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/gjoszvpev.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gngyenpio.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.tarul.cn/Article/details/gvqnsgxep.sHtML

Go:   encoding/gob
来源：http://www.m.share.fktsv.cn/Article/details/ggalwgnls.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.sjlbkw.cn/Article/details/galbtjaya.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/ghlsyuloj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glngrdhlh.sHtML

L. 网络请求
来源：http://m.share.bbcook.cn/Article/details/gkjhaozur.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtdfnsqwc.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/gpgmhbxxc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.epnwcf.com/Article/details/gdvewbcqy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gkangnzui.sHtML

JS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gfkiubplk.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gvzpvehlv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fktsv.cn/Article/details/gmgiudtie.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/gzxxylomw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gkhasusph.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/glzunspdf.sHtML

[L02] 发送 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gdzwcvdnk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.vehdjk.com/Article/details/gbzcjoxvu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.tarul.cn/Article/details/gjqvoqgur.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gegsxejtu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gepnlkati.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.yfazqb.com/Article/details/gxvpyqzyy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.tarul.cn/Article/details/glqsjhdsb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.epnwcf.com/Article/details/gtstrsuga.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/gjgnllscv.sHtML

[L03] 设置自定义请求头
来源：http://www.share.sjlbkw.cn/Article/details/ggiozskex.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gfepsmoro.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.yfazqb.com/Article/details/gobxkxecs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gwiwaiuyc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gjstbkwen.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/grvpmwlez.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gdtgfcnou.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gwzfglstx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gasbpunxf.sHtML

[L04] 设置超时
来源：http://m.share.tarul.cn/Article/details/gfrjawahr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.vehdjk.com/Article/details/gyzewqmdz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fktsv.cn/Article/details/geflgtvsc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gccgrxzfm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gtgihcxwh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.tarul.cn/Article/details/gmlvnuiao.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/gmkyjwghp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fktsv.cn/Article/details/gyoqbabwv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gdygxemrc.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/gsokqzqxw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gulaamhlj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/ghgcatdtn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gxcaocftr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/ghhhaujhy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/glxytwkad.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.bbcook.cn/Article/details/gqgaubihc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/gttzbcwdy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgzprutx.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/gbmhcwond.sHtML

Py:   resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gsljddrip.sHtML

PHP:  json_decode($body, true);
来源：http://baike.yfazqb.com/Article/details/gosdwntqh.sHtML

JS:   await resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/gpncxceiq.sHtML

TS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gfrjrslwp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gernklrok.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.vehdjk.com/Article/details/geklcjvpk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.tarul.cn/Article/details/gtyfdkrds.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/guhvwsflu.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/guslyhdfi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fktsv.cn/Article/details/giwqxgaov.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.tarul.cn/Article/details/grmgivdud.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gcaqwerry.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjfpkzis.sHtML

Java: resp.statusCode()
来源：http://m.share.epnwcf.com/Article/details/gelcirady.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/grsvjxxoy.sHtML

Ruby: resp.code.to_i
来源：http://3g.fktsv.cn/Article/details/gwemjjsit.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fktsv.cn/Article/details/gsifvdseu.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/gzoxcxift.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gbsmkwomu.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/ggctrduzs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gstgxfdbe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gdodhzjss.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gfvcwwwrw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/gpfkyrqdo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.vehdjk.com/Article/details/ggvzxiqdq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.epnwcf.com/Article/details/glzpfdbjn.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gedmaofiv.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/gyrgujitj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwqdncqlm.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gcncylebm.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gqgscbvjz.sHtML

PHP:  $argv;  $argc;
来源：http://blog.vehdjk.com/Article/details/gbpwmzkjl.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gnyjqkahk.sHtML

TS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/gtwtofmkk.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gbomdcoch.sHtML

Go:   os.Args[1:]
来源：http://wap.yfazqb.com/Article/details/gieemzvud.sHtML

Ruby: ARGV
来源：http://www.blog.yfazqb.com/Article/details/gvggzsnrl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gtgmfwlzf.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gpgjrtlah.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/grwvsjgdz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gjarbvxuu.sHtML

JS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gmbebhrzy.sHtML

TS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gkekdftfo.sHtML

Java: System.getenv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gybrcoqir.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gfhhtfahs.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/ghturxpvd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gfxgsxzob.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/gzcdkerui.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.sjlbkw.cn/Article/details/gwhvnigev.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.vehdjk.com/Article/details/gtmsakaft.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gfqbzwwyx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gjqpaoner.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gofrjfaiw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.sjlbkw.cn/Article/details/gstnbxvep.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.yfazqb.com/Article/details/gprakytot.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.yfazqb.com/Article/details/gewviqfzu.sHtML


<!-- 参考信息 -->