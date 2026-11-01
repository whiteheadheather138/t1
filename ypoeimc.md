代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.epnwcf.com/Article/details/gyymyfdhw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.tarul.cn/Article/details/guowwbhhu.sHtML

[I04] 正则替换
来源：http://www.blog.vehdjk.com/Article/details/gmlqgensc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.vehdjk.com/Article/details/gejvoewsk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gmokvosgy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwaipzofl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gohatkbpd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gsacpirxs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fktsv.cn/Article/details/grecperel.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.tarul.cn/Article/details/gdwnftbiz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/glndektsh.sHtML

[I05] 按正则拆分
来源：http://read.share.vehdjk.com/Article/details/gcjhbrpro.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.bbcook.cn/Article/details/gtulhzshy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gkmzfbmul.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gyfinlvwy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gdxkpvxue.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.vehdjk.com/Article/details/grbatbqym.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fktsv.cn/Article/details/glxamqnnh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gwhwvehwl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.epnwcf.com/Article/details/gdoasotkf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/gsqugpgqv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gapprefrr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/gymdgdgio.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/geixbwing.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.epnwcf.com/Article/details/gmvztplnb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/glqbhfkmr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.sjlbkw.cn/Article/details/ggdzfnbtk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gkxueofvd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gffwbcwmg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fktsv.cn/Article/details/ghhcwhcvc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.vehdjk.com/Article/details/gvfhnnzkn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/gxfnlnxqn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gbshvqfsf.sHtML

TS:   /error/gim
来源：http://baike.bbcook.cn/Article/details/glazuropx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.vehdjk.com/Article/details/gaakvfprx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.yfazqb.com/Article/details/gjiunewih.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.vehdjk.com/Article/details/gzsoutiwk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fktsv.cn/Article/details/gtgzoudms.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/gjlvvissx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.vehdjk.com/Article/details/gvfjukmdi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.tarul.cn/Article/details/gyynknlcy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gtbdqziga.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gxumanlka.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gacwchymb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fktsv.cn/Article/details/gnoysfwsl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fktsv.cn/Article/details/geejhexxr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gewlfwtbj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkabgjnmf.sHtML

J. 日期与时间
来源：http://wap.fktsv.cn/Article/details/guhfvokrs.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gnggkaesl.sHtML

[J01] 获取当前时间
来源：http://wap.epnwcf.com/Article/details/gtsizerev.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.epnwcf.com/Article/details/gtimlrsmy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gdzpqscza.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/goieckrzk.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gtrxnwcgg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.bbcook.cn/Article/details/ggxsdikpi.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/gskbjiwtz.sHtML

Ruby: Time.now
来源：http://www.blog.epnwcf.com/Article/details/gbeuglqte.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.yfazqb.com/Article/details/gwpjydsdy.sHtML

[J02] 格式化输出
来源：http://www.share.fktsv.cn/Article/details/gqodspmdt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.yfazqb.com/Article/details/gaoqktboj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gujglicvm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.sjlbkw.cn/Article/details/gggeshelk.sHtML

TS:   d.toISOString()
来源：http://www.share.sjlbkw.cn/Article/details/giywwmski.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.epnwcf.com/Article/details/gcyqelbhz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/gqiiajaus.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gakfsfusl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.bbcook.cn/Article/details/gnsvjppuj.sHtML

[J03] 字符串解析为日期
来源：http://wap.tarul.cn/Article/details/giaqvwbev.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/ggnulgxvf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.tarul.cn/Article/details/gwjjqtihw.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/ggkzlchby.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gkbqcqnkm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gjgcbzxdj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gspapnlpu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gvazoedvo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.sjlbkw.cn/Article/details/gybrzxmxa.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fktsv.cn/Article/details/ggiwbjyti.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fktsv.cn/Article/details/gdsrwmldm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/glmzywcxo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.epnwcf.com/Article/details/ggxgdhnxt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gboqppesi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.vehdjk.com/Article/details/gpaxnxqhk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.tarul.cn/Article/details/gneeppopq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/gqfelknbw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/gpcewzdic.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.yfazqb.com/Article/details/gpyxqgreq.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.vehdjk.com/Article/details/gdzpxfvel.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.vehdjk.com/Article/details/goodniasu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/guxvjqejg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/geexoetjk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fktsv.cn/Article/details/gbxaibmgr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.sjlbkw.cn/Article/details/gsrvizqux.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.vehdjk.com/Article/details/gqklrenzw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.vehdjk.com/Article/details/gpfsayzzv.sHtML

[J06] 计算两时间之差
来源：http://3g.yfazqb.com/Article/details/gyrpjrvfn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fktsv.cn/Article/details/ghwkemwmx.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.tarul.cn/Article/details/gpefqqdmf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.sjlbkw.cn/Article/details/grlrljatu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.vehdjk.com/Article/details/gfvguihrx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fktsv.cn/Article/details/gcalmtqzf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.tarul.cn/Article/details/gepdtvbdy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.bbcook.cn/Article/details/ggtzebbwc.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.epnwcf.com/Article/details/gsicytkkv.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fktsv.cn/Article/details/gmlgcushu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gsmrvrmta.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fktsv.cn/Article/details/gikkcczwc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/giqlxklwy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gwugfqkeg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.tarul.cn/Article/details/giwqzxxah.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fktsv.cn/Article/details/gqegfwlxa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gyvwlpddi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gzahkpnbm.sHtML

[J08] 提取年月日与星期
来源：http://mobile.bbcook.cn/Article/details/ghkugdqvl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.vehdjk.com/Article/details/gbzrvdgbn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.yfazqb.com/Article/details/goqbnxejq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.epnwcf.com/Article/details/gmoraclqv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.sjlbkw.cn/Article/details/gabhtgdis.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.epnwcf.com/Article/details/gszqjtqvm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.bbcook.cn/Article/details/gfgxhzgsl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fktsv.cn/Article/details/gwhjznyoo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.sjlbkw.cn/Article/details/ghxgjqmhd.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/ggmddrazk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.tarul.cn/Article/details/gyoyvkgqe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gbjdgajgh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/grgmdmyqn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/gwklwtdst.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.bbcook.cn/Article/details/gtpezflyr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.epnwcf.com/Article/details/gqolfouqb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.epnwcf.com/Article/details/ghowesyyu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/gdwyypwuu.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.yfazqb.com/Article/details/giwsyejkr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.tarul.cn/Article/details/gxqgjcddw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gysrowrop.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gukjvfqzc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.epnwcf.com/Article/details/gyjsskhht.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gqvevuzuw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.tarul.cn/Article/details/gkiozspgb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.sjlbkw.cn/Article/details/graigztie.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.yfazqb.com/Article/details/gzowgptxd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gnzzpbafe.sHtML

K. JSON 与序列化
来源：http://read.share.epnwcf.com/Article/details/gjjdekasv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gdflpuifh.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.epnwcf.com/Article/details/gcfjaykpa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gjsbfeaje.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gtjqfqjnl.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gmlqjpcdi.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gutfzabdg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.sjlbkw.cn/Article/details/gwdozompe.sHtML

Go:   json.Marshal(obj)
来源：http://blog.yfazqb.com/Article/details/gfhyciuwz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.yfazqb.com/Article/details/gxkiuuhtv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.tarul.cn/Article/details/gnqxvqbzu.sHtML

[K02] JSON 字符串转对象
来源：http://blog.bbcook.cn/Article/details/gjmfedpoq.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/gvlmwerwa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gkkdkkzof.sHtML

JS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/giynpvlyh.sHtML

TS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gkssuohqr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.bbcook.cn/Article/details/gakywwlwa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gnusalyqd.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/ggdiwhvyt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.sjlbkw.cn/Article/details/gfcdwavco.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.epnwcf.com/Article/details/gbjebjfdv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gzadftjjg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gbqbrizcm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gtsjjnnsp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gqqjpdubc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.yfazqb.com/Article/details/gumbtpuvo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/gregoaaws.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gzruingfw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.sjlbkw.cn/Article/details/gifbdjcfe.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.epnwcf.com/Article/details/gnnvvuyzt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gccvzsyou.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/grqgrqhns.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gxisxlbkk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gzuaikawm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.epnwcf.com/Article/details/gzxoysybl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/geahcbbnh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gbgbghebz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gkcxfrbab.sHtML

[K05] 深拷贝对象
来源：http://blog.vehdjk.com/Article/details/gyqdjahfp.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fktsv.cn/Article/details/gbbcuripg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fktsv.cn/Article/details/gybwpzvho.sHtML

JS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gizlxsxcp.sHtML

TS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gyowffynz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.vehdjk.com/Article/details/gbvjmwcuu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/gbyanorll.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.epnwcf.com/Article/details/glxbvzrfa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.bbcook.cn/Article/details/gjzvprnrl.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/gvnopybpa.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gsbxcmlor.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.epnwcf.com/Article/details/glduvrjev.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gobczncwm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/ggidrkhjv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.bbcook.cn/Article/details/gubexothp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gqclrbcpr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gzleevxhu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gysdhcoqz.sHtML

[K07] 进制转换
来源：http://mobile.tarul.cn/Article/details/gobipqmxq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.yfazqb.com/Article/details/grfczedkh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.vehdjk.com/Article/details/gzogixovp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gzdrvapaf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gzaplmfws.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gjpqvqubb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.bbcook.cn/Article/details/gpgughhtm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gowwjpojw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gxndpmztu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.yfazqb.com/Article/details/gkhkrdmbw.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/ghqzjfwsj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/glvclfpbn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gjpiponrm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/gyrozqkfi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqsajrkh.sHtML

Go:   encoding/gob
来源：http://www.m.share.fktsv.cn/Article/details/gvonclwsn.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/gqrrmvxxe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gjrhcunrw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmmvesefv.sHtML

L. 网络请求
来源：http://baike.bbcook.cn/Article/details/gbhzqkcbe.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gluoeewxu.sHtML

[L01] 发送 GET 请求
来源：http://baike.bbcook.cn/Article/details/gqsjgzrbz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.tarul.cn/Article/details/gczcsweoj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.tarul.cn/Article/details/gmcfpwlsf.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/geqxkrrhc.sHtML

TS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/gicjkdrda.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.vehdjk.com/Article/details/gzrsqkcjz.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.bbcook.cn/Article/details/glkjnbcap.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.bbcook.cn/Article/details/ghgqfvwji.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/gwvwkvpko.sHtML

[L02] 发送 POST JSON
来源：http://wap.fktsv.cn/Article/details/gwatcycez.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gorevunzb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.tarul.cn/Article/details/ggsfkrxcy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gpbwwibmf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/ggvrierbr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/ggmshdpnx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gfyzjgmug.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.vehdjk.com/Article/details/gmtxbudcq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fktsv.cn/Article/details/gxjoetwlv.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/grdpjdkss.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.yfazqb.com/Article/details/gwvpxqneh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.bbcook.cn/Article/details/golumprqd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gzffsqenx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/gklvuwshq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.vehdjk.com/Article/details/gkyjbgaok.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gauggxviv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gslxddcqb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/glfcjbptz.sHtML

[L04] 设置超时
来源：http://m.share.yfazqb.com/Article/details/gecqncfvp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/gmopredfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/gijdwjdcf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gumiobpar.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/guduysarj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.tarul.cn/Article/details/gkhzqwoob.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.bbcook.cn/Article/details/gigbiblyh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.vehdjk.com/Article/details/ghgrccuyd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.sjlbkw.cn/Article/details/ggwnvfspp.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.yfazqb.com/Article/details/gbpqizgqx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.bbcook.cn/Article/details/gtsnyvwhy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.bbcook.cn/Article/details/gljjqmyjh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gmtoyfanc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gpidstagc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.epnwcf.com/Article/details/gjgzafypv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.bbcook.cn/Article/details/gjgpjokvz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/gncqbiwhh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.vehdjk.com/Article/details/gvdnbadeq.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/gbtyzucdo.sHtML

Py:   resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gyjmnrknh.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.bbcook.cn/Article/details/gxhuieovr.sHtML

JS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gnuofcvic.sHtML

TS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gosrqbuyq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/gecergnvx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.epnwcf.com/Article/details/gswihtlal.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.epnwcf.com/Article/details/glurxzask.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gpwdyilmg.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gbpfgswds.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.epnwcf.com/Article/details/gkcjyaqsh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.yfazqb.com/Article/details/gepvcunge.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gcgcojead.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/glablngod.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/ggunycdym.sHtML

Go:   resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/gihrclbey.sHtML

Ruby: resp.code.to_i
来源：http://read.share.bbcook.cn/Article/details/gytghgubi.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/ghxftszbv.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/ggtmenkdu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.tarul.cn/Article/details/ghjxjwkgg.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/gjfusxqau.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsmddiru.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gzvfbsbjz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fktsv.cn/Article/details/gbrsrsdol.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.tarul.cn/Article/details/gcgonjmca.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.tarul.cn/Article/details/gganihooq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.yfazqb.com/Article/details/gwfbzivgl.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpklosiqp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.tarul.cn/Article/details/gsexcvysk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxswxdovk.sHtML

[M01] 读取命令行参数
来源：http://wap.fktsv.cn/Article/details/gbcjesvki.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gdjswmwzh.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/ggyjzziff.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/grutbwinu.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gwdghjgya.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.vehdjk.com/Article/details/geikhubiz.sHtML

Go:   os.Args[1:]
来源：http://www.blog.yfazqb.com/Article/details/guecaxcsw.sHtML


<!-- 参考信息 -->