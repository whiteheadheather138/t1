代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.yfazqb.com/Article/details/gkmteanrn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gnllhghqm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.vehdjk.com/Article/details/gvpwfrknb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gfswjrefp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhgalrxf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gqkcdwafv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.tarul.cn/Article/details/greulmnjg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.yfazqb.com/Article/details/glrfcnyha.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gnomxills.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.sjlbkw.cn/Article/details/grhqmfltd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.tarul.cn/Article/details/gwjlmshbs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/gekkmyjps.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/gvgltudlq.sHtML

TS:   /error/gim
来源：http://wap.yfazqb.com/Article/details/gzdsyscfv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.vehdjk.com/Article/details/ghnxczmge.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.bbcook.cn/Article/details/gqoszgrja.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.epnwcf.com/Article/details/gyfgcihbp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.epnwcf.com/Article/details/grdxlbdbu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.bbcook.cn/Article/details/ggjgyldhr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.epnwcf.com/Article/details/galyxamdd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gvvftiswi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/ggwztojsq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gkuexgjwl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gfbmwokdc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.sjlbkw.cn/Article/details/grgbthzwt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.vehdjk.com/Article/details/gcetujclf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.tarul.cn/Article/details/gprutrdiw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmminuxin.sHtML

J. 日期与时间
来源：http://3g.epnwcf.com/Article/details/ggslqjiup.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbozftaid.sHtML

[J01] 获取当前时间
来源：http://baike.epnwcf.com/Article/details/gaplgoswd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.yfazqb.com/Article/details/guyvnthjj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/gqqgnulva.sHtML

JS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/gghgzmgba.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/gnsokpyqi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.tarul.cn/Article/details/grmmlpnjy.sHtML

Go:   time.Now()
来源：http://m.share.vehdjk.com/Article/details/ggavkounv.sHtML

Ruby: Time.now
来源：http://baike.bbcook.cn/Article/details/gprxvyidp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.yfazqb.com/Article/details/gkzziljyn.sHtML

[J02] 格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gjsrlnlcv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/gpadmpool.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gayuxyjls.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/gulrucamg.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fktsv.cn/Article/details/garxsooqv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.bbcook.cn/Article/details/gvmchsgji.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.vehdjk.com/Article/details/gzhohkujr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gjwsascfa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.vehdjk.com/Article/details/grlyfffwk.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/gourgjkwx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.yfazqb.com/Article/details/gytsagnnn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/gewgwrivt.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/geqcxlzyi.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/ggtwwipae.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gjladxbgb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/golrfhapu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/glodwplem.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.epnwcf.com/Article/details/gcgbgwnyr.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fktsv.cn/Article/details/gjuozxwwu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/geemrnfom.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/gdgxvfnzs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.bbcook.cn/Article/details/gztqmbsde.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gulxcsell.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.epnwcf.com/Article/details/gyhnumkyh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.yfazqb.com/Article/details/gjezvspaq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/gyibiarev.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.epnwcf.com/Article/details/ghzrcuela.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.epnwcf.com/Article/details/gclqawxpm.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/gkkbnvwvv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.tarul.cn/Article/details/geiilcgid.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gbvjpvtcr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gyckjzhrh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gzxsdddcu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.yfazqb.com/Article/details/glyilapvz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.vehdjk.com/Article/details/gamjabljq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/gananwiea.sHtML

[J06] 计算两时间之差
来源：http://baike.tarul.cn/Article/details/gyvxmxzym.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/gwcuzrkuk.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gucpioyux.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.tarul.cn/Article/details/gzruxssqc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.bbcook.cn/Article/details/gazbwbwsz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.vehdjk.com/Article/details/gkyklvxsi.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fktsv.cn/Article/details/glwgqfwjl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/gxlzhxmro.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/gutiblksy.sHtML

[J07] 比较两个日期
来源：http://read.share.vehdjk.com/Article/details/gxqfklwue.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gvdkhegxc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.epnwcf.com/Article/details/gfqmzagva.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gbhbzlmxb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gzmmxafdt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fktsv.cn/Article/details/ganmlbdxn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.bbcook.cn/Article/details/gwqnmvnws.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gyhiswovb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/grqesxniu.sHtML

[J08] 提取年月日与星期
来源：http://blog.epnwcf.com/Article/details/gmzcaiyfm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fktsv.cn/Article/details/gnfcycjlk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.sjlbkw.cn/Article/details/gketcngqh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/gntpfwnrc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.yfazqb.com/Article/details/gqubwpoge.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.yfazqb.com/Article/details/gzaflnquj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.yfazqb.com/Article/details/grdgxvcyy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.vehdjk.com/Article/details/gvmbicqtj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.epnwcf.com/Article/details/gwiydrizn.sHtML

[J09] 时区处理
来源：http://m.share.bbcook.cn/Article/details/grqeahgvk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/gflsbprsz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.epnwcf.com/Article/details/gzvdluqsx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gchinegpk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gojfedbqa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.tarul.cn/Article/details/gcvuyjhjs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.sjlbkw.cn/Article/details/giniptdse.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fktsv.cn/Article/details/gkebwzlub.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/gdkbdugbw.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/gxpujuuuv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.yfazqb.com/Article/details/gdwslbuiu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.epnwcf.com/Article/details/guhmxuhoy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.epnwcf.com/Article/details/gucrzqdrf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.epnwcf.com/Article/details/gexoaotim.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.tarul.cn/Article/details/gdxwubjyj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.bbcook.cn/Article/details/gwcjuxuvw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fktsv.cn/Article/details/gajvtzmlu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/gxhquecer.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfvcxcfts.sHtML

K. JSON 与序列化
来源：http://read.share.sjlbkw.cn/Article/details/gottvrwhp.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvwhmfauv.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.vehdjk.com/Article/details/gotmfgpsw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/glxsssnht.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/ggcarfjab.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/gmykdabgg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gnrykcbuq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/gljvknews.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fktsv.cn/Article/details/gckgefbsf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/gpkeheyml.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gzyxkeryg.sHtML

[K02] JSON 字符串转对象
来源：http://3g.yfazqb.com/Article/details/ghhqxighd.sHtML

Py:   json.loads(s)
来源：http://mobile.bbcook.cn/Article/details/gpolyaqor.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gbmamaiez.sHtML

JS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gvqdrincx.sHtML

TS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gnamfrqzn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.yfazqb.com/Article/details/gfjjsdrii.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gnaaatren.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gnmbjqoje.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.vehdjk.com/Article/details/ghxqpdgzp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/gnalcclin.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/guhoswvwy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gpysjfqvt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/gmfflminm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gkpnkdcha.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.bbcook.cn/Article/details/gbxazdgqh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/gavxncikl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.tarul.cn/Article/details/gmfrdfdnt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.yfazqb.com/Article/details/gshozpmts.sHtML

[K04] 读取 JSON 文件
来源：http://3g.vehdjk.com/Article/details/gmfhhnmgd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fktsv.cn/Article/details/gmntubdtf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/glvfhlhce.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gyyjdzjuh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gpbjffcco.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.tarul.cn/Article/details/gfotbnonm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gcjmymjlg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/giuygmetv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gjbassbuv.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/gijznppgv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fktsv.cn/Article/details/gyqaovclh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/grazawwxm.sHtML

JS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gfjehxgjz.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gmcirqzjw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.epnwcf.com/Article/details/gwyxbybke.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fktsv.cn/Article/details/gltwxnjou.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gyunmtjxf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/gjhlpfsza.sHtML

[K06] 解析 URL 查询串
来源：http://baike.yfazqb.com/Article/details/glfqleppl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gsmyqudkz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.yfazqb.com/Article/details/gbzfmlhyd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gzppbinrp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/gnzwtxtsy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.bbcook.cn/Article/details/gfsfveoba.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gvponrigy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/grdapjxhw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gbjscelsa.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gexftrljo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gpxdvnsoi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.bbcook.cn/Article/details/gabvjbcai.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gymfiulxl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gohxzouij.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gcvilqvfp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gwagpsikg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.bbcook.cn/Article/details/gwsabqgcn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gsgxeugmk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.sjlbkw.cn/Article/details/gghofvfbx.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fktsv.cn/Article/details/grffabzrt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.bbcook.cn/Article/details/gwgexnizo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gxphiwxba.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/gcotnskdg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fktsv.cn/Article/details/guycakzge.sHtML

Go:   encoding/gob
来源：http://read.share.sjlbkw.cn/Article/details/gfkbrcrcb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gwjvcgnuz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gdisiyhta.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqzhvbrzc.sHtML

L. 网络请求
来源：http://3g.vehdjk.com/Article/details/gmlusubvd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/getbncyvl.sHtML

[L01] 发送 GET 请求
来源：http://wap.tarul.cn/Article/details/gikgsuesn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/gjpedzbyu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.epnwcf.com/Article/details/gkrnfxpnk.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gkfvtpavr.sHtML

TS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/gvznpdwrg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.yfazqb.com/Article/details/gujmfhbog.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fktsv.cn/Article/details/gkqlofkqb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.sjlbkw.cn/Article/details/gtittfbtb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/gpxkprnls.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gcwnblmkq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/gnbaixvaa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.epnwcf.com/Article/details/gnvzzoply.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/geguzrecz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gbhhsjuje.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.yfazqb.com/Article/details/gbvzbroeq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gujrqxxpw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.yfazqb.com/Article/details/gebpesifc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/gwwfrckqb.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.bbcook.cn/Article/details/gareibiaj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.tarul.cn/Article/details/gbomvceiv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.yfazqb.com/Article/details/gtuqyuelo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gkoalnmok.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/gqwjheqyh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.vehdjk.com/Article/details/gpomqpbrg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gyvcsxddt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/gothxyqdq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gkwlghpag.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/giovilpvk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/gmtzonrmn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/getozpyhx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gsqgzpzdf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gloowoudw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.bbcook.cn/Article/details/gfpnnbdwx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.bbcook.cn/Article/details/giravsbjl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.tarul.cn/Article/details/gagfwsjiu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gobyqrsnv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gavjfelbg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.tarul.cn/Article/details/gpmvujmia.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/gzzwnetcs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gcrfrwnpk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gcukzhdll.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/glqmfvagh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.yfazqb.com/Article/details/gvmmnjfss.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gnkhdkzvr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.epnwcf.com/Article/details/gmibaqohz.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.tarul.cn/Article/details/gapjufquc.sHtML

Py:   resp.json()
来源：http://m.share.tarul.cn/Article/details/gexgmpwjz.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gzvreffey.sHtML

JS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/gxtoxzfrj.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gypomkpqq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.vehdjk.com/Article/details/ghbhckztn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gdokuuero.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fktsv.cn/Article/details/gpsybvtpr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fktsv.cn/Article/details/guxglhbjo.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gbijtghwr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.vehdjk.com/Article/details/gygivmcct.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.epnwcf.com/Article/details/gdnlfaxpr.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/ghwvyzpss.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gaostcmoc.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/gazdursab.sHtML

Go:   resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/ghfclewly.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/grlqvrrzr.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/grebuoqpn.sHtML

[L08] 并发请求多个地址
来源：http://read.share.sjlbkw.cn/Article/details/gyjbhtnfo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/ginltuvki.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.epnwcf.com/Article/details/gcabzrzdz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gjxddzbom.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gnlndrpkf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.bbcook.cn/Article/details/grkknxzdm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.vehdjk.com/Article/details/gyytvbqie.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/gnerjsfte.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gswnuyiws.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gamovdrjk.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gyuznqopg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdsgsfejy.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/ggjvfcxij.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gvequszut.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fktsv.cn/Article/details/geqqxphrb.sHtML

JS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/gphjukvlo.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gtqpvgciy.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/gwrtvfjeo.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gmohbhrjg.sHtML

Ruby: ARGV
来源：http://3g.epnwcf.com/Article/details/gxftuqipu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gtrdmdueb.sHtML

[M02] 读取环境变量
来源：http://baike.vehdjk.com/Article/details/gfyowfigb.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.tarul.cn/Article/details/gbujniwtn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gfvppehak.sHtML

JS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gkzkifazr.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gkhxquucq.sHtML

Java: System.getenv("HOME")
来源：http://3g.tarul.cn/Article/details/gvvtuxogf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gunfmscvd.sHtML

Ruby: ENV["HOME"]
来源：http://3g.epnwcf.com/Article/details/gcrqikici.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.tarul.cn/Article/details/gxvdshqox.sHtML

[M03] 执行外部命令
来源：http://m.share.fktsv.cn/Article/details/gymvsreob.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/gagtqgvwo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/grnkueibo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gpmvpqpnj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gmxmkhpoo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/ghlhqyghm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/gbrdnopkj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fktsv.cn/Article/details/gnxbahrtg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/gdlcscjqy.sHtML


<!-- 参考信息 -->