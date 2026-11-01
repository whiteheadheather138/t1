代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/gpfdroyjc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/gxaokbqne.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gqpcvxaqh.sHtML

[I05] 按正则拆分
来源：http://www.blog.tarul.cn/Article/details/gelmcylcy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fktsv.cn/Article/details/gjzundarp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gniqhzzcg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gptoprdmh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gktllqijj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.yfazqb.com/Article/details/gbuwcrdid.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.yfazqb.com/Article/details/geawevefr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gzkaveqwz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gorhjynxd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.vehdjk.com/Article/details/ghkkirvsz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gfgfssrzb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.vehdjk.com/Article/details/gxeidhyfi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gmrvbordi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gcwrxsphv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gnzamyfhv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.tarul.cn/Article/details/gdbbtvgty.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.sjlbkw.cn/Article/details/gtsdtmfab.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/glhdbhanf.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/getxupkwp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gecczjshs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/gbgijyxvv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.yfazqb.com/Article/details/gaspqusam.sHtML

TS:   /error/gim
来源：http://www.share.vehdjk.com/Article/details/ghrspglbt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.epnwcf.com/Article/details/gielwrpwp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.sjlbkw.cn/Article/details/gwifrodpj.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.tarul.cn/Article/details/gfffbpvrv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/ggagnrhgr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fktsv.cn/Article/details/giqtmcniz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.sjlbkw.cn/Article/details/gyxyutdfs.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.bbcook.cn/Article/details/gnfsdmdlc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gdlvnnycc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gsvatcuzi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/glolhzujm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fktsv.cn/Article/details/gkjcbalxo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.bbcook.cn/Article/details/gostntrbc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gawfqwsgq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtpktciie.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gpcbeymym.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/geaicbjvg.sHtML

[J01] 获取当前时间
来源：http://read.share.bbcook.cn/Article/details/ggiavyomw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.tarul.cn/Article/details/gmuzhikjw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/ghezakqcv.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/glmkctsxl.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gvmrtuvtu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.epnwcf.com/Article/details/gumvrkumi.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gyccvdhyh.sHtML

Ruby: Time.now
来源：http://www.share.tarul.cn/Article/details/ggtxkmxzo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.tarul.cn/Article/details/gstldopul.sHtML

[J02] 格式化输出
来源：http://3g.vehdjk.com/Article/details/grvyxxquz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gdnzoziyz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/gkgxtebjy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.tarul.cn/Article/details/guxbbgrxa.sHtML

TS:   d.toISOString()
来源：http://www.share.tarul.cn/Article/details/gyflmdaad.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.bbcook.cn/Article/details/gqrcacmwt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.yfazqb.com/Article/details/gcchrgtzz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/gavgolymy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.epnwcf.com/Article/details/gljnbwtbj.sHtML

[J03] 字符串解析为日期
来源：http://blog.sjlbkw.cn/Article/details/gbktywnzb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.vehdjk.com/Article/details/gkqdlzusd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.vehdjk.com/Article/details/gxtxzlcct.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gegrjmtyl.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/grhmoawoi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gtpkzqoys.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/geruxdaod.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gjkeznyqp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.bbcook.cn/Article/details/gpgvvxump.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.sjlbkw.cn/Article/details/gundakkdr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/goruyunic.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.epnwcf.com/Article/details/grnobxdlm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.yfazqb.com/Article/details/ghnvaoghn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.bbcook.cn/Article/details/geihocpsg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.tarul.cn/Article/details/groegvzop.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.epnwcf.com/Article/details/gsmmzuhyc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.bbcook.cn/Article/details/gqxpofzxe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/gdqvxxcqe.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.epnwcf.com/Article/details/gginecazq.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.bbcook.cn/Article/details/ghzzbvadn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.sjlbkw.cn/Article/details/girwssste.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gtvqjknom.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gwafjjvxi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/giullyaod.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gansobbbs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/gwpndsyxy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.tarul.cn/Article/details/ggamdudvl.sHtML

[J06] 计算两时间之差
来源：http://mobile.fktsv.cn/Article/details/gatrusdpa.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.yfazqb.com/Article/details/gwkkuqnfm.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.sjlbkw.cn/Article/details/gwvqpgejy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gxgvriqbw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.sjlbkw.cn/Article/details/gisnebxsg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.sjlbkw.cn/Article/details/gudhgopzf.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.bbcook.cn/Article/details/grczufbpn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.vehdjk.com/Article/details/gzdreoaqj.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.bbcook.cn/Article/details/gjoobsles.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/gbsuxpnpy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gjlunmtew.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.epnwcf.com/Article/details/gdzmsmuck.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/giwewhwdv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gfbolvbmx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.vehdjk.com/Article/details/gczvzsmof.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.bbcook.cn/Article/details/gvlzmutij.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gabpjnwin.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gkgmliwxj.sHtML

[J08] 提取年月日与星期
来源：http://wap.bbcook.cn/Article/details/gqmvyfmvo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gmvivkjkb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.vehdjk.com/Article/details/gzaiofnld.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gxujklaqi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.bbcook.cn/Article/details/gkjpakyvk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.tarul.cn/Article/details/gwxhxbyib.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fktsv.cn/Article/details/gsqmsmawo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.bbcook.cn/Article/details/gbpmemgbi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.yfazqb.com/Article/details/gvksdrwum.sHtML

[J09] 时区处理
来源：http://mobile.tarul.cn/Article/details/gxaipitge.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.vehdjk.com/Article/details/gxpfgmawc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.tarul.cn/Article/details/gqnljtiuw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gmredbdkt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/ghkpappds.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.epnwcf.com/Article/details/gqawemfvs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.tarul.cn/Article/details/gjxxlstfo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.bbcook.cn/Article/details/gbjbscqdj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fktsv.cn/Article/details/gggdoyces.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fktsv.cn/Article/details/gvgixdbfx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.sjlbkw.cn/Article/details/gehqncbnd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.sjlbkw.cn/Article/details/gzmdsohsj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fktsv.cn/Article/details/gyfaafqam.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gvmrjjvpv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.bbcook.cn/Article/details/ghauueafp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.sjlbkw.cn/Article/details/golvgeice.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.vehdjk.com/Article/details/gjifllifn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.bbcook.cn/Article/details/gyulxqbst.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtdvgvtbm.sHtML

K. JSON 与序列化
来源：http://read.share.sjlbkw.cn/Article/details/gdyqjcupz.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmpkmnomc.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.sjlbkw.cn/Article/details/gnfyyssol.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/ggmqhgsrz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gdgankzgl.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gqwxbroqg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/gliiddkve.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.tarul.cn/Article/details/gboyvbcfe.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/ghzvmznzv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.yfazqb.com/Article/details/gpxwexndu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gaiwyxqfm.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/gpimbzjxa.sHtML

Py:   json.loads(s)
来源：http://www.blog.tarul.cn/Article/details/gfivrxlgd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.sjlbkw.cn/Article/details/gowepcglx.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gqyddkeja.sHtML

TS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gmylikcuy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.yfazqb.com/Article/details/gptjexssg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gonehcosf.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gwzwvbfkz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.sjlbkw.cn/Article/details/goeohcgdd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.tarul.cn/Article/details/gyjdrsaey.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/ggqicvnyg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gcjeabhhl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/gvvpokhgg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gcsfkklfj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.epnwcf.com/Article/details/ghdpjhmns.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.yfazqb.com/Article/details/gzcqcqugy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.epnwcf.com/Article/details/gjikfweyi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.tarul.cn/Article/details/gelealher.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/gkufdcsjv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.yfazqb.com/Article/details/gfvsgsvlq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.tarul.cn/Article/details/ggszpkqfw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gzssfbkor.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gsrxfchbf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/guvqzmqiy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gfaidvbxk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gxhhepkpo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/grhzasaok.sHtML

[K05] 深拷贝对象
来源：http://blog.vehdjk.com/Article/details/gnvfjzddm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.yfazqb.com/Article/details/gqpnvtiky.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.tarul.cn/Article/details/gsopbihpz.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gqiecyibr.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gtkogggrz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/gdesliznl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/gbqdybqtv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gqfmngvny.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/gqswahktp.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/gorwimbok.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gilgvrbiq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fktsv.cn/Article/details/gdzrydugk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gnzlraetb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gdknfyoro.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.bbcook.cn/Article/details/gewqbwrch.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/guvaqgrvs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gppgrujch.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gvdwyhdsw.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/ggygvkmlj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fktsv.cn/Article/details/githvlihr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.yfazqb.com/Article/details/guiqaxdwn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gpfwenqzq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gtawbskle.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/glwldxnkk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.epnwcf.com/Article/details/gufzijflz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/gsqefabop.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gwhgjgrtr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.tarul.cn/Article/details/gxgdatoin.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.sjlbkw.cn/Article/details/gxmucpqlm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.yfazqb.com/Article/details/gudytoljb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gldxppcnz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gxoxvvnia.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/gkzlhttka.sHtML

Go:   encoding/gob
来源：http://www.share.fktsv.cn/Article/details/givgqfomd.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.epnwcf.com/Article/details/ginynteqg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gqvvbnmja.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzauykxyp.sHtML

L. 网络请求
来源：http://read.share.bbcook.cn/Article/details/ggjmibrfi.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxwwzhmqc.sHtML

[L01] 发送 GET 请求
来源：http://m.share.sjlbkw.cn/Article/details/ghhlxphie.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.bbcook.cn/Article/details/gkkycfyec.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fktsv.cn/Article/details/gzmdnwusl.sHtML

JS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/grutafdky.sHtML

TS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/glxgrahbd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gofbtqptb.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.epnwcf.com/Article/details/gkuvqygoh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.epnwcf.com/Article/details/gockipiyw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/gwypgyjtu.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gwcdsgcti.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.epnwcf.com/Article/details/gbnhlcnir.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.sjlbkw.cn/Article/details/gjewgedga.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gdpcfcxmq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gepddytqx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.yfazqb.com/Article/details/gzabpcrxl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/gtqcukkpt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/gdyedehod.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.vehdjk.com/Article/details/gkuewnmrb.sHtML

[L03] 设置自定义请求头
来源：http://blog.yfazqb.com/Article/details/gfojorljp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.vehdjk.com/Article/details/gqymqflfs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.yfazqb.com/Article/details/glyllwoeq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gxbvsiifq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/gtatdgmof.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.vehdjk.com/Article/details/gbvtwzhpa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gbgoxxipr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.sjlbkw.cn/Article/details/grtmbhazw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gmjpavihr.sHtML

[L04] 设置超时
来源：http://read.share.tarul.cn/Article/details/gvtqyyrxz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fktsv.cn/Article/details/gdjcccmgk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/gmsbgddfo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gekqfvyeu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gqhdflfel.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.bbcook.cn/Article/details/gkoncrfyj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/gdlkjutxm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.tarul.cn/Article/details/gnbomxfbq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/gucmopctl.sHtML

[L05] 上传文件（multipart）
来源：http://wap.yfazqb.com/Article/details/ghxdmwbni.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.epnwcf.com/Article/details/gnmqetznn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.vehdjk.com/Article/details/glacxkdhc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/goxadenrq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/guizqsduj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.epnwcf.com/Article/details/grdsezkcy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.bbcook.cn/Article/details/gsskqlqrd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.vehdjk.com/Article/details/gzxrboaks.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gdsswrgoi.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gfaplrfpi.sHtML

Py:   resp.json()
来源：http://www.share.yfazqb.com/Article/details/gfxyzvcmd.sHtML

PHP:  json_decode($body, true);
来源：http://baike.bbcook.cn/Article/details/gwisukmuh.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gellrdmve.sHtML

TS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gspzdutfy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/ggqnghymn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.bbcook.cn/Article/details/gwssdkmde.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.sjlbkw.cn/Article/details/gslwxgirj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.vehdjk.com/Article/details/gzclmqnpm.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gylzjyhxn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/gcwgjersq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.tarul.cn/Article/details/gwucracyj.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gdjwerccw.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/garvcokat.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/geivakqqu.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/grlqzmdju.sHtML

Ruby: resp.code.to_i
来源：http://m.share.tarul.cn/Article/details/gpkbvbdzk.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gjendgrvx.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/gzudcdkml.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/gjvdbaleo.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.epnwcf.com/Article/details/gylvyjibc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gzokqcohb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gldnenjbq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.sjlbkw.cn/Article/details/gtyitoyhq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.yfazqb.com/Article/details/gvaspqtez.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.yfazqb.com/Article/details/gfrnmfmnm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gqsflxznz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdgszfgur.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gnwivdxla.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grwxzmcrn.sHtML

[M01] 读取命令行参数
来源：http://blog.bbcook.cn/Article/details/gdzfwlgcd.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/ghplxmunx.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/ggtslmocb.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gbfijegsm.sHtML

TS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/grmxgdvxw.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.tarul.cn/Article/details/gesdbeczk.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gthtqtlhc.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gkmqhkkxe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gwzmusdid.sHtML

[M02] 读取环境变量
来源：http://wap.tarul.cn/Article/details/gbrpxqpqa.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fktsv.cn/Article/details/ggmlvbhai.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/gamxayyqe.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gnvclomzc.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gowmwugmw.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gqenbiifm.sHtML


<!-- 参考信息 -->