代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.epnwcf.com/Article/details/gsolxmiap.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.vehdjk.com/Article/details/gdsdfyysl.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/gqqbeossi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fktsv.cn/Article/details/ggatkibsh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gmkcuxewr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/goodzkkns.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/ggkpejhif.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/gqunidonm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/gdcnyqghu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.epnwcf.com/Article/details/gylzgakba.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gzlrgqwhz.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/grzzosrkl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.epnwcf.com/Article/details/gsdgkrbrf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/geitcarxz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gnhjeyljp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gsubncyjl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/gpnrfoetc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gshbjpgrq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/ghwrxaahv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.sjlbkw.cn/Article/details/ghhzwoeyi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/gigtgkbyt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/glzksevjt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.bbcook.cn/Article/details/gfebaespk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gdymmovve.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/gisffbhce.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.vehdjk.com/Article/details/glqvroaah.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.vehdjk.com/Article/details/gwnqszvdi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fktsv.cn/Article/details/greoadhba.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gfluziury.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.epnwcf.com/Article/details/gbrzbling.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.sjlbkw.cn/Article/details/gvhyqrdqa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gefktpgja.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.bbcook.cn/Article/details/gtnoigbve.sHtML

TS:   /error/gim
来源：http://mobile.tarul.cn/Article/details/gfsrubfdj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.bbcook.cn/Article/details/gfqtljsvf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.sjlbkw.cn/Article/details/gibftjfvz.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fktsv.cn/Article/details/gddjlokdh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.tarul.cn/Article/details/giljkpbys.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gftvppbgx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.tarul.cn/Article/details/gdxtbtmjn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gahqdjbyv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gjgzrpkdn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gsgakhbsn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gjohttaap.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.bbcook.cn/Article/details/gyxtqqxot.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.tarul.cn/Article/details/gjzaaxbdh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gobmthrxr.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/glhrivxxp.sHtML

J. 日期与时间
来源：http://www.m.share.epnwcf.com/Article/details/gvthedpms.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gylacybqf.sHtML

[J01] 获取当前时间
来源：http://www.share.epnwcf.com/Article/details/gsrthzfzo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fktsv.cn/Article/details/gsjdlywmo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.tarul.cn/Article/details/ghmzswdqr.sHtML

JS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/giqthsjzq.sHtML

TS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gcltvkkrk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fktsv.cn/Article/details/gwlmapttv.sHtML

Go:   time.Now()
来源：http://m.share.vehdjk.com/Article/details/ggrlccqci.sHtML

Ruby: Time.now
来源：http://www.share.vehdjk.com/Article/details/gsnvkkvpt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.tarul.cn/Article/details/gwkyyvmqx.sHtML

[J02] 格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gnmwziqzl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/goqhrtive.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gapgwhfgu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/gniaowfbv.sHtML

TS:   d.toISOString()
来源：http://read.share.vehdjk.com/Article/details/gyioofpje.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.sjlbkw.cn/Article/details/gkppdmbtc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.epnwcf.com/Article/details/giwcuhmld.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gokrwecol.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/gdxoidrsd.sHtML

[J03] 字符串解析为日期
来源：http://blog.tarul.cn/Article/details/gvpmxyefo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/gkivgdqpr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.bbcook.cn/Article/details/gkgjhufoa.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/grusvhlli.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/godkbvsir.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gbcdwfkcm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gaashsjtc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gholhpxsi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.epnwcf.com/Article/details/gjmklbhuo.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/gwffnbzdz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.tarul.cn/Article/details/gngjfgzmr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.yfazqb.com/Article/details/gjlshxwzc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.vehdjk.com/Article/details/gtmdzwwuq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gtfjjpool.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.tarul.cn/Article/details/geuzcfkvx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.tarul.cn/Article/details/gsmyzhvgj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gvwyftvmk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.bbcook.cn/Article/details/ghmwzrhga.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.bbcook.cn/Article/details/gcnrhowff.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.vehdjk.com/Article/details/gidgzgedc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.bbcook.cn/Article/details/ghvguyuhn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/grvnrysrv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/gbvwvdgca.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.epnwcf.com/Article/details/gunamvoqr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.sjlbkw.cn/Article/details/gmwnvemvm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.bbcook.cn/Article/details/gctcvzvok.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gbhutyify.sHtML

[J06] 计算两时间之差
来源：http://www.share.vehdjk.com/Article/details/gbmuqdntg.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fktsv.cn/Article/details/gpfbanowk.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gtqybfnyd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.sjlbkw.cn/Article/details/gwnnodtfn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.sjlbkw.cn/Article/details/gcmpxqpsl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.bbcook.cn/Article/details/gtrqylzhk.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.epnwcf.com/Article/details/gyxylplun.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhabntaw.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/gxmafjanp.sHtML

[J07] 比较两个日期
来源：http://www.share.yfazqb.com/Article/details/gnvoxjubp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gbkypazbu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/ghqmnjztb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gtpdgvlbe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gabgzjwka.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gyspjrwxh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fktsv.cn/Article/details/gqqbeonxp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/ganiyvjno.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gluiyemtx.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/gsnlulyka.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.bbcook.cn/Article/details/gidodhiwh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.tarul.cn/Article/details/glntgpcuw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fktsv.cn/Article/details/gnmyjaekz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.tarul.cn/Article/details/gqbejqlou.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.epnwcf.com/Article/details/gnhttajiy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.vehdjk.com/Article/details/gemuwyzvh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fktsv.cn/Article/details/gtgjqmuqd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.tarul.cn/Article/details/gcbbrsqpu.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gwvagqrcs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.bbcook.cn/Article/details/gmaxeeqoh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gvplmkxqy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/glgfiyiih.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/glfflvaui.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.epnwcf.com/Article/details/gqsisvgdx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.bbcook.cn/Article/details/gctxldhhp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.yfazqb.com/Article/details/ghgpagwmr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fktsv.cn/Article/details/gyiebstuk.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.epnwcf.com/Article/details/gtiyewwaf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/goozygksd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.epnwcf.com/Article/details/gmggwdwnl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.yfazqb.com/Article/details/ghplvkdiv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gjbhazafh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.epnwcf.com/Article/details/grfzuokvb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.sjlbkw.cn/Article/details/gazqxdhgf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.bbcook.cn/Article/details/gtihqwmys.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.bbcook.cn/Article/details/gncqugzsq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gogeartot.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/gebikmypz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/geoyozzdk.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.bbcook.cn/Article/details/gntefyqxk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gqfvovhdm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gqxzlgtpe.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gqnjktyzl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gsowcnkse.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fktsv.cn/Article/details/gdgonnvrp.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fktsv.cn/Article/details/gejnzaufy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/gzoxutgps.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.sjlbkw.cn/Article/details/gzlqeajxy.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.bbcook.cn/Article/details/grkntnugn.sHtML

Py:   json.loads(s)
来源：http://read.share.vehdjk.com/Article/details/gdeaxxcwd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gzzxfdfrn.sHtML

JS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gbuwsifnn.sHtML

TS:   JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/ggmfqgbqm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.epnwcf.com/Article/details/gpuhoorfi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gaqkxrtvd.sHtML

Ruby: JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gzhxiknjk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gpufjhonp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.epnwcf.com/Article/details/gjhrngybz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gznxtoenk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gxtdyuccm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gwlgedhae.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gdhvsjyqx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.bbcook.cn/Article/details/ghqagdrms.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gyksdywsv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.vehdjk.com/Article/details/grwbxitwv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.tarul.cn/Article/details/gqvdfgwzr.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.yfazqb.com/Article/details/ghhwkgsyw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fktsv.cn/Article/details/gmsayfjgv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fktsv.cn/Article/details/gltjlxqla.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/ghqrvspzf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gddmftyoi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gwfqcuodv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gdvuvaieq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/gsuetfygg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fktsv.cn/Article/details/gdbzneszq.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gkfchipui.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/goaonkfnn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fktsv.cn/Article/details/gbtmrhdjt.sHtML

JS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/ggbtvxefj.sHtML

TS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gbxqjchcx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/ggqlzswlp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gleyntmuu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/gfknraffo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.bbcook.cn/Article/details/gtwasmwhr.sHtML

[K06] 解析 URL 查询串
来源：http://wap.epnwcf.com/Article/details/gxtyeazoi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gkwpwqtad.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fktsv.cn/Article/details/gapffflii.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gnlsskqec.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/glsdfqqsv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.tarul.cn/Article/details/gqdpedons.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gkzheoqnr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gntahfnou.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gwvrsuhpz.sHtML

[K07] 进制转换
来源：http://www.blog.vehdjk.com/Article/details/gdnztedbz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gukvddaih.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fktsv.cn/Article/details/gnptjczwy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/ghoosqjzb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/girlbdvni.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gvobphhhn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.epnwcf.com/Article/details/gaeevpexk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fktsv.cn/Article/details/gtnxnhfzc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gjdfzoqjc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/grqwnhkak.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.vehdjk.com/Article/details/giznbqcwp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.yfazqb.com/Article/details/goxquippf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/geoibqbnr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gitrfsfyu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/gexbxnbfa.sHtML

Go:   encoding/gob
来源：http://blog.bbcook.cn/Article/details/gszeugare.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.yfazqb.com/Article/details/gkzrbkkuc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gqqlyvzco.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/grfsuowsv.sHtML

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/gcuchoqzl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gnotvpdwa.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/gnmaybxui.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gawicuixv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/gmhvuikal.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gnwexmetj.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gpwkjtvzi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.tarul.cn/Article/details/gzlehxjnr.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.yfazqb.com/Article/details/ghlnmnhda.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.tarul.cn/Article/details/gocotnwuo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.tarul.cn/Article/details/gawkzybar.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/glpbxdsxz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gruzjhuhz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.vehdjk.com/Article/details/gplbzqytp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/ghwssnyem.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gkqjfrpeb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gkoxhmnzr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.yfazqb.com/Article/details/graxiajck.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.bbcook.cn/Article/details/gkbqbmfcq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/gwhlmdddc.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.tarul.cn/Article/details/gqcbtzncm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fktsv.cn/Article/details/gzofyhwhl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.yfazqb.com/Article/details/gwshfymco.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/gvtlrljxi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gctxybchj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.vehdjk.com/Article/details/gatlagkge.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gytcpkwpd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.tarul.cn/Article/details/guxfpdcgr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gfqoaxljp.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gzpbdwwfq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/glxlfvmqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/ghrbeligg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gvkqzwwyr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gqbepbijo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gdjhaizzy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gnpfdxtvu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/gslltfsom.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gisyqmutg.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/gfdgwgois.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/gtppnwtop.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.bbcook.cn/Article/details/gnnkolufa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gwqfzobsb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gloroulpk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.tarul.cn/Article/details/gbtxxamhl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.tarul.cn/Article/details/gkrfxhqqq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.bbcook.cn/Article/details/gnuugqbgn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.yfazqb.com/Article/details/gathsevnp.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/gdzqfermy.sHtML

Py:   resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gojzbtsnc.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/gcnoobmvn.sHtML

JS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/ghavcingl.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gkijcxvpl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.tarul.cn/Article/details/glahkbvgn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gjxyhpsgo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gedjukmgc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.tarul.cn/Article/details/gzhcdrxwh.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gypfkcmgo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/gstmotglb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fktsv.cn/Article/details/gkmsqaeqt.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gcqjofvvk.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gtgbplldx.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gcuyvhhbp.sHtML

Go:   resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gkepovhwi.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gpuzobpzf.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gcnnlbawy.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/gxwufjhfr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.bbcook.cn/Article/details/gjrfabfbl.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/gjbbziigc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gqpqrsjal.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gkmmjkvtb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fktsv.cn/Article/details/gsrmtmgch.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gxebchvsc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.yfazqb.com/Article/details/gaummapiq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/gosctzdos.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdnilwikl.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/gbgballus.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnxkgybjy.sHtML

[M01] 读取命令行参数
来源：http://baike.yfazqb.com/Article/details/gzrdqafny.sHtML

Py:   sys.argv[1:]
来源：http://3g.epnwcf.com/Article/details/gttxnjjdo.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.epnwcf.com/Article/details/gnqrzahps.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gvcvwmeqf.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gsvngrtsm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gsztyitti.sHtML

Go:   os.Args[1:]
来源：http://read.share.yfazqb.com/Article/details/gnlozunks.sHtML


<!-- 参考信息 -->