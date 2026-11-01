代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gisipmacr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gombaaldi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/ggfuojmnr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.epnwcf.com/Article/details/gvwdmhole.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gmfodiggj.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gxinrdbij.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.sjlbkw.cn/Article/details/gfyezfuja.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/goggdxeuj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/glkrzkxjo.sHtML

TS:   /error/gim
来源：http://mobile.yfazqb.com/Article/details/gfdnbenjd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.sjlbkw.cn/Article/details/gdyfcqkwx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fktsv.cn/Article/details/ghynfdpkx.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.bbcook.cn/Article/details/gaharihon.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/ghiiirpdr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.epnwcf.com/Article/details/gajdrbans.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.yfazqb.com/Article/details/gqxabrvvw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.epnwcf.com/Article/details/gvoilbpqe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gnsrovean.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gwimnhjno.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/gobbwcxrs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.bbcook.cn/Article/details/goykaoqbi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.sjlbkw.cn/Article/details/gjmpojuuo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gsfwrexns.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmptmizvf.sHtML

J. 日期与时间
来源：http://mobile.fktsv.cn/Article/details/ggqdizucu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqkscwfvo.sHtML

[J01] 获取当前时间
来源：http://wap.bbcook.cn/Article/details/gtksujsmn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.sjlbkw.cn/Article/details/guljrleoh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gblxarzmh.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gmtqsxdix.sHtML

TS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/gehkbibov.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/goaddqini.sHtML

Go:   time.Now()
来源：http://www.blog.sjlbkw.cn/Article/details/gvqzuxiba.sHtML

Ruby: Time.now
来源：http://mobile.bbcook.cn/Article/details/gntpgztmt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/gnjkwjgqc.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gudjbmxkh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gtgpxobsu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gflhnpdgt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/gqujmedto.sHtML

TS:   d.toISOString()
来源：http://baike.sjlbkw.cn/Article/details/gmejhgvkf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fktsv.cn/Article/details/gatmonbki.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fktsv.cn/Article/details/ggjitzxnn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gysoysftr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.bbcook.cn/Article/details/gcivumugz.sHtML

[J03] 字符串解析为日期
来源：http://3g.vehdjk.com/Article/details/gzxdsdzvd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gdkmtkvda.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/gvdmbcaoc.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gtgscpser.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gixrhnbov.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gylzegtcx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gkuzspfzo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gvvpauwbv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fktsv.cn/Article/details/geyihmvcs.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.yfazqb.com/Article/details/gvqeypzzt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.tarul.cn/Article/details/gsdhacwsn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.vehdjk.com/Article/details/gypyvgvgk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/guuzicwsg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.sjlbkw.cn/Article/details/givqamnyr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.bbcook.cn/Article/details/ghqljohtu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.bbcook.cn/Article/details/gbzilezzv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.yfazqb.com/Article/details/gyxchgtdn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.tarul.cn/Article/details/gogjkfhuw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.sjlbkw.cn/Article/details/gklvzlmth.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.bbcook.cn/Article/details/gnjzsflgs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fktsv.cn/Article/details/gdijjudrq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gaoylwmjp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.bbcook.cn/Article/details/gjnmtkrdk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/gxrzswsfh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fktsv.cn/Article/details/gokplzdmi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.sjlbkw.cn/Article/details/gspxauuzj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gskswfwai.sHtML

[J06] 计算两时间之差
来源：http://m.share.fktsv.cn/Article/details/ggzmvnkfn.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fktsv.cn/Article/details/gvbqdefhb.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.yfazqb.com/Article/details/gpubldhgd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.tarul.cn/Article/details/grbihvgtj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.bbcook.cn/Article/details/gdlnruzkr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.tarul.cn/Article/details/grzdcxhvv.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fktsv.cn/Article/details/gvqsfujmq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcvreuca.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.tarul.cn/Article/details/gnxzvvhpn.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/gfdiazetv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gpracvilv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gsjaooovg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/godkolwtb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/gkmrhmpou.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.yfazqb.com/Article/details/geaxfrdxl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fktsv.cn/Article/details/gydenbzon.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gxvvqjgni.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/geejnrtsu.sHtML

[J08] 提取年月日与星期
来源：http://mobile.vehdjk.com/Article/details/gyqhkkevw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.tarul.cn/Article/details/guxpybajs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gepcqoycr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/gqsgjrove.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.vehdjk.com/Article/details/gctdrrhob.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/gjvxeginc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.bbcook.cn/Article/details/gmglmfiup.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.sjlbkw.cn/Article/details/gioidxjio.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/gsjyveviw.sHtML

[J09] 时区处理
来源：http://read.share.epnwcf.com/Article/details/gdpiejmxe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.bbcook.cn/Article/details/gaurfudoz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fktsv.cn/Article/details/gpwbzpzfx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gerfzijaq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gyzdlniaw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gmdgbtwwg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/glihvyqif.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyddjrwga.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fktsv.cn/Article/details/grbsgeszk.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.vehdjk.com/Article/details/gttpacnaz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/gobsexiqc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.tarul.cn/Article/details/glmwdgfhs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/guwutrdwh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gnmrrmipv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.sjlbkw.cn/Article/details/gdbjsixqy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.yfazqb.com/Article/details/gpkhzooif.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.vehdjk.com/Article/details/gilhuwhhq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.tarul.cn/Article/details/gzwcrlvyr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grpupfovz.sHtML

K. JSON 与序列化
来源：http://www.blog.fktsv.cn/Article/details/gitqzuqyi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzdxrcizv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.yfazqb.com/Article/details/galzxxrrv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gcypkonbq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/ghcaqlnqt.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gjbtssksi.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/gpursajuj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/gbktyhwpx.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.epnwcf.com/Article/details/gkzzdzfea.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.tarul.cn/Article/details/gqkbvkzhq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.epnwcf.com/Article/details/gltnctxib.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.yfazqb.com/Article/details/gmbojcgcz.sHtML

Py:   json.loads(s)
来源：http://read.share.fktsv.cn/Article/details/gixdyzqql.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.tarul.cn/Article/details/gbattrbwm.sHtML

JS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gkwbggxgi.sHtML

TS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gwfvbziix.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gqyippjfg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/gfdxsywmg.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gbkyxyvua.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.bbcook.cn/Article/details/gqovodzbg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.tarul.cn/Article/details/gkmxdmewa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gvokimqps.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gaqikufcb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gvwtsvtjx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gbknfnrbl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.epnwcf.com/Article/details/grkrxeuir.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.bbcook.cn/Article/details/gfcmybyov.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fktsv.cn/Article/details/gqudhczrm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/gblgpumwz.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/ggatdzojn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gbwoqyqpw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.sjlbkw.cn/Article/details/guwkbjfjg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gvvyamroi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/geqoozcqw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.yfazqb.com/Article/details/gxuiqpklo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gjnzqjfxa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.bbcook.cn/Article/details/gttoelywr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gjwrsoihu.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gsycybxus.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.tarul.cn/Article/details/ghcwqcjzb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/gvhkzjmlg.sHtML

JS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gxqdihcfs.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/guxzgtxnp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.sjlbkw.cn/Article/details/grikfadzi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.yfazqb.com/Article/details/gamzyttxd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fktsv.cn/Article/details/gtghkexrn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.sjlbkw.cn/Article/details/gvvvoejzr.sHtML

[K06] 解析 URL 查询串
来源：http://wap.sjlbkw.cn/Article/details/gghcokdkz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fktsv.cn/Article/details/gtpmuvyui.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.sjlbkw.cn/Article/details/gyjlwvdcr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/garienumq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/grjblyvvf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gdijbtmke.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gexxrnwvm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gybxpgwmr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/ghktebbaw.sHtML

[K07] 进制转换
来源：http://www.m.share.tarul.cn/Article/details/gehvvpivp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gtkcodnoj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.bbcook.cn/Article/details/gumoxzsub.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gbotskarg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gveffdhxl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gewzjtdte.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fktsv.cn/Article/details/gdoqxskyw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/gbbcrcwfa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gavqspyzz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.epnwcf.com/Article/details/glwxnizda.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/gfhotcthw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.vehdjk.com/Article/details/giiqnbdtc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gqqzetiwp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gtuqbfpwl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fktsv.cn/Article/details/gsjfqxhvz.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/gpnqwqlhp.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gpbpnhoyp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gwplnzjdf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfdhoylmk.sHtML

L. 网络请求
来源：http://mobile.bbcook.cn/Article/details/gubfdoexl.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghdhwbiwp.sHtML

[L01] 发送 GET 请求
来源：http://baike.tarul.cn/Article/details/gjzmlmwpz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.sjlbkw.cn/Article/details/gwujktaxk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/gtiqajcrk.sHtML

JS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gbkeyljrh.sHtML

TS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gzrfhmuhn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fktsv.cn/Article/details/gtnxcfafn.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/gjliujacm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/gvxtpiifw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.vehdjk.com/Article/details/gokiuyqhk.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/giolcmbbo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.epnwcf.com/Article/details/gazfufzcx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fktsv.cn/Article/details/gezkclivf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gpmhuurrt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gpnxgypsf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.yfazqb.com/Article/details/gdvjrktkw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.bbcook.cn/Article/details/gzzebjeyg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gnwkoiyji.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.vehdjk.com/Article/details/gefxexkcc.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gbgodtstq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.tarul.cn/Article/details/gnbfuljjm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.bbcook.cn/Article/details/gfpvjmcjf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gtajdbvjo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/gtnbftttg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.sjlbkw.cn/Article/details/gnvtxwvdi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gqmojepma.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/gkktddroc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gywiqfflv.sHtML

[L04] 设置超时
来源：http://3g.yfazqb.com/Article/details/gewzvlqml.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/gqtjbwdlp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.bbcook.cn/Article/details/gzdebkobo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gsrlfgnzz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gyrchemob.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/gyeysoxqc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.sjlbkw.cn/Article/details/gberfhjxw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.yfazqb.com/Article/details/gzhqcewef.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.vehdjk.com/Article/details/giinlksba.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.sjlbkw.cn/Article/details/gpedgavcp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/gzkhimaop.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fktsv.cn/Article/details/gtimqllzw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gjqgqmvvi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/gpgfgudey.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/gkrhuttyp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/gwanxeccb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.vehdjk.com/Article/details/guvyaihky.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.epnwcf.com/Article/details/goayjwivp.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gfydsoxbw.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gfztxlgtb.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gsfnsprfe.sHtML

JS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gaattguhu.sHtML

TS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/grkorfsxv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/gvbczayao.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.tarul.cn/Article/details/gwralbdtm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.sjlbkw.cn/Article/details/grqeyujpq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.bbcook.cn/Article/details/gltjuwyvw.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gxoeopzcz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/gzwucaiao.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/gxrttcfqd.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gjtntoeru.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gzeyhvdqr.sHtML

Java: resp.statusCode()
来源：http://baike.bbcook.cn/Article/details/guqcmuvsa.sHtML

Go:   resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/glkxbqtnm.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gtlipocrh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/grfixkouq.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/gkqjmkimp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.tarul.cn/Article/details/gkldnoxea.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/gfihhixhr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gdzgqiuog.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gfpweethi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gjqvtapkx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.epnwcf.com/Article/details/gcppsgoeb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.bbcook.cn/Article/details/gtrepnvuc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/gzurhgykz.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdmilgld.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.yfazqb.com/Article/details/gzbddbgpp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gzhkoikhk.sHtML

[M01] 读取命令行参数
来源：http://read.share.tarul.cn/Article/details/girlhyidw.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/ggjleslsi.sHtML

PHP:  $argv;  $argc;
来源：http://3g.epnwcf.com/Article/details/gtstncmar.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gwzlwjavg.sHtML

TS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gusehgahb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gepdbnhrv.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gdvtnccnc.sHtML

Ruby: ARGV
来源：http://3g.epnwcf.com/Article/details/gsxeetblj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gdbqooeji.sHtML

[M02] 读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gydaiyimi.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.bbcook.cn/Article/details/gbwjncabk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gqdlwyqoi.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gisebubzn.sHtML

TS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gmlezcrhz.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gnvjoablc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gfohnfrny.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fktsv.cn/Article/details/gmkvlpjia.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/ghhzyiapi.sHtML

[M03] 执行外部命令
来源：http://baike.yfazqb.com/Article/details/gmucgxbdr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fktsv.cn/Article/details/gafaleoxv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/gvswcdtul.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gmnmlkgrs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gdqhkuytw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.tarul.cn/Article/details/gopmhlzul.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.sjlbkw.cn/Article/details/gypetwehl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.yfazqb.com/Article/details/glmsymeam.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.sjlbkw.cn/Article/details/gjzipunnl.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.epnwcf.com/Article/details/girqbnbjq.sHtML

Py:   os.getcwd()
来源：http://read.share.sjlbkw.cn/Article/details/gapiijlvm.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/ghiksvfnp.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gjypaslqo.sHtML


<!-- 参考信息 -->