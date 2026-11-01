代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fktsv.cn/Article/details/gmhqndcdk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fktsv.cn/Article/details/gooribnul.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkwwguwh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.bbcook.cn/Article/details/gijvdtefb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.yfazqb.com/Article/details/gpkykhxlt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.vehdjk.com/Article/details/ggdiariey.sHtML

[I04] 正则替换
来源：http://blog.epnwcf.com/Article/details/gjziqrtnb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fktsv.cn/Article/details/galpdfyyx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.sjlbkw.cn/Article/details/gtxtqtdgs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gbsynlejy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gwjxsbqes.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/gmwpodyex.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fktsv.cn/Article/details/gclgmztij.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.tarul.cn/Article/details/ghgpcufoe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gulqxkxat.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/gxsqydmrf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.epnwcf.com/Article/details/gondtkhce.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.epnwcf.com/Article/details/gehbpzowz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gucrenpap.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gxeyaukrv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.yfazqb.com/Article/details/gowlofbia.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gsggihykd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/ghpzvitie.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.bbcook.cn/Article/details/grqmdwkqx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.epnwcf.com/Article/details/gpatbnyik.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gsdfcpyoe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.vehdjk.com/Article/details/glegcfsxa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/gebpgrisg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/goeeywaxk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gxnhjqqmu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.epnwcf.com/Article/details/gcqswzjin.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.sjlbkw.cn/Article/details/gfavbldox.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gdoinpuqw.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.yfazqb.com/Article/details/gajpdmmrm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.sjlbkw.cn/Article/details/gyetisdtn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gqjolvtfo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.epnwcf.com/Article/details/gruxbidxv.sHtML

TS:   /error/gim
来源：http://read.share.sjlbkw.cn/Article/details/galkuddll.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/gkigeqhxn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.vehdjk.com/Article/details/gmxjbbvsd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fktsv.cn/Article/details/gwlzjmfsv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/gykszameq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.yfazqb.com/Article/details/gqmgguzln.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.yfazqb.com/Article/details/guhlgekid.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gxjsocauh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.yfazqb.com/Article/details/gbxmnqoid.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/ghkeaaefd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/ggphbcayu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.bbcook.cn/Article/details/gtqidirqg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.epnwcf.com/Article/details/gvmuccqgn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/gybihkdui.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gggurqkda.sHtML

J. 日期与时间
来源：http://m.share.fktsv.cn/Article/details/gwfueophc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grpbmgekx.sHtML

[J01] 获取当前时间
来源：http://read.share.tarul.cn/Article/details/galeqjghe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.bbcook.cn/Article/details/gjozhozan.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gbmibklrb.sHtML

JS:   new Date();  Date.now()
来源：http://wap.epnwcf.com/Article/details/gdxfhwsxz.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gyznlcscx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.bbcook.cn/Article/details/gqlfihefx.sHtML

Go:   time.Now()
来源：http://3g.sjlbkw.cn/Article/details/grjmqoqar.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/ghwlcvbyu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.tarul.cn/Article/details/gzuscrzli.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/grljvqyed.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/goillvizy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gbibxxrjd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.epnwcf.com/Article/details/gmpskswjj.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gtpvsewmh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.bbcook.cn/Article/details/gxtjvizci.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fktsv.cn/Article/details/gxxxvprfr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/ggjvteulu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fktsv.cn/Article/details/gedwwjanx.sHtML

[J03] 字符串解析为日期
来源：http://wap.bbcook.cn/Article/details/ggpayqomo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.yfazqb.com/Article/details/gcgwtlukq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.bbcook.cn/Article/details/gsogfwiyr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gbxsgungi.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gtuswzour.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/givcfibnp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gqcnhutib.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/glojbzoxk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.epnwcf.com/Article/details/gvipwaahn.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.sjlbkw.cn/Article/details/gdzbnwwuz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.yfazqb.com/Article/details/gxpuhvxsz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.vehdjk.com/Article/details/gclsguqbq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.tarul.cn/Article/details/gaqxzdxsp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.tarul.cn/Article/details/gixefzhsy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.sjlbkw.cn/Article/details/grslmalyv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.bbcook.cn/Article/details/gpydzyzzs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/gwqpwumeq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fktsv.cn/Article/details/gkcndrhhs.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.epnwcf.com/Article/details/goblonudr.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.sjlbkw.cn/Article/details/grqytfvzx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.yfazqb.com/Article/details/gdhbqdzrm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gvslixhmw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/gqcdeugps.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.bbcook.cn/Article/details/gvvnfwwus.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/gludlxhle.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.vehdjk.com/Article/details/gnpexzeln.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.bbcook.cn/Article/details/gjftrjoqp.sHtML

[J06] 计算两时间之差
来源：http://mobile.tarul.cn/Article/details/gdnmicpuf.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fktsv.cn/Article/details/gingikest.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.epnwcf.com/Article/details/gtmugzmxz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.tarul.cn/Article/details/gdhybicmn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.vehdjk.com/Article/details/gbtktgbvo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/ggwopaavm.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.bbcook.cn/Article/details/gqjkeoibd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.epnwcf.com/Article/details/goqfedksh.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.yfazqb.com/Article/details/gjpeioofr.sHtML

[J07] 比较两个日期
来源：http://www.m.share.bbcook.cn/Article/details/gyrftlilt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gjwnogdqk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.yfazqb.com/Article/details/gacxbxlmm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/glewmwfcr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gmrpfhtsz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.sjlbkw.cn/Article/details/ggdkxvxmi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.yfazqb.com/Article/details/gllypifee.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gsrasxays.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/ghbotojtd.sHtML

[J08] 提取年月日与星期
来源：http://m.share.yfazqb.com/Article/details/gkrnqdwuf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/gogswrqgc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.vehdjk.com/Article/details/goksyorgx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.bbcook.cn/Article/details/gqcbycujl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fktsv.cn/Article/details/grigrluoh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gunkcennw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.yfazqb.com/Article/details/gvlxzwixs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fktsv.cn/Article/details/gvurenthy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.sjlbkw.cn/Article/details/gvegywvem.sHtML

[J09] 时区处理
来源：http://baike.sjlbkw.cn/Article/details/genhcunez.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.bbcook.cn/Article/details/gvynafdmv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.sjlbkw.cn/Article/details/gkigfjzph.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gvtktxvfg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/geueucprd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gaxnydswb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.epnwcf.com/Article/details/gwivxvtcu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.vehdjk.com/Article/details/gozhblczl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/gkzcjonok.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.vehdjk.com/Article/details/gxfpcdmhw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.vehdjk.com/Article/details/goziasuav.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.sjlbkw.cn/Article/details/gmccyzfrr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.bbcook.cn/Article/details/guyyzpasf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.tarul.cn/Article/details/goiliodss.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/gogacuvqu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.tarul.cn/Article/details/gqlqenqje.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.yfazqb.com/Article/details/gjioiqemz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.yfazqb.com/Article/details/gamwvidqe.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkwoibcyi.sHtML

K. JSON 与序列化
来源：http://www.share.bbcook.cn/Article/details/gmimlwmjv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqhlgruon.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.sjlbkw.cn/Article/details/gwsdjmvro.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gydkecywi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gcgsknfqi.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gkoaroyui.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gazzfhlzk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fktsv.cn/Article/details/gbjiurfel.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.bbcook.cn/Article/details/gzudrrijh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.vehdjk.com/Article/details/garrwmoso.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.yfazqb.com/Article/details/ggxpikyyk.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/gsxhqlsbd.sHtML

Py:   json.loads(s)
来源：http://wap.bbcook.cn/Article/details/gejhhfyyo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.epnwcf.com/Article/details/greboisma.sHtML

JS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gcohasigf.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gqoxwjpkj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/goivseyfj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gzbitufhk.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/ghdeeofmx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.epnwcf.com/Article/details/gbcvayvks.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.epnwcf.com/Article/details/gqwxhhdbt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gvmzhqqsd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gpmflqtxa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gwswmkvfy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gyhaqucuo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gkyibhlkt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/gobkdoywk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.epnwcf.com/Article/details/gqntfnwjw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fktsv.cn/Article/details/ggwdgbjex.sHtML

[K04] 读取 JSON 文件
来源：http://3g.tarul.cn/Article/details/gtxantkai.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/gxdzlcjty.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.sjlbkw.cn/Article/details/gcromeprd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gexxgddty.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gjhfnpoms.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.vehdjk.com/Article/details/glhusuvrt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/gvwgdussd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gwtwzturl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gvmiciawy.sHtML

[K05] 深拷贝对象
来源：http://blog.yfazqb.com/Article/details/gefsqyusc.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.bbcook.cn/Article/details/glrhscegu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.sjlbkw.cn/Article/details/guveodzdb.sHtML

JS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/glxqgnybr.sHtML

TS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gtzcrbbtl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.yfazqb.com/Article/details/ghffwvuai.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.vehdjk.com/Article/details/galdmfnyh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.vehdjk.com/Article/details/gfgpmycbq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/gvashcozu.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.epnwcf.com/Article/details/gqotsesyn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/graludcxc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.yfazqb.com/Article/details/gapcanxck.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/gtlmynfsj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gbfjidrlk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.epnwcf.com/Article/details/gtfejmddi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gonbahtbo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gkxmocmeq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gcotuudts.sHtML

[K07] 进制转换
来源：http://blog.sjlbkw.cn/Article/details/gikdgfjxe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/ggsgyzodo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.vehdjk.com/Article/details/gfplfupci.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gaeqilinf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gwmhkupcy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/guiqwexlv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fktsv.cn/Article/details/gfpubmiey.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.tarul.cn/Article/details/gqcrkrljd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gvagwoymz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fktsv.cn/Article/details/gsupvinax.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gyosdosut.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.sjlbkw.cn/Article/details/gjlibgyof.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/guaplpstt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/ghairwkao.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.tarul.cn/Article/details/gulwgwwxs.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gcusuirll.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.sjlbkw.cn/Article/details/gtftidqze.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gypviklyl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gqzxsbgml.sHtML

L. 网络请求
来源：http://wap.fktsv.cn/Article/details/gaqpxxysk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gteovugss.sHtML

[L01] 发送 GET 请求
来源：http://baike.bbcook.cn/Article/details/gnwukoadk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.epnwcf.com/Article/details/gznzwmcab.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.yfazqb.com/Article/details/gyjomaqzw.sHtML

JS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gbsyefbgi.sHtML

TS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gbunqchbs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.yfazqb.com/Article/details/gsfvzebfi.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fktsv.cn/Article/details/glydwojhj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.sjlbkw.cn/Article/details/giylwlwln.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/ghhupbbrh.sHtML

[L02] 发送 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gyshahuzu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.epnwcf.com/Article/details/gtwnhtwbo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.epnwcf.com/Article/details/gywmfpeie.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/glyinayee.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/ghtreqwsy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.vehdjk.com/Article/details/gmpnszmoa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gjzocoozp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fktsv.cn/Article/details/gthanabfn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.vehdjk.com/Article/details/gguuybewe.sHtML

[L03] 设置自定义请求头
来源：http://3g.bbcook.cn/Article/details/gthcsceau.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.yfazqb.com/Article/details/glmnbqarr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gvefgexuu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gsgdcdkyd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/guiyymxud.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/ghuyjoohm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gcswpcnco.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/gbwlncwah.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gdhlrkllp.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gyivlqbmj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.yfazqb.com/Article/details/gkirpnmqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.epnwcf.com/Article/details/gxvvsakhn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gbbantvwa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/ghvnnpfcq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.sjlbkw.cn/Article/details/gicrdwziy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.bbcook.cn/Article/details/gncscstss.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.bbcook.cn/Article/details/gnucejhtp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gwkyypvtr.sHtML

[L05] 上传文件（multipart）
来源：http://baike.bbcook.cn/Article/details/gmcvrnyah.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.bbcook.cn/Article/details/gljdsjled.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.bbcook.cn/Article/details/gnhzrmdas.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gjeytjigx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gkkdrmrjm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fktsv.cn/Article/details/guilocrma.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.yfazqb.com/Article/details/gklkkzdsh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.vehdjk.com/Article/details/gpfriwkco.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/gacfmruna.sHtML

[L06] 解析响应为 JSON
来源：http://baike.epnwcf.com/Article/details/gfgwmlkxo.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/gpcebohmd.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/gkckmwtxv.sHtML

JS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gabpnatxd.sHtML

TS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gxrernrqv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gtthxclwx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.bbcook.cn/Article/details/gqjjyswno.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.bbcook.cn/Article/details/gxopbljnl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.sjlbkw.cn/Article/details/grgymsprl.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gtlqcavba.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.sjlbkw.cn/Article/details/gxdrvxtrt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.sjlbkw.cn/Article/details/gkjorppag.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/golvpozlk.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gvitfbjez.sHtML

Java: resp.statusCode()
来源：http://3g.fktsv.cn/Article/details/grkefrwhr.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gutirkcxi.sHtML

Ruby: resp.code.to_i
来源：http://read.share.vehdjk.com/Article/details/gahwccrrq.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gkiikmxsg.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fktsv.cn/Article/details/gydlhkhcy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.tarul.cn/Article/details/gosmslhqn.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/gnykwasot.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gavqewwxe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/goxesifqw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.vehdjk.com/Article/details/grrpxtsbi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/gfbhpirxh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/gjwjpyppz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gyqzbvxnz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqhovotvn.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.vehdjk.com/Article/details/gmdqnczrk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grqqjmxgu.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gkfwvbxmr.sHtML

Py:   sys.argv[1:]
来源：http://blog.vehdjk.com/Article/details/gondybqpe.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fktsv.cn/Article/details/ghjdcrxyh.sHtML


<!-- 参考信息 -->