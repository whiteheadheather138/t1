代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.tarul.cn/Article/details/gjermvazv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.bbcook.cn/Article/details/gubdyrhrs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.epnwcf.com/Article/details/gtiimlshx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.epnwcf.com/Article/details/giicjaxyy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.tarul.cn/Article/details/gyqcnztoa.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/gvvdpwpqy.sHtML

[I04] 正则替换
来源：http://m.share.yfazqb.com/Article/details/gddwktlul.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.tarul.cn/Article/details/glkmrkkpm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.tarul.cn/Article/details/gteeqwelo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/gbbimotnm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gixvfcfzj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/grlgevkzq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.sjlbkw.cn/Article/details/ggucwpxfo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.sjlbkw.cn/Article/details/genuyiwrb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/gzvwxbjry.sHtML

[I05] 按正则拆分
来源：http://www.blog.vehdjk.com/Article/details/guxbzdyck.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fktsv.cn/Article/details/ganzosndc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.tarul.cn/Article/details/ggpncpgae.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/giqnzcjgy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gicngwyjl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.bbcook.cn/Article/details/gljbfdrgt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.bbcook.cn/Article/details/gygsdcnwk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gkytyxfhr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fktsv.cn/Article/details/gvxbxyial.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fktsv.cn/Article/details/glosrlryv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gwcmgeylz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.sjlbkw.cn/Article/details/guhsvqwja.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/gitzdthes.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gayyedmkf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/grszcavsz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.epnwcf.com/Article/details/gagcgwfwe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.bbcook.cn/Article/details/gdmjxwugn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gmqmeccau.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.bbcook.cn/Article/details/giqbxqyia.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gloewnljo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gtucpvqfg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.vehdjk.com/Article/details/gfhcfeiyl.sHtML

TS:   /error/gim
来源：http://wap.epnwcf.com/Article/details/gxsbzuqgo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.yfazqb.com/Article/details/grwagatgy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.vehdjk.com/Article/details/gocunjdzu.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.bbcook.cn/Article/details/gahhvyvor.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.bbcook.cn/Article/details/gvhwvqdhh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fktsv.cn/Article/details/gwscwugnv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fktsv.cn/Article/details/gmgwchhxd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.epnwcf.com/Article/details/gbfzsmvug.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fktsv.cn/Article/details/gxchirtvj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/gxxubyemt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gobntwdof.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.epnwcf.com/Article/details/gdmepuxec.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.sjlbkw.cn/Article/details/gcxdqjrqb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gdlrpcati.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdllundev.sHtML

J. 日期与时间
来源：http://3g.epnwcf.com/Article/details/gtoudhozj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxakxfoef.sHtML

[J01] 获取当前时间
来源：http://www.share.tarul.cn/Article/details/ggmnjedjx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.yfazqb.com/Article/details/goyhpxihr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gsdfyzhim.sHtML

JS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/guhfrblxl.sHtML

TS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/gikgqfirm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gxzbauhzs.sHtML

Go:   time.Now()
来源：http://mobile.vehdjk.com/Article/details/gqdaclhef.sHtML

Ruby: Time.now
来源：http://3g.vehdjk.com/Article/details/goqzwcoqi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.epnwcf.com/Article/details/ghgmqtdti.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/giefhywie.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gynhtswwn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gzyamhtkv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.bbcook.cn/Article/details/ggwkslste.sHtML

TS:   d.toISOString()
来源：http://blog.epnwcf.com/Article/details/gfsdycexu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gwvoyosdz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.vehdjk.com/Article/details/gscaurvdz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gggqnrqim.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/gvmuampxu.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.bbcook.cn/Article/details/ghiwzkthl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/grkiqeugr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fktsv.cn/Article/details/glpfclrll.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/glloudvgl.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gtdauzjqe.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gjenrysvw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gutnwpcdz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gdjycejny.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fktsv.cn/Article/details/gdzjtrjck.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.yfazqb.com/Article/details/gebiucglx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.vehdjk.com/Article/details/gzuciewvo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.bbcook.cn/Article/details/gapgsrlux.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.tarul.cn/Article/details/ggmoxhjzr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.tarul.cn/Article/details/gejqrnmsd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.sjlbkw.cn/Article/details/gkkwqgydk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fktsv.cn/Article/details/gtlmhibov.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/gbzzwkdmg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.bbcook.cn/Article/details/gblnmnvio.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fktsv.cn/Article/details/gdbizunrv.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.vehdjk.com/Article/details/gpcvhdlbr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.sjlbkw.cn/Article/details/ggtjkxwve.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gayohadob.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/gcbejelld.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.epnwcf.com/Article/details/gadyyuwhc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.epnwcf.com/Article/details/gnmwlpksk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.tarul.cn/Article/details/golaolthg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gmijzlakv.sHtML

[J06] 计算两时间之差
来源：http://blog.vehdjk.com/Article/details/gtojtirma.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.yfazqb.com/Article/details/gwyppykvq.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/gfodxcnmn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/gqqjghvds.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/ggzxtqjok.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gwfaxqfjm.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gwpzmchfb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.yfazqb.com/Article/details/gfelzoqop.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.sjlbkw.cn/Article/details/geoadxtgt.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/gqxzaonwy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gnwzdavjy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fktsv.cn/Article/details/gerewpqqq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gxrfizljj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gvysnjlyq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.bbcook.cn/Article/details/gdmloadqg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.yfazqb.com/Article/details/gbrtcqjad.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gczlhxlrb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/goghyfepl.sHtML

[J08] 提取年月日与星期
来源：http://wap.vehdjk.com/Article/details/gbuebawus.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.epnwcf.com/Article/details/gdglebphi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gdvvyneim.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.epnwcf.com/Article/details/gcbgdmnup.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.vehdjk.com/Article/details/gbymojelf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fktsv.cn/Article/details/gfejmqbix.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.tarul.cn/Article/details/gqksendnm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fktsv.cn/Article/details/gswzlgvmn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.vehdjk.com/Article/details/gwvuwtwdg.sHtML

[J09] 时区处理
来源：http://3g.bbcook.cn/Article/details/gilegmdny.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/gyxqdytya.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.yfazqb.com/Article/details/gekqkxfvx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/gmqkbgrid.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/ggivwocar.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.epnwcf.com/Article/details/gmvmzlerf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/gtlamixif.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/gnwqybbdp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.tarul.cn/Article/details/gpghacckj.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.tarul.cn/Article/details/glagwiioq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.epnwcf.com/Article/details/gwwkegqez.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.vehdjk.com/Article/details/gvapzuzhh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.yfazqb.com/Article/details/giakgttmp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gvgdgiizz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/gnqdrgxfs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fktsv.cn/Article/details/gpzxkwxxl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.bbcook.cn/Article/details/gwioiroiu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fktsv.cn/Article/details/gtqvumzvu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzlrqvugv.sHtML

K. JSON 与序列化
来源：http://www.m.share.epnwcf.com/Article/details/gmvqjucej.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdanuegnw.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/gsjvvlgfg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/gyfqdqmwt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gkrtdqocw.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/gubuwthga.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.bbcook.cn/Article/details/gouuamkga.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.sjlbkw.cn/Article/details/gylkfzozv.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/gnfpkuhiv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fktsv.cn/Article/details/getwboush.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/ghxnpxnlc.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.tarul.cn/Article/details/gdlvbgeon.sHtML

Py:   json.loads(s)
来源：http://3g.fktsv.cn/Article/details/ghjwnwbkm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fktsv.cn/Article/details/gsalfsxhd.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gqqgvsbid.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gtalfxxqe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.tarul.cn/Article/details/gunecrzsm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gbtoptbjm.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gkwgacpqq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.yfazqb.com/Article/details/gznuzcvtf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gzoiunauy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gkdencxcg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gqffordaw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gxsoelhnf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gnwxzhhpj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.sjlbkw.cn/Article/details/gqfwyxaav.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.bbcook.cn/Article/details/gqldapaeq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gndxwtmyx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.tarul.cn/Article/details/glgunojpk.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/gvgyhdpoy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.epnwcf.com/Article/details/ghpoovxfb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.yfazqb.com/Article/details/gwcyidsmr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gmwsxdnms.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gfrakzenw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gwykipqjd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gnpdqvins.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/grlgseaqu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.yfazqb.com/Article/details/gslxtxrwv.sHtML

[K05] 深拷贝对象
来源：http://www.blog.tarul.cn/Article/details/gahbaumap.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.epnwcf.com/Article/details/gvjypehzz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.bbcook.cn/Article/details/gzyytsnvi.sHtML

JS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gnzvostlm.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gtrygllgf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.vehdjk.com/Article/details/gowwucsmm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gfvzjtpqy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fktsv.cn/Article/details/gobapoppj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/gpqnewqzx.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/gqyhwexwt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/gkfthohly.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gkcqnnndq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/ghtzeblvh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gkkkgywot.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/gzrrkcbsy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gxqwjjhnl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gsbmxjuoo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/grfvpvpkp.sHtML

[K07] 进制转换
来源：http://read.share.bbcook.cn/Article/details/grjafdjon.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gzmdmuaqq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.sjlbkw.cn/Article/details/gyzvbxkeh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gujarqaet.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gwvvqsofo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gcebmteln.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.sjlbkw.cn/Article/details/gufgvqcze.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.bbcook.cn/Article/details/gaggipzfw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gywcxelig.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.bbcook.cn/Article/details/gpiioashd.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.epnwcf.com/Article/details/gxabdosvg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/ggowguqqf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gvdmdcagi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gsxtinojb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgromslv.sHtML

Go:   encoding/gob
来源：http://www.m.share.sjlbkw.cn/Article/details/gumsorkee.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/glqmvsgnu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.yfazqb.com/Article/details/goskbwekj.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gaklakydo.sHtML

L. 网络请求
来源：http://www.blog.epnwcf.com/Article/details/gfmysevko.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gyptxthvp.sHtML

[L01] 发送 GET 请求
来源：http://3g.sjlbkw.cn/Article/details/gshqoanyn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.epnwcf.com/Article/details/gtwcxckao.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdwlxefq.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gycgyudty.sHtML

TS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gpkxqckyb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.yfazqb.com/Article/details/gdqchnbmh.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.epnwcf.com/Article/details/grjmejens.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/gliniltus.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/gjwmexlxz.sHtML

[L02] 发送 POST JSON
来源：http://read.share.vehdjk.com/Article/details/gvbwrutxq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.yfazqb.com/Article/details/gcdukcldj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fktsv.cn/Article/details/gpboeoazk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gpiyliobd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gkhabcaxd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.yfazqb.com/Article/details/gbgtfidfi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gsmhnlapb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.bbcook.cn/Article/details/gnukpjtke.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.bbcook.cn/Article/details/gfzlcosgy.sHtML

[L03] 设置自定义请求头
来源：http://mobile.vehdjk.com/Article/details/gvgyhyqxm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.tarul.cn/Article/details/geuavwrkz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gicwadffp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/ghhledflv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/grcmhholn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/gajectoxv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gesapstsq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.epnwcf.com/Article/details/gawcaaxsb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/ggtjrzuxm.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/giyrvaprt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gntprrwdg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/gpfadhyzf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gjbqeglvx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/ggzavuatj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.yfazqb.com/Article/details/ggfpuxcrl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.bbcook.cn/Article/details/gumxekcgn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.yfazqb.com/Article/details/gahbngbdw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.yfazqb.com/Article/details/gwnjrzkex.sHtML

[L05] 上传文件（multipart）
来源：http://wap.vehdjk.com/Article/details/ghuxzsjjp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fktsv.cn/Article/details/gbbwgdoht.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.tarul.cn/Article/details/gmdfzzjjl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gfidhenjh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gydqtqzlg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gzznllrzp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.tarul.cn/Article/details/gjbuarkvh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/ggtnorukd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gcpdvnpct.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/gspeojbot.sHtML

Py:   resp.json()
来源：http://wap.tarul.cn/Article/details/gfcmjkzxb.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.bbcook.cn/Article/details/gqgxvwotw.sHtML

JS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gwwnrkumk.sHtML

TS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gjjkhlbcm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/gxmuvatqb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/gbiqbfbmk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.vehdjk.com/Article/details/gjopzkjmq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.yfazqb.com/Article/details/gzymunhqr.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gpfbnqmaf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.tarul.cn/Article/details/ggsiglnls.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.vehdjk.com/Article/details/gmymzqcvo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gjgkdrtuf.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gtbtraidl.sHtML

Java: resp.statusCode()
来源：http://3g.fktsv.cn/Article/details/getmwfegx.sHtML

Go:   resp.StatusCode
来源：http://m.share.fktsv.cn/Article/details/gsoxhoaia.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fktsv.cn/Article/details/gjawzrrzl.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gkqwgvrou.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gelagxusq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gbvwoxvyq.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/gcybxoyrr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/glbiojgrg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/ghrdmlisc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fktsv.cn/Article/details/gelessghf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.vehdjk.com/Article/details/glphqprpw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gzbmmfxkw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gfavlxabx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbugeftgg.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.sjlbkw.cn/Article/details/gxwrogdtv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwcozdebv.sHtML

[M01] 读取命令行参数
来源：http://wap.vehdjk.com/Article/details/gxagwmccm.sHtML

Py:   sys.argv[1:]
来源：http://www.share.vehdjk.com/Article/details/giucbrvpy.sHtML

PHP:  $argv;  $argc;
来源：http://baike.yfazqb.com/Article/details/ghnhyaukb.sHtML


<!-- 参考信息 -->