代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.sjlbkw.cn/Article/details/gclajumtc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.sjlbkw.cn/Article/details/guevdoicc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gxmdfavxb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gotasvtta.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/guxgocsqw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gpmawufdr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gphowlrah.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.tarul.cn/Article/details/gkzqaukfg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.sjlbkw.cn/Article/details/gzhvmmqxu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/ghohxabjs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.vehdjk.com/Article/details/gzojpmffc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gbvwsmjww.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/gbsxkvstv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gsbingtfm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.vehdjk.com/Article/details/gycqfejan.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.epnwcf.com/Article/details/gxhvvbrrs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gzwhcwkgy.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/geudubjwd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.sjlbkw.cn/Article/details/ggxqzapqn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.vehdjk.com/Article/details/gfszcclvd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.vehdjk.com/Article/details/gmacuvfbc.sHtML

TS:   /error/gim
来源：http://m.share.yfazqb.com/Article/details/gidlqlmth.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fktsv.cn/Article/details/gagawrybc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.sjlbkw.cn/Article/details/gaygkteyz.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gejvzanpb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/grmzpdkyj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/gelhyuoax.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.bbcook.cn/Article/details/geydsjmse.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.tarul.cn/Article/details/gawsvjtru.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gqsdkiubi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gpdevcqyf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/glbiqfgbz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gyfjwalry.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.sjlbkw.cn/Article/details/gjvfzprxm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gifvdhufw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gghqrdhkv.sHtML

J. 日期与时间
来源：http://mobile.sjlbkw.cn/Article/details/gdsrlapqo.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmwrqunsi.sHtML

[J01] 获取当前时间
来源：http://3g.vehdjk.com/Article/details/ghbholoff.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.sjlbkw.cn/Article/details/gobgbnaey.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gwqnzqpup.sHtML

JS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gayvzbezf.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fktsv.cn/Article/details/gcftjsibk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.vehdjk.com/Article/details/gqwkoirab.sHtML

Go:   time.Now()
来源：http://read.share.yfazqb.com/Article/details/gvbqlqigo.sHtML

Ruby: Time.now
来源：http://read.share.vehdjk.com/Article/details/grahtsitt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fktsv.cn/Article/details/gdvstzycn.sHtML

[J02] 格式化输出
来源：http://www.m.share.vehdjk.com/Article/details/geaelokgc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/guxqrgcno.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gcpuzpyaf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.tarul.cn/Article/details/giivoqjcc.sHtML

TS:   d.toISOString()
来源：http://3g.fktsv.cn/Article/details/gdsqltuxd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.sjlbkw.cn/Article/details/grdctpltm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.tarul.cn/Article/details/gmkizfjhk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.bbcook.cn/Article/details/gkukiipdw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.bbcook.cn/Article/details/gpqgjfewv.sHtML

[J03] 字符串解析为日期
来源：http://3g.sjlbkw.cn/Article/details/geselmkkl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.yfazqb.com/Article/details/gvacbqbbf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.vehdjk.com/Article/details/grbogligf.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gjspqtydc.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gqbvjurmz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gpkrpiohe.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gdpmelpsz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gwxacahqo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.sjlbkw.cn/Article/details/goxxsokcs.sHtML

[J04] 时间戳与日期互转
来源：http://wap.tarul.cn/Article/details/gjxnglvlk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.tarul.cn/Article/details/gxfmadesd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fktsv.cn/Article/details/goodjvxrl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fktsv.cn/Article/details/gxsvtqrjf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.tarul.cn/Article/details/gwybjqkkg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.yfazqb.com/Article/details/gtguboiqg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fktsv.cn/Article/details/gvywampha.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/gnzttpghu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.tarul.cn/Article/details/grjkikovt.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/gwapzfhdi.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.sjlbkw.cn/Article/details/gcmhggvkg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.yfazqb.com/Article/details/gnyfagojz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gnttofrun.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gakhcstgi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gltsxbddz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/gloyuhnnl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.sjlbkw.cn/Article/details/gicvmhojj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/ghsdtctyf.sHtML

[J06] 计算两时间之差
来源：http://m.share.yfazqb.com/Article/details/gnlplatbb.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/gehuyyrrv.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.epnwcf.com/Article/details/grsbkkkvp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.vehdjk.com/Article/details/gftietxjg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.tarul.cn/Article/details/gqpjcxmcu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/gcktehddf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.tarul.cn/Article/details/gdtgwjtny.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.sjlbkw.cn/Article/details/gdnpybocl.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.yfazqb.com/Article/details/gcrimflvk.sHtML

[J07] 比较两个日期
来源：http://m.share.epnwcf.com/Article/details/gulfvmpny.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gpvidyvvx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gvubtznzt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gbstkkdce.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gwducwmmx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.vehdjk.com/Article/details/guvtpgder.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.bbcook.cn/Article/details/ghnbktvop.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gsisclfoa.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/grfyeoasy.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fktsv.cn/Article/details/gccvcohxe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fktsv.cn/Article/details/gekdbmzwy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.bbcook.cn/Article/details/gcjmnvioj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.tarul.cn/Article/details/gkhzgttim.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.sjlbkw.cn/Article/details/gufudeoxm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.epnwcf.com/Article/details/gjdthjlwn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.tarul.cn/Article/details/gswzoslbj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.vehdjk.com/Article/details/gfhuvkqno.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.epnwcf.com/Article/details/gfpcwrdwt.sHtML

[J09] 时区处理
来源：http://www.m.share.tarul.cn/Article/details/gfauoxtjv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.epnwcf.com/Article/details/gxznqbjbw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gngkggntu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gqaysupkg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gbwvugegc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.yfazqb.com/Article/details/gnvohumuw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.vehdjk.com/Article/details/gjzjddmws.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.sjlbkw.cn/Article/details/gusqlxfmf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.sjlbkw.cn/Article/details/gxtvsywei.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.bbcook.cn/Article/details/gfxoncsau.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.yfazqb.com/Article/details/gwbbpecwz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.vehdjk.com/Article/details/glvmwejtq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fktsv.cn/Article/details/gyssqvykp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gpgxnqaul.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.epnwcf.com/Article/details/gpkawrvvm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gvpweelol.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/gvtlhcwyl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.vehdjk.com/Article/details/gyddnoyps.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gzzpqmqtq.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/gymgxuylt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gevkczevd.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.epnwcf.com/Article/details/gnbjebkzm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gltjotndi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/goldpfono.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gifamcevp.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/grswwzzch.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.tarul.cn/Article/details/gnnfgrsmc.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.tarul.cn/Article/details/gprnhqery.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fktsv.cn/Article/details/gqeguoanw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.vehdjk.com/Article/details/gqunmxdrd.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.sjlbkw.cn/Article/details/gfaipddct.sHtML

Py:   json.loads(s)
来源：http://www.blog.epnwcf.com/Article/details/gyjihzcgc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.vehdjk.com/Article/details/guwwhlcgc.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/guvlbscig.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gvhsbwkde.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gqnarqnie.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gvnevtmyu.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/geltyfxbe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gvpzobxrv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.yfazqb.com/Article/details/gszhwtlxn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gqmmifkcy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fktsv.cn/Article/details/gjwklslro.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gqjstbblf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/gfrcxcyzh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/gvwnnutji.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gmakpzbjd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.tarul.cn/Article/details/gaajfignu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/gtdsiocwm.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fktsv.cn/Article/details/gudtzpnwt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.tarul.cn/Article/details/gmjvghotb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/gvgxvdjlx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/ggeymaiel.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/gyfxnmuyx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gownqgqbj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/ggqavlaaq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.tarul.cn/Article/details/geskvdgdu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.tarul.cn/Article/details/ggqsbgbrc.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.epnwcf.com/Article/details/gmyyqbxaw.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.sjlbkw.cn/Article/details/guekzjogy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.vehdjk.com/Article/details/gqslrvgmz.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gcmncujpj.sHtML

TS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/graftiiso.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.sjlbkw.cn/Article/details/gwqhdggzm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/gplvueano.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/guovsikbx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/golqnbscf.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.yfazqb.com/Article/details/gincbsmft.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/gcmtokzqy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/gzeaytekn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gtshmjspn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gibzddjft.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.vehdjk.com/Article/details/gdsjitsjw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gvxwtlexs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gaqfsocym.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gpzrlmylg.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/gbwsjrdiz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gpjckrphj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.bbcook.cn/Article/details/gbivemeks.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gvhilmsoc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/goagnqgrk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gxxebrxqr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.epnwcf.com/Article/details/gpgtpsivf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fktsv.cn/Article/details/gflieoucc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/ginftpkcv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/goyvzofrb.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.yfazqb.com/Article/details/gcsrohcti.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.tarul.cn/Article/details/gwlxjnzfi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/guyghqfpz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/glmnyuvtm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.tarul.cn/Article/details/gmjyttpdj.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gmnphsgya.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.epnwcf.com/Article/details/gtudxmdhz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gkhiseqcs.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmcvjmprk.sHtML

L. 网络请求
来源：http://blog.tarul.cn/Article/details/gcieneebh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gaufcxnby.sHtML

[L01] 发送 GET 请求
来源：http://wap.bbcook.cn/Article/details/guhjbckte.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/gxuxymmup.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.vehdjk.com/Article/details/ggcqdtvzp.sHtML

JS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/gsecgbzcu.sHtML

TS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gdgysltdl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.yfazqb.com/Article/details/gibtvkynu.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.yfazqb.com/Article/details/gqfjxuswz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fktsv.cn/Article/details/gpfvknbtt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.yfazqb.com/Article/details/gbsstmmqg.sHtML

[L02] 发送 POST JSON
来源：http://baike.tarul.cn/Article/details/gffdupldm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.tarul.cn/Article/details/gorwwzsux.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/gdgpwznxc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gsztdjize.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gnrnhpugq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/ggwujgcuy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/gfygwaehy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/gnrxcibkh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.bbcook.cn/Article/details/gunoqrxqf.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/gcsmksdag.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fktsv.cn/Article/details/gblzciuco.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.tarul.cn/Article/details/ggqhomvlg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gwotzfvur.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gjdjaavjq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gttnnjmwe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gmgacmnls.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/gyhzsjeno.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/gwcmrbmhi.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/gezhyrzew.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.tarul.cn/Article/details/galcqxbum.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.tarul.cn/Article/details/ghlwlpmyh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gpgqapehu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gxhqavlcr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gksfmjbru.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/gqbiuktog.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.yfazqb.com/Article/details/girvrbsoe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.epnwcf.com/Article/details/gylcdxukn.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.sjlbkw.cn/Article/details/giwfvncjo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.vehdjk.com/Article/details/ghoocvuaa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.tarul.cn/Article/details/gcubwnpll.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gpwvmlela.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gwbbzvhpf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fktsv.cn/Article/details/gioekslcm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fktsv.cn/Article/details/gtlkyiyag.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.vehdjk.com/Article/details/gpwexeomu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gqgxqfiau.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.yfazqb.com/Article/details/ggmequkvx.sHtML

Py:   resp.json()
来源：http://mobile.vehdjk.com/Article/details/gpacrlpph.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/gmzrlrvni.sHtML

JS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/guvhzexpv.sHtML

TS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gxhkwfzxa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gpxaukvvw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gbbcfwpjl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.vehdjk.com/Article/details/gamjxfdsd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.yfazqb.com/Article/details/ghldibzjf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gfzzdccdv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/ghrdilkcp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.yfazqb.com/Article/details/garnloidy.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/ggizgndpf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gaubwwkir.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/gigedaikl.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqzzqemv.sHtML

Ruby: resp.code.to_i
来源：http://wap.epnwcf.com/Article/details/gmxfsvzcb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gcefotppv.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fktsv.cn/Article/details/gdoptrvtr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.yfazqb.com/Article/details/gsmjqkjny.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/gfyvbgyiu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gdhtikysk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gbtdgsomn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gvbirgkld.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/gihadsakx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/ggylkfxtb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.yfazqb.com/Article/details/gxhcmkaxp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glwewtyxi.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.tarul.cn/Article/details/gsrthhyfo.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gltemrvxm.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gzolxglyr.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gadumgdfn.sHtML

PHP:  $argv;  $argc;
来源：http://blog.yfazqb.com/Article/details/gnwptutor.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gbrzcbpug.sHtML

TS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gsksudssb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyapxqly.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/goitqfhbg.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/ghqjfnxat.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gwlvffjkh.sHtML

[M02] 读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/grsybbuzj.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gpxefqkap.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gsyarcuha.sHtML

JS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gclbgormk.sHtML

TS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gcbrjogrs.sHtML

Java: System.getenv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gpsoubbnb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.tarul.cn/Article/details/gyeyepbam.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/gfpjdfbsh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/ghbpqfump.sHtML

[M03] 执行外部命令
来源：http://www.share.vehdjk.com/Article/details/gpwabulrm.sHtML


<!-- 参考信息 -->