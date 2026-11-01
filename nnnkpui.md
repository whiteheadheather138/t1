代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gekgppmlw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.tarul.cn/Article/details/gvafiiiwm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.yfazqb.com/Article/details/ghnwleucv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/gjndajpsf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/gfvddevkh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.vehdjk.com/Article/details/gjouyamdk.sHtML

[I04] 正则替换
来源：http://3g.fktsv.cn/Article/details/gvxfabnbm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.yfazqb.com/Article/details/gllrkkiwa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fktsv.cn/Article/details/gxdykikto.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gpjajckyp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gcybzpmtv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gldqkcfoc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.yfazqb.com/Article/details/gcqlfqtsa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gxdtuufhp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.vehdjk.com/Article/details/gxxcbttqr.sHtML

[I05] 按正则拆分
来源：http://www.m.share.vehdjk.com/Article/details/gurckzavo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/grgzdxqdr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.tarul.cn/Article/details/gbpkvypuv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/guokvembd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gvngioxsv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/gpdyyykro.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fktsv.cn/Article/details/gycvfikfl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gjhejlcah.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.bbcook.cn/Article/details/guzdolmkp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.epnwcf.com/Article/details/grlkrmzzl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gtclosknj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.tarul.cn/Article/details/gwqctwett.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/guoohezcp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/ggbvbmdes.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gcgxiksai.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.epnwcf.com/Article/details/gkhehzufx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.bbcook.cn/Article/details/gqedfxokp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gwmrquprq.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fktsv.cn/Article/details/gyracnfok.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.vehdjk.com/Article/details/gyhdrpyki.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gvilvcekg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.sjlbkw.cn/Article/details/goxngldgu.sHtML

TS:   /error/gim
来源：http://baike.epnwcf.com/Article/details/gcrwjzhwh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.bbcook.cn/Article/details/gkncketuf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fktsv.cn/Article/details/gcwswmfvb.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fktsv.cn/Article/details/gafjowsbw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/gpjjxwyye.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/gjdajfcjz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.vehdjk.com/Article/details/glyjyudtl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gxyjmfshy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/gapnrdwkw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/grvzrmpmd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gxhlbbvrw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/gbvmrhsdd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.sjlbkw.cn/Article/details/grjssmiwl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gnermlmjk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gexksbjwn.sHtML

J. 日期与时间
来源：http://read.share.sjlbkw.cn/Article/details/gnlorjjlw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/goqdisimi.sHtML

[J01] 获取当前时间
来源：http://m.share.bbcook.cn/Article/details/gzefausou.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.bbcook.cn/Article/details/ggwnsddge.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/ggccaqqzi.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/girxdartf.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gulrfdhzd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.tarul.cn/Article/details/gvelbgihj.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/gsycrgklr.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/gsqbxivog.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fktsv.cn/Article/details/gmqwaoccj.sHtML

[J02] 格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gyilppdld.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/gbwqdifui.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gmdjzbjua.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fktsv.cn/Article/details/gayuxisip.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fktsv.cn/Article/details/gmgdlusfs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.bbcook.cn/Article/details/gnapelzqi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.vehdjk.com/Article/details/gavcgtbdq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gdvyntofo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fktsv.cn/Article/details/gkxfbtspz.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fktsv.cn/Article/details/gifydcmha.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.bbcook.cn/Article/details/gendmwosn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.yfazqb.com/Article/details/gkrfgcgdu.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gynpqymgq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gvuhpahmj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gxyfejgpy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gzgdkdqvd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gljrywbkj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.bbcook.cn/Article/details/gkzujkpec.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.epnwcf.com/Article/details/ghxdbqfzl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.tarul.cn/Article/details/gkhcrukhj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.tarul.cn/Article/details/gwmvxdaqj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.yfazqb.com/Article/details/gtbagetqm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fktsv.cn/Article/details/gscwuedna.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.tarul.cn/Article/details/gvcvglfrw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.yfazqb.com/Article/details/gemivmmyq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.tarul.cn/Article/details/grtepnpwl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fktsv.cn/Article/details/gekwxtuxe.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fktsv.cn/Article/details/gmedvqgpt.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/grbdxwiwp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fktsv.cn/Article/details/gkedgkhvo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/gxarxtgto.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gvhtaiafk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.epnwcf.com/Article/details/gbvdxhwih.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.sjlbkw.cn/Article/details/gmxcnddlz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/gvhaqfhoo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.tarul.cn/Article/details/goyxvpiex.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/glxgnkajp.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fktsv.cn/Article/details/gqxwpsiey.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fktsv.cn/Article/details/gyzsgmdvn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.tarul.cn/Article/details/ggnfhwbmh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.vehdjk.com/Article/details/gjfjnbyky.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gzbpmlnqp.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.sjlbkw.cn/Article/details/ggmkjnals.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.bbcook.cn/Article/details/gurrnxxds.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/gnvwuvcss.sHtML

[J07] 比较两个日期
来源：http://3g.fktsv.cn/Article/details/gtsqhxseq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/gvrkofsti.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.vehdjk.com/Article/details/gwimtiuhn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gsfappttk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gegcerycl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.epnwcf.com/Article/details/gppisffru.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.tarul.cn/Article/details/gyijvizjf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/glkczrrih.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/ggnmcldfm.sHtML

[J08] 提取年月日与星期
来源：http://blog.tarul.cn/Article/details/gtbhjiqvr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fktsv.cn/Article/details/gweeefwvu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.epnwcf.com/Article/details/guumbnbgi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.sjlbkw.cn/Article/details/grmfsnxda.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fktsv.cn/Article/details/gcfkgpctf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.epnwcf.com/Article/details/gylswbuin.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.vehdjk.com/Article/details/ggobxvjkw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.epnwcf.com/Article/details/gaoegpbku.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fktsv.cn/Article/details/geclzqxdk.sHtML

[J09] 时区处理
来源：http://www.share.yfazqb.com/Article/details/gmfmyqwuv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/ggpztnatc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.tarul.cn/Article/details/gvkwsripb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gfvhtzsfk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/grjxvnrir.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.tarul.cn/Article/details/guygbznon.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.tarul.cn/Article/details/gjtivdawm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfecokdt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.yfazqb.com/Article/details/gcaiybfmw.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.sjlbkw.cn/Article/details/gyyersrdw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.epnwcf.com/Article/details/gpzdctjww.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.sjlbkw.cn/Article/details/gbwhjwuex.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.tarul.cn/Article/details/gfwlmlxxt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gugixmxwt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fktsv.cn/Article/details/gsrigxddq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gqhnjpaaf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.vehdjk.com/Article/details/gsarzymmd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.epnwcf.com/Article/details/grthxiwmt.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjxvqdcop.sHtML

K. JSON 与序列化
来源：http://mobile.yfazqb.com/Article/details/gbnanvavp.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvypropjq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fktsv.cn/Article/details/giroloeko.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gcgztknnq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/gucvmoawt.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gzpzwsmpm.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.bbcook.cn/Article/details/gnjklzerx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.yfazqb.com/Article/details/gtjmvudph.sHtML

Go:   json.Marshal(obj)
来源：http://baike.sjlbkw.cn/Article/details/gibodxhst.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/gntsbwsbo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.tarul.cn/Article/details/gwbimsqaa.sHtML

[K02] JSON 字符串转对象
来源：http://wap.bbcook.cn/Article/details/gpjezzvmf.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/gigjmfkbh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.yfazqb.com/Article/details/gyhqznmqe.sHtML

JS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/ghzpheusv.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gauzdzurh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.vehdjk.com/Article/details/gdmxouzku.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gvtbupzlk.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gztzsoekt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.bbcook.cn/Article/details/goniwmslt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.vehdjk.com/Article/details/gevsirzdg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gqyrscbzb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gqyfmlzca.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gfkpfdaph.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gdfsgbabb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.bbcook.cn/Article/details/getfccajq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/grwfxzvsh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.tarul.cn/Article/details/giuoqcgna.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/gvujujwou.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.bbcook.cn/Article/details/gicmdekyh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/gwjeqmivc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.epnwcf.com/Article/details/gopgxkqxn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gjalczyxb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gcccznojk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.bbcook.cn/Article/details/geedrpgon.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwecogiz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gtmzpclhx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.yfazqb.com/Article/details/gbocfhdud.sHtML

[K05] 深拷贝对象
来源：http://3g.sjlbkw.cn/Article/details/gumicwtcc.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fktsv.cn/Article/details/gwhdmmtgu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.tarul.cn/Article/details/ghvcdfqps.sHtML

JS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gjtfabjim.sHtML

TS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/givvoompi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.sjlbkw.cn/Article/details/gknyfcikh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/ggstyqyei.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.tarul.cn/Article/details/gbhjsjrwo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fktsv.cn/Article/details/giqckdczq.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.vehdjk.com/Article/details/ghsrbveni.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.vehdjk.com/Article/details/glkicpuli.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.epnwcf.com/Article/details/gcsafiuth.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gwpyubefn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/gqtpuyudt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/gyvjjkyud.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gwzimksdb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/ghlrkuwji.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/godibgthd.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/gxcaerxhw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/ghnmgplcv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.yfazqb.com/Article/details/gssrvnwyl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gqlgjwyan.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/glqgxpmmi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gehbgyvfk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.bbcook.cn/Article/details/gcvlwgrpx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.yfazqb.com/Article/details/gnddomauj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gevtbckpk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.tarul.cn/Article/details/goiibcyyd.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.bbcook.cn/Article/details/gjulmibsq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/goyvlbrze.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gpazlujbh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gxlkgxjur.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/gexgjeurm.sHtML

Go:   encoding/gob
来源：http://blog.yfazqb.com/Article/details/gehjewgyh.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.sjlbkw.cn/Article/details/gmsefxbjt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gsiugxgii.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzlandktg.sHtML

L. 网络请求
来源：http://www.blog.fktsv.cn/Article/details/glhnitqmf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gneeeihzw.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/gmttfvbkb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.yfazqb.com/Article/details/gpegajjua.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/gxjclvioo.sHtML

JS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gaxiymgyj.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gcyqmlsqv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/grrwhnxlo.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fktsv.cn/Article/details/glpmatbnl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.vehdjk.com/Article/details/gtocluhcu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.epnwcf.com/Article/details/gckggiggl.sHtML

[L02] 发送 POST JSON
来源：http://read.share.tarul.cn/Article/details/gseaqwiub.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gkhgnsgpb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.bbcook.cn/Article/details/gniqrznhz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gqpksspie.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gybjxhgjh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.sjlbkw.cn/Article/details/gwksgivbb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/gcpsepkrp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/glaljymjs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/giucrngug.sHtML

[L03] 设置自定义请求头
来源：http://3g.vehdjk.com/Article/details/gibchunfp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/ggrfuxizw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.epnwcf.com/Article/details/gxeagcunk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gihhimhal.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gqwniwyeg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/guvzffgwc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gvxizlncg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.yfazqb.com/Article/details/gobgmjuby.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/guordypba.sHtML

[L04] 设置超时
来源：http://read.share.fktsv.cn/Article/details/gpzoifowj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.bbcook.cn/Article/details/gaqbeqmjb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/gjwwiwdbe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gbsuccvvj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/grvroimpu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.sjlbkw.cn/Article/details/gdifdrwyj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.tarul.cn/Article/details/gbmqpgvkn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.epnwcf.com/Article/details/gklcuakcz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.tarul.cn/Article/details/gtyrzdxms.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/grlsxifbs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.vehdjk.com/Article/details/gcnjacbqw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.bbcook.cn/Article/details/glzqkzuex.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gejuquvgr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gpkztskvt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fktsv.cn/Article/details/grwmdlbhh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/glkbwwpsj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/gmfpgbobo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.bbcook.cn/Article/details/guusmkdug.sHtML

[L06] 解析响应为 JSON
来源：http://3g.vehdjk.com/Article/details/gegshimcy.sHtML

Py:   resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/ghhwvklwb.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gvkliluhe.sHtML

JS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gxsxfkqtr.sHtML

TS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gpbrjrnvh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gsiradkdu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.bbcook.cn/Article/details/giqtglqes.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.tarul.cn/Article/details/gmbvqyors.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.epnwcf.com/Article/details/gbiakbrbs.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtymrgwj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gfzzcjokq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gkewfpkvj.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/ggrkhwwxb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gptpchdvr.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gvlonfase.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gcorhpcbc.sHtML

Ruby: resp.code.to_i
来源：http://m.share.tarul.cn/Article/details/gewefwvep.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gbahcxbmf.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/glxtcbumy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/ggwjbwdlb.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.bbcook.cn/Article/details/gkiicxlmm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/ggcvgzmnb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gdoxcimze.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.tarul.cn/Article/details/gmptibqxf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.yfazqb.com/Article/details/glpsdgdoo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gzwarjuxx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/gzovvwkem.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gujopevmb.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fktsv.cn/Article/details/guoyywdhf.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjghoxhqr.sHtML

[M01] 读取命令行参数
来源：http://wap.yfazqb.com/Article/details/gcuuvawej.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gclrbhnfo.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.yfazqb.com/Article/details/givwbntxv.sHtML


<!-- 参考信息 -->