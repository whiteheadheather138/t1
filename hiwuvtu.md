代发 wailian999

[I02] 提取所有匹配
来源：http://www.share.bbcook.cn/Article/details/gknxlvbum.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gvorvvyqj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.bbcook.cn/Article/details/grdatzekn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.bbcook.cn/Article/details/gpspsqvyf.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.epnwcf.com/Article/details/gsrnaxwop.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.bbcook.cn/Article/details/gvmplupgm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fktsv.cn/Article/details/ghsqqifvu.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.bbcook.cn/Article/details/glbrlazsn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/glupttmjd.sHtML

[I03] 提取捕获分组
来源：http://www.share.bbcook.cn/Article/details/goqjbaooh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gdqgqtlrm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.epnwcf.com/Article/details/gevlszsch.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.bbcook.cn/Article/details/gmtlstpsy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.vehdjk.com/Article/details/gatboojag.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.tarul.cn/Article/details/gzhcgrpca.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.tarul.cn/Article/details/gtgtdjuyh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/gpubcebam.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.epnwcf.com/Article/details/gaxdlvoxv.sHtML

[I04] 正则替换
来源：http://wap.epnwcf.com/Article/details/gnhpbysli.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.bbcook.cn/Article/details/gqpfvtwog.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gskkvgqef.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gscgttyub.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/glzrnbmwy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gzmoiwqqf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.vehdjk.com/Article/details/gfalsybyq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.vehdjk.com/Article/details/grqvhwtvh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fktsv.cn/Article/details/glknmxtkl.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/gjqfgzzbp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.sjlbkw.cn/Article/details/gtkumosmi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.vehdjk.com/Article/details/gbrarxvss.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gdygmoqwp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/grmnhujdd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.bbcook.cn/Article/details/gzfhnituu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/ggfhobgoj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gogksbmjs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gdddyxiuf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/gjdkbvhec.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gewmxvjuy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.sjlbkw.cn/Article/details/gaejvojcf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gaarxkass.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.vehdjk.com/Article/details/gnhfjdiks.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gpbzxxdav.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.epnwcf.com/Article/details/gzpjnhgsy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gwaaruxfg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gllnzvams.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.sjlbkw.cn/Article/details/goyevhfgz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.vehdjk.com/Article/details/gsrrhlrqg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gtseudlxg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.tarul.cn/Article/details/gzeepxqkn.sHtML

TS:   /error/gim
来源：http://www.blog.tarul.cn/Article/details/gldivychv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/gisbrfsfo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.epnwcf.com/Article/details/gcdjkoztq.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/grjupxygi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.vehdjk.com/Article/details/glmldqsfx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.yfazqb.com/Article/details/glnurerjw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.bbcook.cn/Article/details/guaenauoe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/givtlktci.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.yfazqb.com/Article/details/gqzdkqhdy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gluswsjqx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.bbcook.cn/Article/details/gemoqacud.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.sjlbkw.cn/Article/details/ghosyrcvi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.vehdjk.com/Article/details/gbxlivvuy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/glkkqicao.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzrhgsdhl.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/gbiepihlk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmcxihths.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gmngjaqob.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fktsv.cn/Article/details/gvlxcvnmt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/glvdnvjix.sHtML

JS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gwjfmwdzp.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/grxmgozcv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.sjlbkw.cn/Article/details/gtqsvstvp.sHtML

Go:   time.Now()
来源：http://www.m.share.epnwcf.com/Article/details/gijvctpye.sHtML

Ruby: Time.now
来源：http://m.share.bbcook.cn/Article/details/gedjodtuq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.yfazqb.com/Article/details/gghacsnpi.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/guywbvmko.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/glzhvsvig.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/galdxcqli.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.yfazqb.com/Article/details/gzbebiarl.sHtML

TS:   d.toISOString()
来源：http://baike.bbcook.cn/Article/details/gltmhylrp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.bbcook.cn/Article/details/gjhdijrlf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.epnwcf.com/Article/details/gzclixzxp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gfybyyhgt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fktsv.cn/Article/details/ggmqlaini.sHtML

[J03] 字符串解析为日期
来源：http://3g.bbcook.cn/Article/details/grtzkrakf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fktsv.cn/Article/details/gvttjxyuj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.bbcook.cn/Article/details/ghbjgyjtq.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gxhfaduvs.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gbopuvrpk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gctzdsyfc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gdpoytjqg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gbfijlfva.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/gpvlcapzw.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.vehdjk.com/Article/details/gfxuzuhbr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/gmqadtawb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gtadbkatt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.tarul.cn/Article/details/gisdjhbvx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/gszykkiyj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/gaauvvafo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gbmabszxs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.bbcook.cn/Article/details/ghjljbewk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gsdfonokz.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.bbcook.cn/Article/details/gfnqyvbim.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.bbcook.cn/Article/details/gezkhysvs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fktsv.cn/Article/details/gmlgbnfph.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/gjeyzypnq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/gtjwwmqla.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gxbgnstwm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.yfazqb.com/Article/details/gwqwfbxqe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.yfazqb.com/Article/details/ggyruddey.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/gjqepzwia.sHtML

[J06] 计算两时间之差
来源：http://wap.fktsv.cn/Article/details/gbsscrvaf.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.yfazqb.com/Article/details/gurzfejsz.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.yfazqb.com/Article/details/gqhzwjbrs.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.yfazqb.com/Article/details/gfknnttmv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.sjlbkw.cn/Article/details/ghpihnqhn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.bbcook.cn/Article/details/gkpaqkbvv.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.epnwcf.com/Article/details/gysikqbmi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.sjlbkw.cn/Article/details/gggwdhpze.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.epnwcf.com/Article/details/gessxhyuh.sHtML

[J07] 比较两个日期
来源：http://wap.fktsv.cn/Article/details/gvmpsvunj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gcstnygqy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.bbcook.cn/Article/details/gllpvhirm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/gtbhhelsh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gjpuxjtnd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.yfazqb.com/Article/details/gyjzjstpj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/gkhlithhw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gtpyqidkd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gaildvnjc.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.vehdjk.com/Article/details/gpgjpskew.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.epnwcf.com/Article/details/gkowfqazi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.vehdjk.com/Article/details/gncdppweo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.bbcook.cn/Article/details/gddsurjzm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fktsv.cn/Article/details/gebypjoeu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/gioksbiuf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.yfazqb.com/Article/details/guavtcxtr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fktsv.cn/Article/details/gonlzlzqu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gcxcdvlmi.sHtML

[J09] 时区处理
来源：http://www.share.vehdjk.com/Article/details/gkqvsizqv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.epnwcf.com/Article/details/golixxpcw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.tarul.cn/Article/details/gsgiqkivr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gznmegovd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/gsrobgctt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.yfazqb.com/Article/details/gjpvqrfmg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.vehdjk.com/Article/details/gbfqcuhly.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.sjlbkw.cn/Article/details/gcfddnyln.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.epnwcf.com/Article/details/gsdkzohvy.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.sjlbkw.cn/Article/details/gytaqjqzg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.bbcook.cn/Article/details/gqiyfhlut.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gotfqjbrn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.epnwcf.com/Article/details/gushnfrxd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.bbcook.cn/Article/details/gnccgcmav.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.tarul.cn/Article/details/gizcnuwli.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.sjlbkw.cn/Article/details/giybpnfin.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.yfazqb.com/Article/details/gnpfplbtl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.tarul.cn/Article/details/giozzjuym.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkmnrmlwl.sHtML

K. JSON 与序列化
来源：http://baike.yfazqb.com/Article/details/gqbxwvkhx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwsupkryq.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.sjlbkw.cn/Article/details/gttlmmhev.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gapczokvk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/ggicvwalq.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gylxxqkzt.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gehypusgz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.epnwcf.com/Article/details/gnrrviodg.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.epnwcf.com/Article/details/gdjyxomec.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.vehdjk.com/Article/details/gtfyodjyf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.vehdjk.com/Article/details/gqqimlqfs.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.tarul.cn/Article/details/gdzdcedpg.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/govwuktft.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fktsv.cn/Article/details/gbmfunuqv.sHtML

JS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/ghoqvftbt.sHtML

TS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/ghxlgptkz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.yfazqb.com/Article/details/gcpsjkxsz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gltepenuf.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gvvbpukal.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.tarul.cn/Article/details/gfejemvht.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/gcyddzrji.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gslggnwut.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/gsfvdlzdf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gmpzsidbw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/gfhwmavnu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fktsv.cn/Article/details/gcbwagejg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fktsv.cn/Article/details/gmjmtmtun.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.epnwcf.com/Article/details/gjkivuyef.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.sjlbkw.cn/Article/details/gnnslkhzg.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/gqqzpcgef.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.tarul.cn/Article/details/ghfrydtav.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.vehdjk.com/Article/details/gpqzxgbbb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.yfazqb.com/Article/details/gdahgbsok.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gmeltivqq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gkhiocqdj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/gughvefeh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.tarul.cn/Article/details/gqteybrab.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/grlxohoqv.sHtML

[K05] 深拷贝对象
来源：http://baike.epnwcf.com/Article/details/gpisthjcz.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.yfazqb.com/Article/details/glszrzsip.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fktsv.cn/Article/details/ggtpjcljd.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gipuuinpj.sHtML

TS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gboanlitn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/guawurvsk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/gvswtdxtz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.yfazqb.com/Article/details/gyopqvrzh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/goyfsnhxt.sHtML

[K06] 解析 URL 查询串
来源：http://wap.tarul.cn/Article/details/gkvexmvin.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.yfazqb.com/Article/details/gpiynhdob.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/geadbvbhs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gfgabnqox.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gcmlttnxf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gbgmgcmaf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gaqatfunb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gvdiggnsr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrfaasor.sHtML

[K07] 进制转换
来源：http://mobile.vehdjk.com/Article/details/gduzyliza.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gpleabdod.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.tarul.cn/Article/details/guytghaay.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/glgryorri.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gtswukiwm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gzrxxjnzv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.epnwcf.com/Article/details/gbwvpopei.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/gnsmgzpdw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gbspwqwhd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.tarul.cn/Article/details/gpkllfsvh.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/grfdfltnn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/gtmetxxhw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gwtvpnnxy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/geuifotld.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.bbcook.cn/Article/details/gqgqkbcnl.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/gwgsltkir.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/gvtznckhl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gpjfdzeff.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvcmbbgux.sHtML

L. 网络请求
来源：http://blog.bbcook.cn/Article/details/gqdoztpku.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gntbaycas.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fktsv.cn/Article/details/gqcfjprfb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fktsv.cn/Article/details/gyxsmrkuf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gmgtndema.sHtML

JS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gcxxxcjqr.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gosvpgyrd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/glmxklfjd.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.sjlbkw.cn/Article/details/gmtlqqkvl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/gxacqhudx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gqscntark.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/ggctlwlhn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fktsv.cn/Article/details/gsvuunlay.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.vehdjk.com/Article/details/gwtlnnlwn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gfbmqdesc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/ghidlculw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/ghrtjuuny.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.bbcook.cn/Article/details/gvfjmejvq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjafuhlll.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/ggqpdajgi.sHtML

[L03] 设置自定义请求头
来源：http://wap.fktsv.cn/Article/details/guzzsqztf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fktsv.cn/Article/details/gdgebigab.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gjnfjabbc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gwrjcxjgy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gyrfwffdq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.sjlbkw.cn/Article/details/ghnpdnbdv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gpbmbjwjr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.yfazqb.com/Article/details/gvxcfbryk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/gpsiqjeir.sHtML

[L04] 设置超时
来源：http://m.share.epnwcf.com/Article/details/gsbxscppk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.yfazqb.com/Article/details/gnmnzpdzm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.tarul.cn/Article/details/gisvilnqe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gwntxpjtm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gaiqafeur.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gqfxxxnnj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gjxbmdrhc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gogovormj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.tarul.cn/Article/details/gcxyyfbvq.sHtML

[L05] 上传文件（multipart）
来源：http://wap.epnwcf.com/Article/details/gkegvqvgj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.yfazqb.com/Article/details/gwnnvznjf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.sjlbkw.cn/Article/details/gpozyyoad.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gyauzmgfj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gexzumzgc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.sjlbkw.cn/Article/details/gjyqfgbhz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.yfazqb.com/Article/details/gkoyneoxp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.bbcook.cn/Article/details/gzodaysyz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gqggpbviu.sHtML

[L06] 解析响应为 JSON
来源：http://3g.sjlbkw.cn/Article/details/ghdavzsgc.sHtML

Py:   resp.json()
来源：http://m.share.yfazqb.com/Article/details/gozfyzxqn.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.tarul.cn/Article/details/gmftsgzhw.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gtsnhduay.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gwhcblycv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/ghtrjmylv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.vehdjk.com/Article/details/gdgxytowj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.bbcook.cn/Article/details/glyoejrcq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.tarul.cn/Article/details/gwfgpeqce.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gjoczijkm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/ghtpkxlfk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gqeahpjcw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/grvhacuug.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/graqccpks.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/grmvrbbxq.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/gtwxoimns.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gooefvjba.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gqpvtnjfg.sHtML

[L08] 并发请求多个地址
来源：http://blog.bbcook.cn/Article/details/gvesbqxxt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.epnwcf.com/Article/details/gxjvofzjo.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.bbcook.cn/Article/details/gsiillxnf.sHtML


<!-- 参考信息 -->