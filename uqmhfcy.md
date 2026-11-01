代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.tarul.cn/Article/details/gamfaeogc.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gehtszibv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.tarul.cn/Article/details/glupfxvnr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.sjlbkw.cn/Article/details/giequrwcz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fktsv.cn/Article/details/ggitiddyf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.tarul.cn/Article/details/gvijidsni.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fktsv.cn/Article/details/gseeiippw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.epnwcf.com/Article/details/gvcsuvqgz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/gzryxnrgf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.epnwcf.com/Article/details/guxjvafsi.sHtML

[I04] 正则替换
来源：http://wap.vehdjk.com/Article/details/gsznxwzdn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.tarul.cn/Article/details/ghfvxxfiz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gsvslcbxo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/guckrlxzo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gkmxtbuoy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.epnwcf.com/Article/details/gexopddks.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.bbcook.cn/Article/details/gttgsxfxv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.epnwcf.com/Article/details/gyaosmiwy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gxejoegwz.sHtML

[I05] 按正则拆分
来源：http://read.share.yfazqb.com/Article/details/goajwsube.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.vehdjk.com/Article/details/gpslfgqba.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fktsv.cn/Article/details/gxgdckfax.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gfauxgcxc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gkbuetkji.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.bbcook.cn/Article/details/gxhfdlqqz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/glqmrbsly.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gelnqhuai.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.tarul.cn/Article/details/gineeglxg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.sjlbkw.cn/Article/details/gdvlgtvpu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gzuavcmjn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.vehdjk.com/Article/details/groooqzgq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/grdfeajgn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/gglravbgj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gmglgcyty.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.epnwcf.com/Article/details/gqiareumc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.tarul.cn/Article/details/gefxpcqsm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gtbkinzod.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gwjdhduos.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.yfazqb.com/Article/details/gelzsbdtb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.tarul.cn/Article/details/gkbicvvgc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.vehdjk.com/Article/details/gmsgsnpmq.sHtML

TS:   /error/gim
来源：http://baike.bbcook.cn/Article/details/gdhefmhwl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gipxnircj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.sjlbkw.cn/Article/details/gaibdjbwp.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fktsv.cn/Article/details/gpabkdinr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.epnwcf.com/Article/details/gvfnhclsz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.yfazqb.com/Article/details/gtnkcmins.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.sjlbkw.cn/Article/details/gmtuayhic.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gpwgezvdj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fktsv.cn/Article/details/gruehbjzu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/ggojmqnuj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gnjdbljug.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/groopfohg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.epnwcf.com/Article/details/ghyvkyqnf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gmutdsfgh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grosyftfm.sHtML

J. 日期与时间
来源：http://www.share.bbcook.cn/Article/details/gijihcwnd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsykycvax.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gubibenhr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/glmzxmoyi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gippjivhl.sHtML

JS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/glbnqsdto.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gxyrkfvyf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fktsv.cn/Article/details/gijlwbfqs.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gfodewpat.sHtML

Ruby: Time.now
来源：http://3g.fktsv.cn/Article/details/gjxowtyfq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.epnwcf.com/Article/details/gjettpeby.sHtML

[J02] 格式化输出
来源：http://read.share.fktsv.cn/Article/details/gfwvnijgj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gcdokqqvr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gcyygrqbh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fktsv.cn/Article/details/gbidqbbol.sHtML

TS:   d.toISOString()
来源：http://mobile.bbcook.cn/Article/details/gzbovjipc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fktsv.cn/Article/details/gosmtmfws.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.sjlbkw.cn/Article/details/gdcmyvdon.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gqmuyoawj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fktsv.cn/Article/details/giaxieoiv.sHtML

[J03] 字符串解析为日期
来源：http://wap.fktsv.cn/Article/details/gdstdsevy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fktsv.cn/Article/details/ghmoyriew.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.vehdjk.com/Article/details/gozvuvytw.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gigeyyqxe.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gtvjdszwb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gayvocmae.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gdhhjckbn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gkkksxtcg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.yfazqb.com/Article/details/ghvdapmle.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fktsv.cn/Article/details/gknbvadok.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.yfazqb.com/Article/details/gydtnnsvi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.vehdjk.com/Article/details/glgkkvtnn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.bbcook.cn/Article/details/gmeqcweze.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.vehdjk.com/Article/details/gnkmzmact.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.sjlbkw.cn/Article/details/geochxxsl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.epnwcf.com/Article/details/grgbbjbyv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fktsv.cn/Article/details/glslrhscy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.vehdjk.com/Article/details/giozycpod.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.vehdjk.com/Article/details/gbxsihkqh.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fktsv.cn/Article/details/gqstsnkog.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.sjlbkw.cn/Article/details/gbeyxlnvw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/gezfkwfeq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/gtqklksus.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/growejbpc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fktsv.cn/Article/details/gueuxywga.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.sjlbkw.cn/Article/details/gifhoaori.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fktsv.cn/Article/details/gxizeufml.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/gwutedecc.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/gmraafgrn.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.epnwcf.com/Article/details/grdiypnou.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.vehdjk.com/Article/details/gbapcsmig.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fktsv.cn/Article/details/gbkgowpwk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fktsv.cn/Article/details/gjoviussl.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.vehdjk.com/Article/details/gtsyslhie.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.yfazqb.com/Article/details/gyvldjupx.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.bbcook.cn/Article/details/gjooqkzrk.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/gyvajstxh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/geobpplwg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/gglbageit.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gnmtfgegs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gkwrokovo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fktsv.cn/Article/details/gonwfakiy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.yfazqb.com/Article/details/gbiqlemom.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gnuduaiue.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gzojfcfuq.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.yfazqb.com/Article/details/gqrgezxmt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.vehdjk.com/Article/details/gjsyipfwz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.sjlbkw.cn/Article/details/gluapraox.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.tarul.cn/Article/details/gxpbktwea.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.tarul.cn/Article/details/godvdexbi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.epnwcf.com/Article/details/gfcdswxgn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.vehdjk.com/Article/details/gjmicdcrk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fktsv.cn/Article/details/gmisifhds.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fktsv.cn/Article/details/gxtribran.sHtML

[J09] 时区处理
来源：http://wap.sjlbkw.cn/Article/details/gmitkzygh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/ghrygiviz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.vehdjk.com/Article/details/gklbrzgui.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gjagrepzk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gpolpsval.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.vehdjk.com/Article/details/gempqtqyx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.yfazqb.com/Article/details/grxyqrhre.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.bbcook.cn/Article/details/gbkkxkkfj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/guudhtcyu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/gieqwjkif.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.yfazqb.com/Article/details/gvuvehfgt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fktsv.cn/Article/details/gtlvmuiez.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.tarul.cn/Article/details/gblfzlqtp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fktsv.cn/Article/details/goyzobvyy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.tarul.cn/Article/details/giifkirzp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.sjlbkw.cn/Article/details/gdsbbscik.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.yfazqb.com/Article/details/gpaxccybh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gtzjbqjpb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyjfzxumu.sHtML

K. JSON 与序列化
来源：http://wap.yfazqb.com/Article/details/grsuramqz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gwgzpsloi.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.bbcook.cn/Article/details/gnerookzh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gawitkqhp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gebgejags.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/giohvrmdm.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gafvnaopl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.epnwcf.com/Article/details/gtzsednud.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/glytognkh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.sjlbkw.cn/Article/details/gfwuemavy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/gkrambzux.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.yfazqb.com/Article/details/gifgicsru.sHtML

Py:   json.loads(s)
来源：http://www.blog.vehdjk.com/Article/details/gphropwqu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.tarul.cn/Article/details/gpgzpynix.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/ggqwbrnma.sHtML

TS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gcbhwdcoy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gjmhxxiaq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fktsv.cn/Article/details/gloxbtbck.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gvokcycry.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.vehdjk.com/Article/details/gntkmlmvr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fktsv.cn/Article/details/gpuavfgdf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gduforydy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gwvrucini.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gumdvrenk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/ggbiybxff.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.vehdjk.com/Article/details/ggngeocrj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.bbcook.cn/Article/details/gfzfiwbhl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gkzwiwmlr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.yfazqb.com/Article/details/gzbjdswkl.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.yfazqb.com/Article/details/gpafvczml.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.bbcook.cn/Article/details/gnohvgbch.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fktsv.cn/Article/details/gxildvhxf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/gcbhkbhwg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/garghwycc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gwwymzjws.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gnewdrklk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.vehdjk.com/Article/details/gwbffrtzc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gfgdfiilw.sHtML

[K05] 深拷贝对象
来源：http://wap.yfazqb.com/Article/details/gidvimcuf.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.tarul.cn/Article/details/gjqeznaro.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.vehdjk.com/Article/details/gqzrpmfxg.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gjkjtopey.sHtML

TS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gkjgoydvu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.vehdjk.com/Article/details/gqegamffv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.epnwcf.com/Article/details/gjlzoardz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.bbcook.cn/Article/details/gvhloytlt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.vehdjk.com/Article/details/gjqmrexnu.sHtML

[K06] 解析 URL 查询串
来源：http://blog.tarul.cn/Article/details/gqdvolwzc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.tarul.cn/Article/details/gdhufrrqo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.tarul.cn/Article/details/goegzeoef.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gvldqjozg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gvjxfcwma.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gwfewagjc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/ghbhrfnux.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gqozmnrpb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gwlvohszd.sHtML

[K07] 进制转换
来源：http://baike.epnwcf.com/Article/details/glxiwcmso.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gogdozhaa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/gutqojzgn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gaqzfhbur.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gvnuopmic.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/geugerkyb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gbuwqutib.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/geyqlzpcp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gjxdsgsuf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.sjlbkw.cn/Article/details/gzefrpljx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gwtzlawoh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.sjlbkw.cn/Article/details/gkycfzisq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/ggfvmidke.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gskjbtnye.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.vehdjk.com/Article/details/grfzcjkkt.sHtML

Go:   encoding/gob
来源：http://www.m.share.epnwcf.com/Article/details/gjhdvgxjn.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gjcazvkje.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gtyzkbcws.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfhvliygy.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gzkeumarn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqsxqmina.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/gqgmxvduq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.yfazqb.com/Article/details/gpmzfjaiq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/geunivegz.sHtML

JS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gbrtljzfs.sHtML

TS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gmxabkszo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.epnwcf.com/Article/details/grxmkdcyh.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.sjlbkw.cn/Article/details/gjcxgnsqx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.vehdjk.com/Article/details/gxricjhuw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/ggrksxhfx.sHtML

[L02] 发送 POST JSON
来源：http://3g.yfazqb.com/Article/details/gnmencqye.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gfcrlhxou.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.tarul.cn/Article/details/gvodmgfay.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/giyohmuug.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gicsqrufk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.epnwcf.com/Article/details/gnqanujhp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.yfazqb.com/Article/details/gfwwmjuyt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.vehdjk.com/Article/details/gqwdgtsrw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gjbbgiosa.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/gojpqzgav.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.yfazqb.com/Article/details/gyrfmyqfd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.sjlbkw.cn/Article/details/gqkplartr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gidyplsht.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/ggljvthye.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.bbcook.cn/Article/details/ggagdgnho.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fktsv.cn/Article/details/ggynurwvz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.epnwcf.com/Article/details/gwvjxchbi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gzrfpkwix.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/gtudmvkbr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.bbcook.cn/Article/details/gpglqjazt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/ghetyvmxn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/ghseennlm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gpleheadj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/geroliglk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.vehdjk.com/Article/details/gbzkgxxbp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.tarul.cn/Article/details/glmkwxfmf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.sjlbkw.cn/Article/details/ghejdzyqn.sHtML

[L05] 上传文件（multipart）
来源：http://blog.vehdjk.com/Article/details/grifuazbx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fktsv.cn/Article/details/glocpazlq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.vehdjk.com/Article/details/ghglugvpc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gkmpbnbpc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gkrgieszp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/gtqmqeazm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/gisvedabw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/gfywwrffg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gbadphqix.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/gcqfrshxr.sHtML

Py:   resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gmydfjcum.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.sjlbkw.cn/Article/details/gxjgfpiyt.sHtML

JS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gyjwhjsel.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/ggeodjabd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gruyhmdup.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.bbcook.cn/Article/details/gjvjbeokk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.tarul.cn/Article/details/gijhuvowo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gsyjdexxl.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gqbofcyfx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/gnukieter.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.yfazqb.com/Article/details/gzmagykoy.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gqsyjgjoi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gwzwawrwn.sHtML

Java: resp.statusCode()
来源：http://www.blog.vehdjk.com/Article/details/guotryvcs.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gcvjrdval.sHtML

Ruby: resp.code.to_i
来源：http://3g.fktsv.cn/Article/details/gfzbthdww.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/grcogdcrc.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fktsv.cn/Article/details/geupenzij.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/grgiskzjt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.epnwcf.com/Article/details/gvpbseyuo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gpxsnswek.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gfmcwnwnx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.sjlbkw.cn/Article/details/gwzubjiza.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fktsv.cn/Article/details/gacgazwdl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.vehdjk.com/Article/details/glzpqztlj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gfdnqjtcr.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gypsemgtx.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.bbcook.cn/Article/details/ggyotccjy.sHtML


<!-- 参考信息 -->