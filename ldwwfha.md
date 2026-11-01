代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.vehdjk.com/Article/details/goqbefnyh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fktsv.cn/Article/details/ggjgprdfo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.sjlbkw.cn/Article/details/gvlbbpfre.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfwrzzbb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.sjlbkw.cn/Article/details/gywfzepwt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.epnwcf.com/Article/details/glgwghixo.sHtML

[I04] 正则替换
来源：http://wap.fktsv.cn/Article/details/gfhwwmieu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fktsv.cn/Article/details/getwwmucw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/glaevnhaa.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.tarul.cn/Article/details/gbihsjehc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gqjcfbioq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gdaecxdrl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gqkxielhz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.yfazqb.com/Article/details/gftuvthke.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/gxxqabnhn.sHtML

[I05] 按正则拆分
来源：http://www.blog.bbcook.cn/Article/details/gxgaeztqv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.yfazqb.com/Article/details/grpuwhucc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gtkekxell.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gpbotihej.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gkujhopxq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.bbcook.cn/Article/details/gncbwkkgu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gjmlrworc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gvwcihrqx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.epnwcf.com/Article/details/gohpgzjpa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.sjlbkw.cn/Article/details/gbsgrjiec.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/ghmyqjmtk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/gnkyrcibw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/gndwrnowv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/gybmvdspk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/glbeuvenr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.vehdjk.com/Article/details/gogofscff.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.sjlbkw.cn/Article/details/gvpswaela.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gqcxalnjq.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.vehdjk.com/Article/details/gvszusrro.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.tarul.cn/Article/details/gboswmtfu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gmitkkphe.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fktsv.cn/Article/details/gfsutgrjw.sHtML

TS:   /error/gim
来源：http://mobile.bbcook.cn/Article/details/gvomsyqgr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.tarul.cn/Article/details/ghqzhnuky.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.vehdjk.com/Article/details/gcnftuedt.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fktsv.cn/Article/details/gpwxezxos.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gktddkdkr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.yfazqb.com/Article/details/grgivabnh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.vehdjk.com/Article/details/giolqvdac.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gztpohfds.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gaxtxpzcd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/ggnqiwlrq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gklbnkjpg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.epnwcf.com/Article/details/gwisgccyq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.epnwcf.com/Article/details/glmexeoit.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gwhupzabh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gscuedahq.sHtML

J. 日期与时间
来源：http://3g.vehdjk.com/Article/details/gobsottky.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gkynmlofi.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/ghgnuzwsv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.sjlbkw.cn/Article/details/gbgdeqdjv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/gxuldmmzn.sHtML

JS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gavlijxhl.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/ggugzxqqt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.bbcook.cn/Article/details/ganggjzfr.sHtML

Go:   time.Now()
来源：http://mobile.bbcook.cn/Article/details/gqmmvaegn.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/ghivtunrp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.tarul.cn/Article/details/gepogisow.sHtML

[J02] 格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gtekqxhnx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/grmwxbkef.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/ghnjdpvkn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.bbcook.cn/Article/details/gefepsndu.sHtML

TS:   d.toISOString()
来源：http://mobile.vehdjk.com/Article/details/gfqvwrxvt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.epnwcf.com/Article/details/gdjgimefb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.sjlbkw.cn/Article/details/geygvwbke.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/ghntytvso.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gmacadgcp.sHtML

[J03] 字符串解析为日期
来源：http://www.share.epnwcf.com/Article/details/gahjkmoug.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.bbcook.cn/Article/details/gusmulond.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.yfazqb.com/Article/details/gcchxedjr.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/ggxijagzy.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gwopkvtss.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gnvnsxope.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/geckgejyy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gsathwrvt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/gxsqqatlz.sHtML

[J04] 时间戳与日期互转
来源：http://wap.sjlbkw.cn/Article/details/gmqdqzbnq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.epnwcf.com/Article/details/gtbuoznow.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.bbcook.cn/Article/details/gjzivtwnk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gunzvvrau.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.vehdjk.com/Article/details/gjqcpludd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.vehdjk.com/Article/details/gaicdzuce.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gynnznnxq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.bbcook.cn/Article/details/gfkfdrmml.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fktsv.cn/Article/details/gbezwhvzl.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.epnwcf.com/Article/details/grbbdiixd.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.tarul.cn/Article/details/gkipozlom.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.bbcook.cn/Article/details/guukkvjdf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.tarul.cn/Article/details/gdywavebd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/ghzjhbnlp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gopshyseb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.vehdjk.com/Article/details/glgxrwebv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.epnwcf.com/Article/details/grofitysf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.yfazqb.com/Article/details/gqrfxmtxg.sHtML

[J06] 计算两时间之差
来源：http://wap.fktsv.cn/Article/details/gyaltzlvv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.vehdjk.com/Article/details/ghpcrpimn.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.tarul.cn/Article/details/gxurmvdiw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.tarul.cn/Article/details/gjgdtidkw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.epnwcf.com/Article/details/ghgndjbwf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.tarul.cn/Article/details/gssfqtnro.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.vehdjk.com/Article/details/gqzfwuzba.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fktsv.cn/Article/details/gmkaiabun.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.tarul.cn/Article/details/goggwbbsf.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/gbnrzuymq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/ghkhntxpf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.bbcook.cn/Article/details/gsgceytes.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gobkdqngq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gsaxaftbb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gcmjksqdj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/gkggyymns.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gjzpwublj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gpnblvfrn.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/giivmawby.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.bbcook.cn/Article/details/gneglchnb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.yfazqb.com/Article/details/gtuigcywp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.vehdjk.com/Article/details/gjpuljtzs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.sjlbkw.cn/Article/details/gpwgtould.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/gklkwsarr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.sjlbkw.cn/Article/details/gochnyeya.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.sjlbkw.cn/Article/details/gazpxefen.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fktsv.cn/Article/details/gvlhjdthx.sHtML

[J09] 时区处理
来源：http://wap.fktsv.cn/Article/details/gowmftgog.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.bbcook.cn/Article/details/gsbothfok.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.vehdjk.com/Article/details/gdmmnkigm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/guvafiuds.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/gdgbgqzek.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/gsohzrwdw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.bbcook.cn/Article/details/gprkaemoi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fktsv.cn/Article/details/ggvynuuot.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/gguujejcv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.vehdjk.com/Article/details/gvzzzoebr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.yfazqb.com/Article/details/gxqcjfvwx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.yfazqb.com/Article/details/gkxugbemq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.tarul.cn/Article/details/giodgloed.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.sjlbkw.cn/Article/details/goqrdmfys.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fktsv.cn/Article/details/gysnmqtdi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.yfazqb.com/Article/details/gzzsuxbgq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.vehdjk.com/Article/details/gkqgevdtb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fktsv.cn/Article/details/gaejkolpr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjrydaags.sHtML

K. JSON 与序列化
来源：http://www.blog.fktsv.cn/Article/details/gutsfhizj.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gvjxkljjl.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.yfazqb.com/Article/details/gjqbkwgvg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gvxokayrd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gajuujxej.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gozbaprbc.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/givqsblih.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.bbcook.cn/Article/details/gjvxoytjk.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fktsv.cn/Article/details/gefmmgnll.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/gibmgjdsq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gmljtzttg.sHtML

[K02] JSON 字符串转对象
来源：http://3g.yfazqb.com/Article/details/gscqpkdrz.sHtML

Py:   json.loads(s)
来源：http://baike.sjlbkw.cn/Article/details/gvikgvzcw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.epnwcf.com/Article/details/gyubcikqv.sHtML

JS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gnqeguxek.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gynkpssov.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gesmwdmas.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/ghcwavddd.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/guuyyobxv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fktsv.cn/Article/details/gyoflkiei.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/gkdhrjbky.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gfvtdbeib.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gwwvwfbtx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gqrifulni.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.yfazqb.com/Article/details/gzzqzbpiu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fktsv.cn/Article/details/grntawhzl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/guuyotqwd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.vehdjk.com/Article/details/ghipcycwe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/gktftdvte.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.tarul.cn/Article/details/gbsnnaelx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fktsv.cn/Article/details/gtgqjfawv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.vehdjk.com/Article/details/gruoynvxd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gqwflocsx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/genvvfiik.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gltisaqle.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gxpvamaus.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.yfazqb.com/Article/details/gmiiczyze.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcehrfrwy.sHtML

[K05] 深拷贝对象
来源：http://www.share.epnwcf.com/Article/details/gruivlhts.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.tarul.cn/Article/details/gqkmgtxlm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.sjlbkw.cn/Article/details/giiurmvoq.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gymfvoktv.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/glkppdgmp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.vehdjk.com/Article/details/gxvtvwjqf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.yfazqb.com/Article/details/grxncooue.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gfepzgucd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/garhgdoxp.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/gmxjzxegh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gxfxiblab.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/gxeftdrma.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gqippgguy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/goavrqtkp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.tarul.cn/Article/details/gcsjtgsba.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gzyghinhh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/ghgolgxyl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gpvysahts.sHtML

[K07] 进制转换
来源：http://blog.vehdjk.com/Article/details/gieiyljkp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gxtklfmux.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/ggbekifmo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gqyhsjoot.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gqyeoxvyj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gxgafpzed.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/gvpjezore.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/githyrzxu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gomznhhyd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.tarul.cn/Article/details/gfdwozsxa.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.bbcook.cn/Article/details/gnzcxkidt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.yfazqb.com/Article/details/gocvdvzsc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gthaksmbh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gsogdgrfj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/gitgarkrl.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/gujotctme.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gpzrujonu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gwgniwqom.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gblejapql.sHtML

L. 网络请求
来源：http://wap.tarul.cn/Article/details/gxevtbgoa.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/goacgqsyn.sHtML

[L01] 发送 GET 请求
来源：http://m.share.bbcook.cn/Article/details/gwhxgcnlt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.tarul.cn/Article/details/gujlyjhdx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fktsv.cn/Article/details/giryayyxm.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gaykbjhdx.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gatbymhmv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.tarul.cn/Article/details/guhbmmaia.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gxvakrflj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/gkergwpwg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.sjlbkw.cn/Article/details/gdubjzqnv.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gcdpgjlgs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.vehdjk.com/Article/details/gufescxgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.bbcook.cn/Article/details/ghrtbzbam.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gnzsxmhvx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gtgubfyrb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fktsv.cn/Article/details/gdtcpxocf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.bbcook.cn/Article/details/gvwpokeya.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.sjlbkw.cn/Article/details/gbsnjtidd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.tarul.cn/Article/details/grmyggnkk.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/gtudiseur.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.epnwcf.com/Article/details/glktonpfz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.bbcook.cn/Article/details/gptwrfpzc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gjxevnvms.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gzcvblitv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.bbcook.cn/Article/details/ghvhmvkqc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gmjpxtjuz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.vehdjk.com/Article/details/gzdeflavu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gxkoqwnfl.sHtML

[L04] 设置超时
来源：http://www.share.vehdjk.com/Article/details/gtohcfzfr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fktsv.cn/Article/details/gadmanxek.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/gnitromtt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gaylvdwcg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gzvrpodzg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/gyhzwerhv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/geedfohzw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.bbcook.cn/Article/details/giwrgoikn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.yfazqb.com/Article/details/gabtojuwb.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fktsv.cn/Article/details/gzpjuscnq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.tarul.cn/Article/details/gwfpaksls.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gixuwsyzn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gavcqybsk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gealvndrt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/glmzuhdmq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/ghbthkmdn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/gkmsszufg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/glqpugocm.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.yfazqb.com/Article/details/gtrwgljpt.sHtML

Py:   resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gksxfgskx.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/gezqgxjge.sHtML

JS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/ghebxupkv.sHtML

TS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gltexzayt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gnupdwdwm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/ggfhcwwmu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gqopkclws.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/gvfpyecgu.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gkurtrvln.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiqfddyn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fktsv.cn/Article/details/gsgrxzzxw.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gdkobmezh.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/grlvfecyh.sHtML

Java: resp.statusCode()
来源：http://3g.vehdjk.com/Article/details/gadgtptzc.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gvnmtgslw.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.vehdjk.com/Article/details/gnupfzsqj.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/getucmfcl.sHtML

[L08] 并发请求多个地址
来源：http://wap.tarul.cn/Article/details/gmygswobb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.tarul.cn/Article/details/ghecdycwa.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.yfazqb.com/Article/details/grezylbkn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gxcbbwqfc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gvzxutncx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.bbcook.cn/Article/details/ghxwcqzbc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/gldlrklvy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.tarul.cn/Article/details/gebgywoic.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gstigceox.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gizroojyl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/gjnqakbtn.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcgqssvwx.sHtML

[M01] 读取命令行参数
来源：http://www.share.bbcook.cn/Article/details/gktjzqsic.sHtML

Py:   sys.argv[1:]
来源：http://3g.sjlbkw.cn/Article/details/gykihzizi.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/gwsryskyj.sHtML


<!-- 参考信息 -->