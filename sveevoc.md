代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.bbcook.cn/Article/details/guzkqyojt.sHtML

[I03] 提取捕获分组
来源：http://blog.fktsv.cn/Article/details/gatohrpae.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fktsv.cn/Article/details/gnntltvii.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.bbcook.cn/Article/details/gmprshojb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.tarul.cn/Article/details/gsbpccpfu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/gvbobwbgi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.yfazqb.com/Article/details/gfhfkqkww.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.epnwcf.com/Article/details/gbaibxaqe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/gnfmyvxag.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gdtpxerer.sHtML

[I04] 正则替换
来源：http://www.share.fktsv.cn/Article/details/gofyiwlif.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.sjlbkw.cn/Article/details/gdzfjdrjm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/gmhmhsdgj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gvyrkumad.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gxvnqhdrl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gtbzkkxml.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fktsv.cn/Article/details/gchpymdyg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.yfazqb.com/Article/details/geqgjoqnj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gayqfhmxv.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/gcvuvmuuk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.bbcook.cn/Article/details/gskcqgwsv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gigachqbj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gixrdpzsg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gkhskidsd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.vehdjk.com/Article/details/gupbjyukf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.tarul.cn/Article/details/gcmuibqkc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/goqrecxmj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/goqftriqp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.vehdjk.com/Article/details/gnukvxszs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gctugpnov.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.yfazqb.com/Article/details/gujybpmhs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gokegembk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/goezyrroa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gthfpjoot.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.yfazqb.com/Article/details/gkfymywgb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.epnwcf.com/Article/details/gvtqhacse.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gdlbfvxqx.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.tarul.cn/Article/details/guhngjtgn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.yfazqb.com/Article/details/gtuyzqddt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gbjecrkiw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.sjlbkw.cn/Article/details/gbiokafgs.sHtML

TS:   /error/gim
来源：http://m.share.vehdjk.com/Article/details/gcskvpqaj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.sjlbkw.cn/Article/details/gulqougak.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gfopojvnc.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/gasfvvapu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.vehdjk.com/Article/details/gyuszwnqk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/gnqjdjtim.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.bbcook.cn/Article/details/gjmvaxgem.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gzpvaybmo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/guhdxpmdj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/glezetbmt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gkutttobo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.tarul.cn/Article/details/giccfgzoa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.vehdjk.com/Article/details/gnnzrwink.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmckyurib.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gaicomowo.sHtML

J. 日期与时间
来源：http://wap.tarul.cn/Article/details/gmybmwdif.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gyablwurq.sHtML

[J01] 获取当前时间
来源：http://www.share.bbcook.cn/Article/details/gvaeutygi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.epnwcf.com/Article/details/gmmfnrcqb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gqmqblrai.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gvkufxyzf.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fktsv.cn/Article/details/gqvtphvcs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/gblrnvctg.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/goqprqsot.sHtML

Ruby: Time.now
来源：http://www.m.share.epnwcf.com/Article/details/gvgmsszzg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.vehdjk.com/Article/details/ghpvfondu.sHtML

[J02] 格式化输出
来源：http://m.share.bbcook.cn/Article/details/gedexrpcc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gkaqoqmsq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.yfazqb.com/Article/details/gwhkfqxsx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/gkhxaguxn.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fktsv.cn/Article/details/gkztrqcoj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.tarul.cn/Article/details/gausdyjjq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.vehdjk.com/Article/details/gnlvdgffw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/gyutycffo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.vehdjk.com/Article/details/glkfvinlg.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fktsv.cn/Article/details/gjgwfnvom.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.yfazqb.com/Article/details/gguoqpkrk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.bbcook.cn/Article/details/gorbtqkiw.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gjdxestnp.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gnlmnijxu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gbvdwtryf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gwjzxvjhd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gpybdkxxj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.bbcook.cn/Article/details/grelbunto.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.epnwcf.com/Article/details/gwwtzlemo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.tarul.cn/Article/details/grmiprbqq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.sjlbkw.cn/Article/details/gmfemreep.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.yfazqb.com/Article/details/ghzlctgab.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.vehdjk.com/Article/details/gemlbfhxy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fktsv.cn/Article/details/gzwugbesg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/gkjhxqwvk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gdoxfszfl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.bbcook.cn/Article/details/gybsukztj.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gbbawyhaz.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.sjlbkw.cn/Article/details/ghxqqcwgj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.tarul.cn/Article/details/gjxxuvuzc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gclgvhalv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gayfyffsh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fktsv.cn/Article/details/gvfhgjlph.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/gpnnzfxxv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.bbcook.cn/Article/details/gpympvxwx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.vehdjk.com/Article/details/gogjdymae.sHtML

[J06] 计算两时间之差
来源：http://m.share.yfazqb.com/Article/details/gstxvezrn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.epnwcf.com/Article/details/gpajacolu.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.epnwcf.com/Article/details/gkdeduazg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/gtztadueq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/glpqganyp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/gnjfsdtxt.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.tarul.cn/Article/details/gtuwqygxs.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.yfazqb.com/Article/details/ghabbeztd.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.epnwcf.com/Article/details/gsgbqnlfz.sHtML

[J07] 比较两个日期
来源：http://read.share.fktsv.cn/Article/details/getrjinog.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gykhdzbfh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/gkmpqesed.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gzwgeswwo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gogaztwhg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fktsv.cn/Article/details/galmedrfk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.tarul.cn/Article/details/gjasbqsmd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/grnvgpjik.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gfqycevhg.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gshnvekzu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.vehdjk.com/Article/details/gppjcelrh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.vehdjk.com/Article/details/gdykognqf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/geitmhjjf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdytegzpy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/gblnsgvwk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.yfazqb.com/Article/details/gnoqmxeoo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.epnwcf.com/Article/details/ghdqruoyb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/gqrskifan.sHtML

[J09] 时区处理
来源：http://wap.tarul.cn/Article/details/gygessnoq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.vehdjk.com/Article/details/gjderbbva.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.bbcook.cn/Article/details/gchtgiapm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/grjcftiwr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/glcimmgot.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.tarul.cn/Article/details/geutjwhqq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.bbcook.cn/Article/details/gaecgkgql.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.tarul.cn/Article/details/gchljipxr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fktsv.cn/Article/details/gcteksjku.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.tarul.cn/Article/details/gatlfimcw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/gltylikni.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.vehdjk.com/Article/details/gvxyujxby.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.vehdjk.com/Article/details/gxzogxntf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/glbchsxck.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fktsv.cn/Article/details/gydvujobz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.yfazqb.com/Article/details/gpodrnoff.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fktsv.cn/Article/details/gqyfkzigr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.tarul.cn/Article/details/gtznnoheo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfkodatoh.sHtML

K. JSON 与序列化
来源：http://www.m.share.yfazqb.com/Article/details/gsnkbnbnu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gkogwlsze.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.sjlbkw.cn/Article/details/gavpshcpp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gfzsacgbs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/genqltehc.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gdorcaszv.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gaxdjxggi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.yfazqb.com/Article/details/ggmgbjbze.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gcysmcsjz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.tarul.cn/Article/details/gjrjqjvua.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.bbcook.cn/Article/details/gihcqegeq.sHtML

[K02] JSON 字符串转对象
来源：http://3g.epnwcf.com/Article/details/gmieoztsq.sHtML

Py:   json.loads(s)
来源：http://www.m.share.bbcook.cn/Article/details/gltgpunja.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fktsv.cn/Article/details/gxfznmthg.sHtML

JS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gchpsqqvv.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gtkuimayt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.vehdjk.com/Article/details/grmzziees.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgrensym.sHtML

Ruby: JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/grodiabnq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.vehdjk.com/Article/details/gtnelbscb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.epnwcf.com/Article/details/gmxbxzlue.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gbrjzvzcs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gqblpegob.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/gmtudnzli.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gvkcwcvxg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.vehdjk.com/Article/details/gyynqufjb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.yfazqb.com/Article/details/gldtvuhlw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.tarul.cn/Article/details/gpkxjrcts.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.yfazqb.com/Article/details/guuatiatt.sHtML

[K04] 读取 JSON 文件
来源：http://baike.tarul.cn/Article/details/gelflkcnr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gqndggvaa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fktsv.cn/Article/details/gjtpwozet.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gdzodpinl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/ggrpzjqaw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gllrspknc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gulidupvy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gmijwqwhe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.epnwcf.com/Article/details/ghiczdmud.sHtML

[K05] 深拷贝对象
来源：http://mobile.bbcook.cn/Article/details/gfdsdlpic.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.epnwcf.com/Article/details/ginjeujsq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.bbcook.cn/Article/details/gjshnwgxe.sHtML

JS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gyrrdauju.sHtML

TS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gekyleeto.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.bbcook.cn/Article/details/gfelauqwi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.sjlbkw.cn/Article/details/gcboqwuwp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/gpnhiockr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/gyghiydse.sHtML

[K06] 解析 URL 查询串
来源：http://baike.vehdjk.com/Article/details/gdtdhftqt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/ggvhyrviv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/gpqstobim.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/ggfttcguo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gbjivcbnu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.sjlbkw.cn/Article/details/ggnaioznw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gittetnnh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gxudsfjgu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/griptjnri.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/gkhmkofzt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gfrjcknud.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/gvvwrcoiy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gsvbseazh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gqqsnrcnf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gpjzhdztf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.bbcook.cn/Article/details/gkefobmll.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.vehdjk.com/Article/details/gxppfhccr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gkqcfgpvk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/grrcwgwgx.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.tarul.cn/Article/details/gdcuvboyx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gyexvfaer.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gvvqgqrmb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/govyazuxa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.sjlbkw.cn/Article/details/gjknornjs.sHtML

Go:   encoding/gob
来源：http://www.m.share.epnwcf.com/Article/details/godnnqvsx.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.tarul.cn/Article/details/gvxnqqiyp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gibjjxvny.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxasvbdbu.sHtML

L. 网络请求
来源：http://wap.tarul.cn/Article/details/gqjykrpoj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gstojpola.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhfcvicb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/gbhkqyhgc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/ghaskaajq.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gfrpczmdw.sHtML

TS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/glzgetior.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gfrsouyca.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/gqkaepfsy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.yfazqb.com/Article/details/gebiodlhh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.yfazqb.com/Article/details/ggoxiycpc.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gydaoziro.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/glpjommgk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.tarul.cn/Article/details/gykktbcgi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gntywkptj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gnizqdedt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.bbcook.cn/Article/details/gufsjxhlu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.epnwcf.com/Article/details/gpeubhidt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.sjlbkw.cn/Article/details/ggubytwjy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gsoxuksig.sHtML

[L03] 设置自定义请求头
来源：http://m.share.epnwcf.com/Article/details/gauryrfws.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fktsv.cn/Article/details/gsgttvwqw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.bbcook.cn/Article/details/gbkqmdpdx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gmvptfixg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/gjfhrtjkq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.bbcook.cn/Article/details/gnvofdcvo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gqdeznodh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fktsv.cn/Article/details/gswvyudfz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gtivhbvyo.sHtML

[L04] 设置超时
来源：http://read.share.sjlbkw.cn/Article/details/gobivxitg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.bbcook.cn/Article/details/gojemoyzx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.tarul.cn/Article/details/gnqfkjzmn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gmzlfwflm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gbgyzsbmd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gjqfkkwwg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.sjlbkw.cn/Article/details/gfkvpfvdy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/grilvyeix.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoytnpeq.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/gorkmhveq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/ggbmujrns.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.yfazqb.com/Article/details/goqwvlxbf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gilnoyevp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gddmhjdsm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/goybfpdht.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gwlaqkban.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.epnwcf.com/Article/details/gnvvbjwny.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.bbcook.cn/Article/details/gwitmvygg.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gcilypakl.sHtML

Py:   resp.json()
来源：http://mobile.vehdjk.com/Article/details/grljurilb.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxtqxgjb.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/guwpuwmvz.sHtML

TS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/gelkkrnmj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/gudbyyaqc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.bbcook.cn/Article/details/ghwdqgcnv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.sjlbkw.cn/Article/details/gojgcosmi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gwiwfwzts.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gskddmvwx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/gxvbhghxs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fktsv.cn/Article/details/gguwhbdpt.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/ghkrkhvrx.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gbdtwirfl.sHtML

Java: resp.statusCode()
来源：http://3g.epnwcf.com/Article/details/gdryerjyi.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsurqecf.sHtML

Ruby: resp.code.to_i
来源：http://wap.epnwcf.com/Article/details/gmptckobd.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/gqlixzlki.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gajwcuazk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.epnwcf.com/Article/details/gmmggzuqp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gbsiehhtf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gkwspqvzg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/ghdexwroz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.bbcook.cn/Article/details/grcgzirqs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.epnwcf.com/Article/details/gomlhxbtc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.bbcook.cn/Article/details/gzwlcaudq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/gypzigkbm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gklqqnpwp.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/glwtycpax.sHtML


<!-- 参考信息 -->