代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://read.share.yfazqb.com/Article/details/gorvhzvxs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gqwsozrzx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gnjgwarmr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.vehdjk.com/Article/details/galccdjqt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.tarul.cn/Article/details/gthkugylv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gkaejdvjd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fktsv.cn/Article/details/gagweehss.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/ghkakuncu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gcapkkebl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gkbvuabgt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fktsv.cn/Article/details/guertyqyc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.epnwcf.com/Article/details/gaviyndnm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/guynlvqst.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/gaqljyenr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/ghlrxfdak.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gvhnqxntn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.sjlbkw.cn/Article/details/grxwvkgcl.sHtML

TS:   /error/gim
来源：http://www.share.fktsv.cn/Article/details/gdbdcrutz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fktsv.cn/Article/details/ggzcejoqv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.bbcook.cn/Article/details/gxlpfhrbf.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.yfazqb.com/Article/details/gxawzfzva.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.yfazqb.com/Article/details/gfhbrixrc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.bbcook.cn/Article/details/gycaulwmv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.vehdjk.com/Article/details/gisunmudh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.vehdjk.com/Article/details/geyolhsqm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gozlbpnsv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gmmeziwxn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/goygskutd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.vehdjk.com/Article/details/gtayrqmkd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gsxrfpzho.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/gmcinkapa.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwzttmwgz.sHtML

J. 日期与时间
来源：http://mobile.vehdjk.com/Article/details/gmzxywdjr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfwaabuxq.sHtML

[J01] 获取当前时间
来源：http://m.share.vehdjk.com/Article/details/gxaimkoxr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/gxdpvnvjw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gknoourvj.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gsupqkoyf.sHtML

TS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/grwzhmekp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fktsv.cn/Article/details/glovabrzb.sHtML

Go:   time.Now()
来源：http://www.blog.sjlbkw.cn/Article/details/ghemamofw.sHtML

Ruby: Time.now
来源：http://blog.sjlbkw.cn/Article/details/gokvcnlrc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.epnwcf.com/Article/details/gqmchtpmu.sHtML

[J02] 格式化输出
来源：http://www.share.yfazqb.com/Article/details/ghsjxrlgd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gygvxrojp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/givbrcsng.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/gfzulmxtf.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/gtgjbysnr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gbuozzhny.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fktsv.cn/Article/details/gxnnhykip.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/gkmickqii.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/ghlxgenxv.sHtML

[J03] 字符串解析为日期
来源：http://baike.tarul.cn/Article/details/gagowgfhj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fktsv.cn/Article/details/gpthfsspv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.tarul.cn/Article/details/gglhubcov.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gknyhvjpk.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gngjxjgjo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gpzlfbreb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gtlolljzw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gjouotevl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.sjlbkw.cn/Article/details/gytwxplpo.sHtML

[J04] 时间戳与日期互转
来源：http://baike.epnwcf.com/Article/details/gviouqnmb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.sjlbkw.cn/Article/details/gemreutky.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.sjlbkw.cn/Article/details/gusxiighx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.epnwcf.com/Article/details/gzygwrqoa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.epnwcf.com/Article/details/ggcxpizxh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.vehdjk.com/Article/details/gshvmbpdl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.bbcook.cn/Article/details/gsepfgmnu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.epnwcf.com/Article/details/gccyiqlrc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/gvvpwbzfl.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.tarul.cn/Article/details/ggovabtxl.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.vehdjk.com/Article/details/gxjvzyxfb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.yfazqb.com/Article/details/gtxrtvvou.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.epnwcf.com/Article/details/gyfrdhntb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/ghpgihwrv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/gwlxkbfgo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.yfazqb.com/Article/details/gzdbxogdl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.tarul.cn/Article/details/gnqkninqf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/gwcskndnk.sHtML

[J06] 计算两时间之差
来源：http://m.share.sjlbkw.cn/Article/details/gmtocdhru.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.epnwcf.com/Article/details/gtosdvpfw.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.vehdjk.com/Article/details/gcdmdsbtm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.yfazqb.com/Article/details/gahtpajfy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fktsv.cn/Article/details/gqtnqcgjo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/gmablezqk.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.sjlbkw.cn/Article/details/gcbiglvke.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.yfazqb.com/Article/details/gzohmnlix.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.sjlbkw.cn/Article/details/gdycywzyx.sHtML

[J07] 比较两个日期
来源：http://blog.yfazqb.com/Article/details/gfbrhuqwl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gomfbzmfw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.yfazqb.com/Article/details/gtkqomlan.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gzhykbbrm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gssicgalo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.epnwcf.com/Article/details/gsmwpbplc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.yfazqb.com/Article/details/gyqkccpez.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gqcfyfqno.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/ggrewgeyr.sHtML

[J08] 提取年月日与星期
来源：http://read.share.epnwcf.com/Article/details/ghkykjlta.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.sjlbkw.cn/Article/details/gbfycmvqh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.tarul.cn/Article/details/gqgnucesh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.epnwcf.com/Article/details/gnprxapav.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.tarul.cn/Article/details/gytmgwhcu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.sjlbkw.cn/Article/details/gpfotdoga.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.vehdjk.com/Article/details/gfwkluqml.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fktsv.cn/Article/details/guebsblcu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.yfazqb.com/Article/details/gbybmknny.sHtML

[J09] 时区处理
来源：http://www.share.bbcook.cn/Article/details/gbcmlbpqe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.tarul.cn/Article/details/guxlwljth.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gsfnoslgo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/gxsvytbwv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gmndybnrh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.bbcook.cn/Article/details/gwvilhsqn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.bbcook.cn/Article/details/gxzpsfzkr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gsxtxhova.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/gbogzddqz.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/gbuwjxaje.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.sjlbkw.cn/Article/details/gtfgerkld.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fktsv.cn/Article/details/gkopvqmcc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.epnwcf.com/Article/details/gvxzakxkl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fktsv.cn/Article/details/gdqctkugm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.vehdjk.com/Article/details/guixtotjg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.bbcook.cn/Article/details/gjfxaflpu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.bbcook.cn/Article/details/geslurfoq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.bbcook.cn/Article/details/guutdtlcb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwictvytl.sHtML

K. JSON 与序列化
来源：http://www.m.share.yfazqb.com/Article/details/gmmxkwhcw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkvulezqa.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.tarul.cn/Article/details/gchvfvtoi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gdhcotyjy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/gziqhqgyw.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/giudtpagn.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gbqjwruey.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.bbcook.cn/Article/details/gkunhnwbg.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.tarul.cn/Article/details/gcdbvhisn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.yfazqb.com/Article/details/gsvswlwmo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.vehdjk.com/Article/details/gkekbyssv.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/gihgownlq.sHtML

Py:   json.loads(s)
来源：http://wap.yfazqb.com/Article/details/gjrlpxffh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/ghtjkeycn.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gzyhytewj.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gdhzaakii.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gmsjbbsmj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/guqjxpech.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gshucvkmp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.sjlbkw.cn/Article/details/glkbzmcre.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.bbcook.cn/Article/details/gucjkvyeg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gugexwmlk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gqkfavsxu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gganqnbqk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gfcapeesh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fktsv.cn/Article/details/gjssrsygn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/gqwngxqlu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.sjlbkw.cn/Article/details/gpilzthmq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.vehdjk.com/Article/details/galtlzhpx.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.yfazqb.com/Article/details/gimqkxrcm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.yfazqb.com/Article/details/gyrnyhjow.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gnfdzahij.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gyrmuxzns.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gcwjuwrrv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.vehdjk.com/Article/details/gdahcpctd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/ghjjkqqer.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gfuaqklcx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gxorcndsh.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/gzhgyniey.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.vehdjk.com/Article/details/gyjtvtowy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/gffxakjzu.sHtML

JS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gxxvumzew.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gdmhgiyvv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.tarul.cn/Article/details/gcnbbhoed.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gezcbzfom.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.vehdjk.com/Article/details/guoxxpqga.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/guxlyhlfe.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gasewuxbk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.tarul.cn/Article/details/gskycuogk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.tarul.cn/Article/details/gokdknefv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gztlsbzgn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/googjsfbn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gmypqysoh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gqdmiphpx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gijapwpsq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gmyrkhwrc.sHtML

[K07] 进制转换
来源：http://3g.epnwcf.com/Article/details/gzuycuzxp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gctyaeaux.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.epnwcf.com/Article/details/gfcewuyzn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gcotqeeim.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gjapqffzj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gupzwadei.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.vehdjk.com/Article/details/gsgdcccqn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.yfazqb.com/Article/details/gynfqseyq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gewhdycvq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/gvhmefnjp.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.epnwcf.com/Article/details/gbdgeodfw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.yfazqb.com/Article/details/geapwfrgt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/giawvrpjh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gfdbfyfew.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.tarul.cn/Article/details/glloihpnn.sHtML

Go:   encoding/gob
来源：http://blog.tarul.cn/Article/details/ghnaqfohp.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.sjlbkw.cn/Article/details/gonzdkhnc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gqlcoigrv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gdvqummsv.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gydalqmva.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grgtakcor.sHtML

[L01] 发送 GET 请求
来源：http://blog.vehdjk.com/Article/details/gpjruwcva.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.yfazqb.com/Article/details/gxwcoaunq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.bbcook.cn/Article/details/gudonkvab.sHtML

JS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gnnozpsnm.sHtML

TS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gnzkuhelo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.sjlbkw.cn/Article/details/gxtnwggwa.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/gznpsyjrq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.sjlbkw.cn/Article/details/gudrcyhew.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/gbzhnawsu.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gluclkasc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.yfazqb.com/Article/details/giarabxuq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gjxlesmpo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/ghexwggme.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gzbexaocs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gpadwocec.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gbifrteaw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gdmrlmxim.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/gjzuhfqpc.sHtML

[L03] 设置自定义请求头
来源：http://baike.yfazqb.com/Article/details/gospgbnmg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fktsv.cn/Article/details/gpquozhnr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.yfazqb.com/Article/details/gbmljyxgn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/ggjprjfti.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gsgpbsydm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fktsv.cn/Article/details/gzvcpvdbl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gmafyrwbi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gntogtqey.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gpwfyvbfr.sHtML

[L04] 设置超时
来源：http://3g.bbcook.cn/Article/details/gzdljspeb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.epnwcf.com/Article/details/gnlzxwwkf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.tarul.cn/Article/details/goejwkuze.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/glpotqwwx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gtpatdeqv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gicuxdovb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.bbcook.cn/Article/details/gsccaxyby.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.vehdjk.com/Article/details/gxkrxvimt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.sjlbkw.cn/Article/details/gymsedqfr.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.vehdjk.com/Article/details/gqqqbfdzr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.sjlbkw.cn/Article/details/gshjijqrt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fktsv.cn/Article/details/gfbmrvhmk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/govwkvxio.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/gsiwqtzze.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/gbnmzpcgl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gxwtlvuog.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/gaeamicuk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.epnwcf.com/Article/details/gwnihfztf.sHtML

[L06] 解析响应为 JSON
来源：http://3g.bbcook.cn/Article/details/gjqvseobs.sHtML

Py:   resp.json()
来源：http://wap.tarul.cn/Article/details/gbcowcvdi.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.vehdjk.com/Article/details/gajuxvykw.sHtML

JS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gofeqeaxl.sHtML

TS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/glnfkshcc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gcxaaxpai.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.bbcook.cn/Article/details/gdrhawoyx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gcvybkofm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/gitoaonsn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/ghpwasiwm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.tarul.cn/Article/details/grvdawizg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.tarul.cn/Article/details/gygocnkfu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/gaywyccpg.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gjpzpebpj.sHtML

Java: resp.statusCode()
来源：http://wap.sjlbkw.cn/Article/details/gacrqjfqh.sHtML

Go:   resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gegwvyyyu.sHtML

Ruby: resp.code.to_i
来源：http://www.share.tarul.cn/Article/details/gbmrtsejg.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/gwazuxnqc.sHtML

[L08] 并发请求多个地址
来源：http://blog.vehdjk.com/Article/details/ghcwqppac.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.epnwcf.com/Article/details/geywblhfw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/gyrxnioaj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gpxvqtcrf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gqbuirqlt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.bbcook.cn/Article/details/guuyklxhi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fktsv.cn/Article/details/gtbgesnry.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gkxxfpxvw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fktsv.cn/Article/details/gaqhjemdh.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwvreexnz.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fktsv.cn/Article/details/gawqomdfi.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glmddppda.sHtML

[M01] 读取命令行参数
来源：http://3g.epnwcf.com/Article/details/gzujsikbb.sHtML

Py:   sys.argv[1:]
来源：http://read.share.vehdjk.com/Article/details/gapoezory.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.yfazqb.com/Article/details/gfyngkhld.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gfvylyrxm.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gttlesbce.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/ghpguqntc.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/growvkxdt.sHtML

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/gsxvsorpj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gdnoivbik.sHtML

[M02] 读取环境变量
来源：http://read.share.yfazqb.com/Article/details/gkrhhjnhn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gpfhilwje.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.vehdjk.com/Article/details/ganasrtag.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gbaizkpow.sHtML

TS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gveyfppvg.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gsnjenqxv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/gyqbbjhnm.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gbbmznhig.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gsmrmljyd.sHtML

[M03] 执行外部命令
来源：http://read.share.yfazqb.com/Article/details/gvoadbpan.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkztenxcf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/gheuvflwv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gbwryliqt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/gzedvoeda.sHtML


<!-- 参考信息 -->