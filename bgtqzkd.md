代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/gonpgsabg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.vehdjk.com/Article/details/gfhadwcrl.sHtML

[I04] 正则替换
来源：http://wap.sjlbkw.cn/Article/details/gqpzlyenu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.epnwcf.com/Article/details/gubiwigvo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gshfyczlp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/ggbabtfmr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gkcfboogx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.epnwcf.com/Article/details/gphkjhfwq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.vehdjk.com/Article/details/goxctuuxs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.tarul.cn/Article/details/gxucslfsh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gfcbzlleq.sHtML

[I05] 按正则拆分
来源：http://www.share.epnwcf.com/Article/details/ghsdkrlqc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.bbcook.cn/Article/details/gcdsmarlk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.vehdjk.com/Article/details/grdyqpehf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gekufdymy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gudzkgvsj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fktsv.cn/Article/details/glmfrukml.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.yfazqb.com/Article/details/grbaeffns.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gdtqglvya.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.yfazqb.com/Article/details/gzitkacjv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/gfuufaycy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gwzvgapqi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.yfazqb.com/Article/details/gudlntmem.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gsnimppeg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.epnwcf.com/Article/details/geptzxhkg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gffvmetig.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.tarul.cn/Article/details/gaznbrjlg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.yfazqb.com/Article/details/gqxkpygzq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gajmfmbtm.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.sjlbkw.cn/Article/details/glfpmmtau.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.vehdjk.com/Article/details/gqprfcaxq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.yfazqb.com/Article/details/ggfmpwkhu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.tarul.cn/Article/details/gtvnydvje.sHtML

TS:   /error/gim
来源：http://baike.fktsv.cn/Article/details/gdxesyxia.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fktsv.cn/Article/details/gdryfmddd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxffluyrm.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.epnwcf.com/Article/details/gicwsntsr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gytbzeufe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fktsv.cn/Article/details/ggsxqycez.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.sjlbkw.cn/Article/details/gqepicvkh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.tarul.cn/Article/details/glzhlnrah.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/glaglnmcr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gqviysvkp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.tarul.cn/Article/details/gfeddxzua.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.yfazqb.com/Article/details/gygykpnyp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fktsv.cn/Article/details/gnxgyfcnc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fktsv.cn/Article/details/gpztrpgrm.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gqtymimai.sHtML

J. 日期与时间
来源：http://www.m.share.tarul.cn/Article/details/gruoegebr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gljjvxxfo.sHtML

[J01] 获取当前时间
来源：http://www.share.fktsv.cn/Article/details/ghnksghhu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.sjlbkw.cn/Article/details/gqsqjywkm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gwwoafmqo.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gobkypphx.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/ghxskxhcs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fktsv.cn/Article/details/gakdbbycd.sHtML

Go:   time.Now()
来源：http://wap.fktsv.cn/Article/details/gqqumuwsx.sHtML

Ruby: Time.now
来源：http://baike.yfazqb.com/Article/details/gfycpjyso.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.sjlbkw.cn/Article/details/gcsfuieap.sHtML

[J02] 格式化输出
来源：http://blog.sjlbkw.cn/Article/details/ghcvnyxtj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/gfnznbgmw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/gcmcjdbqz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.vehdjk.com/Article/details/gtbtynprd.sHtML

TS:   d.toISOString()
来源：http://3g.epnwcf.com/Article/details/gxwkxmqpn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.yfazqb.com/Article/details/gewnnexfg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.sjlbkw.cn/Article/details/gozpgewrh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gufilueqy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.epnwcf.com/Article/details/givilngqt.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gdbebyvcb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.tarul.cn/Article/details/gkvugehjm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.yfazqb.com/Article/details/gtudsxyov.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gesklozyp.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/geahnmpuz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gexmznunv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gsvsqwkkx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gnpbgeiza.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/gcxqdgpys.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.epnwcf.com/Article/details/gccusbxbe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.bbcook.cn/Article/details/gveqgjdfo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/gztdzinlv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.vehdjk.com/Article/details/gtqixntlp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/gtmjmedwx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.yfazqb.com/Article/details/gudyfbwtu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/grmzheqxb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gtvxxvqgy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/gtctelkcn.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.epnwcf.com/Article/details/gvblkahyo.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.epnwcf.com/Article/details/grshtujlb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.epnwcf.com/Article/details/gmqxyyhgz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/giceoutjk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gvkkcpmjv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gekihuwlr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.sjlbkw.cn/Article/details/gopxaapkn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.yfazqb.com/Article/details/glsoalaps.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fktsv.cn/Article/details/gbwqcmhqk.sHtML

[J06] 计算两时间之差
来源：http://m.share.epnwcf.com/Article/details/ggrmmkpqh.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.yfazqb.com/Article/details/gklphjlkv.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.tarul.cn/Article/details/giyxfoypn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.yfazqb.com/Article/details/gdqoryubb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.bbcook.cn/Article/details/gbcgsjyab.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.tarul.cn/Article/details/guliqosje.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.vehdjk.com/Article/details/gtlwjnvwx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fktsv.cn/Article/details/gmktwybfd.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fktsv.cn/Article/details/grcujpomb.sHtML

[J07] 比较两个日期
来源：http://www.blog.sjlbkw.cn/Article/details/gilcufivp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gkgbqjznl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.yfazqb.com/Article/details/ghmspcheu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gfehzwkwz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gbrdujswm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.yfazqb.com/Article/details/geutgdnpe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gunvcnkva.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gnghvgwpo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gjyfilisz.sHtML

[J08] 提取年月日与星期
来源：http://wap.tarul.cn/Article/details/gtzehikqf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/gadgdzfbx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.vehdjk.com/Article/details/gldmizwpv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.epnwcf.com/Article/details/gsyydggyi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.yfazqb.com/Article/details/gmxmqfoig.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/gsihkrqaj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.yfazqb.com/Article/details/gargaabvr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.yfazqb.com/Article/details/gxraqegns.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gmudlispo.sHtML

[J09] 时区处理
来源：http://read.share.bbcook.cn/Article/details/gbsckibia.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.vehdjk.com/Article/details/gapukbjiz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.bbcook.cn/Article/details/gxfvpiyxe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gnyzmykew.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gexfncatz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.yfazqb.com/Article/details/gwmttjasc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.epnwcf.com/Article/details/ggqjqdfdk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/grkhsarha.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.vehdjk.com/Article/details/gmrpxknxi.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.tarul.cn/Article/details/genhiltig.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/gbilfwjtk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/geunodpbn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.sjlbkw.cn/Article/details/gnnvmyort.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gotzaedmu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.yfazqb.com/Article/details/gxubxgtft.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.bbcook.cn/Article/details/gwlmdekiq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.vehdjk.com/Article/details/grleyaybi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.bbcook.cn/Article/details/gvvzgpemx.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gtdfhypbt.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/ghlapxfvp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gysbunslm.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.tarul.cn/Article/details/gywpnvqpm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.tarul.cn/Article/details/grjnysmnf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gqlwhwbbe.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gigvzakhf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpntntcxy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.bbcook.cn/Article/details/gaixitnoq.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fktsv.cn/Article/details/gypzptzft.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.yfazqb.com/Article/details/gsnjhmpyt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gnscvzfjv.sHtML

[K02] JSON 字符串转对象
来源：http://wap.epnwcf.com/Article/details/ggetrhymd.sHtML

Py:   json.loads(s)
来源：http://m.share.yfazqb.com/Article/details/gljbymgnf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.epnwcf.com/Article/details/gquitomxx.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/giyixpikp.sHtML

TS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gnuhvpmib.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gzczzirrh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.epnwcf.com/Article/details/gidlapcjy.sHtML

Ruby: JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gcqlamvvb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.sjlbkw.cn/Article/details/gatuycxje.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.tarul.cn/Article/details/gywdvzmzl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/glrazmhte.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/gbugolyzb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gcincawtp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gkskqvirf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.epnwcf.com/Article/details/gzucihbij.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gytfcbodl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.bbcook.cn/Article/details/gnqwjnhfg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fktsv.cn/Article/details/gpyecsfqq.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.tarul.cn/Article/details/gqztalgno.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.epnwcf.com/Article/details/ggwgefxlb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.bbcook.cn/Article/details/gdnkypqve.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gjzoscstx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuxtqguc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gwlybccdx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gvkjuptzm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.epnwcf.com/Article/details/gncehkciu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gaubqioow.sHtML

[K05] 深拷贝对象
来源：http://wap.tarul.cn/Article/details/gnuvsbqrr.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.vehdjk.com/Article/details/gsvzmkugw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.vehdjk.com/Article/details/gfscfptfx.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gzuxsnrmn.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gqbkymxno.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.vehdjk.com/Article/details/grbeztads.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fktsv.cn/Article/details/gakselxyu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.epnwcf.com/Article/details/grxdwcbao.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.epnwcf.com/Article/details/gmiaaigzf.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.yfazqb.com/Article/details/gabghlzep.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.epnwcf.com/Article/details/gepksbana.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/ggbvjgvyc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gmgstacqu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.vehdjk.com/Article/details/gjmcbkrms.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gfzhalpvu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/ggohjoupw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gdbahbeja.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gzkcxhbpt.sHtML

[K07] 进制转换
来源：http://www.blog.yfazqb.com/Article/details/gcajcffdg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/gfpiubycl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/giiqyyawx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gykbqmcar.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gwvscsevx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gjrrrltxx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/gzuqhxnee.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gqcbuqbtd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gzazrsegs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.epnwcf.com/Article/details/gjkbmowyx.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.yfazqb.com/Article/details/gjolwhmrn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.vehdjk.com/Article/details/ghrclooml.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gacutlsrj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/ggfozncvv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.bbcook.cn/Article/details/givpmmkol.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/gvwwwyzcd.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.sjlbkw.cn/Article/details/gxdslghyn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gyjeabxxh.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gfjfysjfj.sHtML

L. 网络请求
来源：http://baike.tarul.cn/Article/details/gdkorbkvt.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ggzwgonbd.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gnirzgcej.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.sjlbkw.cn/Article/details/gzxkzfbnp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/ghsicmgql.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbaghnfe.sHtML

TS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gvutxuicg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/glexinonl.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/gjnmnmwcd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gdiyuumfj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fktsv.cn/Article/details/gkhkybhdt.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gekbbyept.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fktsv.cn/Article/details/guwhiiczb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.sjlbkw.cn/Article/details/gickyrqvr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gohgpyjsx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/ghfdhyjnd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.tarul.cn/Article/details/gfadmzuqc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gjznngfkp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/gsrkeneev.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.sjlbkw.cn/Article/details/gdeqqsnbf.sHtML

[L03] 设置自定义请求头
来源：http://3g.fktsv.cn/Article/details/gvfgnsdov.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/gfyyqilhy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.bbcook.cn/Article/details/gnmxlmfrz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gmetihuoz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gkgidbvte.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.sjlbkw.cn/Article/details/glbabhyhb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gqjtnrozg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.sjlbkw.cn/Article/details/gsouuuqjl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gwkcqkdgt.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/glopcmhok.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gililpddn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/ggadhyioh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gsktdqoou.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gqbsrhojf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.tarul.cn/Article/details/gttjgghpl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.epnwcf.com/Article/details/gecrvtxnl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.tarul.cn/Article/details/gpvbczxjw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fktsv.cn/Article/details/ghptztzgb.sHtML

[L05] 上传文件（multipart）
来源：http://3g.bbcook.cn/Article/details/gxbcmrtwv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/gifdlwnyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.epnwcf.com/Article/details/gddoyrqml.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gbktzvbnh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.tarul.cn/Article/details/gtebqasrm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fktsv.cn/Article/details/gsjuoactj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/gxqujyvti.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gdqnuzzeo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/grjyubjya.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.sjlbkw.cn/Article/details/gjcskgyyo.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/gyubbnose.sHtML

PHP:  json_decode($body, true);
来源：http://baike.vehdjk.com/Article/details/gthkeqiaw.sHtML

JS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/ghxujsfvy.sHtML

TS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gknzlqlvm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gmewuukqq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gdrkrbihj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gedtorbak.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.bbcook.cn/Article/details/gvmewjzrb.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gimnqpzmy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.tarul.cn/Article/details/gitkmodyz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/ganfnpvsi.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/ghzwijnrb.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/grdubywfu.sHtML

Java: resp.statusCode()
来源：http://www.m.share.epnwcf.com/Article/details/gjombfbof.sHtML

Go:   resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gwrwimhhb.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/ghnxwrpgv.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gjgryuwgk.sHtML

[L08] 并发请求多个地址
来源：http://baike.yfazqb.com/Article/details/gpijzsunm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.tarul.cn/Article/details/ghtdlzesn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.yfazqb.com/Article/details/gxszekbvc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gosgnxumg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gbxaozdbi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.bbcook.cn/Article/details/gzarzcfhy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.tarul.cn/Article/details/grjcikvce.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gtpqdcqjm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/gljhhnkzf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfeebrvcr.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.sjlbkw.cn/Article/details/gdjubneqp.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghybuiprm.sHtML

[M01] 读取命令行参数
来源：http://blog.yfazqb.com/Article/details/gufoxbwpt.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fktsv.cn/Article/details/genwnkgbe.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/gmfcfehha.sHtML

JS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/gsdkvmxbp.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gyfdmanvr.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gtigtaoec.sHtML

Go:   os.Args[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gbebuzpin.sHtML


<!-- 参考信息 -->