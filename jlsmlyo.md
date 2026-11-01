代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/ggbobqvyv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gtbjeakjo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.sjlbkw.cn/Article/details/gysyicksp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/gupktgihq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gxknvoqbn.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.yfazqb.com/Article/details/gkvnezklj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fktsv.cn/Article/details/gtilgizdg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gnlukqgdr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/gbylbakrh.sHtML

TS:   /error/gim
来源：http://m.share.sjlbkw.cn/Article/details/gowhdgmbh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.sjlbkw.cn/Article/details/gkgcjythg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.vehdjk.com/Article/details/gcqwwnnjd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.yfazqb.com/Article/details/gcjxwhoqk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.tarul.cn/Article/details/gomdugawd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fktsv.cn/Article/details/gktoyfurq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.vehdjk.com/Article/details/ghdoifoba.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.yfazqb.com/Article/details/gjtavfaym.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gwhpajysh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/gclbavrgm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/gmsmcuppj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/gziravdiu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fktsv.cn/Article/details/gdurpwycu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gybwpsyie.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmuykeqyn.sHtML

J. 日期与时间
来源：http://www.blog.sjlbkw.cn/Article/details/gndlktutx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfcefwrgv.sHtML

[J01] 获取当前时间
来源：http://m.share.fktsv.cn/Article/details/gtbxkxtcl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.yfazqb.com/Article/details/gdlmihzqf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/goiflzinv.sHtML

JS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/grzwxfxpu.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gztmxfldw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.yfazqb.com/Article/details/gzfufthcx.sHtML

Go:   time.Now()
来源：http://blog.sjlbkw.cn/Article/details/gqqpdzfqe.sHtML

Ruby: Time.now
来源：http://baike.epnwcf.com/Article/details/gqgyferpg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fktsv.cn/Article/details/ggeamrkwg.sHtML

[J02] 格式化输出
来源：http://baike.tarul.cn/Article/details/gwjxgqxow.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gmdhdllzs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/gplrbhggv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.yfazqb.com/Article/details/gxymuzlxy.sHtML

TS:   d.toISOString()
来源：http://www.m.share.yfazqb.com/Article/details/gxggtmlta.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.epnwcf.com/Article/details/gviwupcmf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.tarul.cn/Article/details/guafcocip.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gghglzhys.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fktsv.cn/Article/details/gkgpbouqd.sHtML

[J03] 字符串解析为日期
来源：http://www.share.epnwcf.com/Article/details/gywkwquoe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.epnwcf.com/Article/details/gydviuodx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.bbcook.cn/Article/details/gsllmpvcy.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gpqmxgofw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gvxxferns.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gitlolleu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gzrnbtedn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgayziqi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/ggxsaweek.sHtML

[J04] 时间戳与日期互转
来源：http://baike.vehdjk.com/Article/details/gxiwlqepx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.bbcook.cn/Article/details/ghybiihdx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.yfazqb.com/Article/details/gzfxvagpk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gjzxvpkuw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gavtqvdzb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.epnwcf.com/Article/details/gihhnovks.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.vehdjk.com/Article/details/gbzntuveu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.tarul.cn/Article/details/gayhqsabh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.bbcook.cn/Article/details/gvtlijpua.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fktsv.cn/Article/details/gtoxqbkjy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.bbcook.cn/Article/details/gepskbkqk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.tarul.cn/Article/details/gwecgztkt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/ggctsefxu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/glubfkprp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.tarul.cn/Article/details/gigjyuxqt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gfxisnorc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.yfazqb.com/Article/details/geybqlyao.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.yfazqb.com/Article/details/gwqrdlhcr.sHtML

[J06] 计算两时间之差
来源：http://blog.sjlbkw.cn/Article/details/grdyekzdq.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.yfazqb.com/Article/details/gzsxwdwdk.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/ggcnolxag.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.sjlbkw.cn/Article/details/gmkrntskb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.sjlbkw.cn/Article/details/gmegfjcic.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/gspixmmxd.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gjqffjliq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.sjlbkw.cn/Article/details/gsnljjopo.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.vehdjk.com/Article/details/gpvajtvjv.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/gvnjrtrcd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gtlcvecoz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.sjlbkw.cn/Article/details/giivgtdmf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gwvwouukb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/goqfcplmp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.epnwcf.com/Article/details/gaamwsoav.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gjbongiox.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gjqcirhyt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gvwidydif.sHtML

[J08] 提取年月日与星期
来源：http://blog.vehdjk.com/Article/details/gmgpzeayy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.sjlbkw.cn/Article/details/gspchphwj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.sjlbkw.cn/Article/details/gzifyoago.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fktsv.cn/Article/details/gcjmlrkoe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fktsv.cn/Article/details/gyejwrdbs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.epnwcf.com/Article/details/gonjvwtwk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.yfazqb.com/Article/details/gavzfkier.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.yfazqb.com/Article/details/gqtmvvbcp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/gyxlebwyl.sHtML

[J09] 时区处理
来源：http://blog.epnwcf.com/Article/details/gcljfqomu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/gamyuihrv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.bbcook.cn/Article/details/gpmylymvv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gvpksokhw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gpjctavql.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.tarul.cn/Article/details/guvjqgheg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.yfazqb.com/Article/details/gyfmruonj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gqobuwyvf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fktsv.cn/Article/details/gdzfknrnt.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/gdtihdoyx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.epnwcf.com/Article/details/glgboyxve.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.epnwcf.com/Article/details/grchpwcbg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.yfazqb.com/Article/details/gmujdeftl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gdjytfmaq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.vehdjk.com/Article/details/gkinsdxtd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.vehdjk.com/Article/details/gkjvjchrc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.yfazqb.com/Article/details/gdpjkfoqj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.epnwcf.com/Article/details/grosyihaz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtwwitnpj.sHtML

K. JSON 与序列化
来源：http://3g.bbcook.cn/Article/details/gdfhklsxj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gngodpkxt.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/ghfkidiyy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gldnzzjye.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gnfazglvt.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gevxoeclo.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gwkcuwubv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.tarul.cn/Article/details/gtcolngly.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/gppeilohn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/gpbvhjwan.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.vehdjk.com/Article/details/ggnyulnqn.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fktsv.cn/Article/details/gytynbodl.sHtML

Py:   json.loads(s)
来源：http://www.blog.yfazqb.com/Article/details/gscpazcwt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gvsgojdfg.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/grbwmgocd.sHtML

TS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gzvfzrxhy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.yfazqb.com/Article/details/gfafvfbkh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/giaprikii.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gtebuqfth.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.epnwcf.com/Article/details/goksuqvps.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.vehdjk.com/Article/details/gtwafhuqq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/gmeslfdhh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gwnuclzdv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gscfxynbs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gaymwkfhc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.vehdjk.com/Article/details/gijuuzjmo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.yfazqb.com/Article/details/gnaqznysu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.epnwcf.com/Article/details/gusshixwi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.sjlbkw.cn/Article/details/gckdqqagk.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gqazoiefx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/grchnuvhy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.sjlbkw.cn/Article/details/gdkwrhfnv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gfzcthmdk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gkjdfvcie.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gqcdgkizt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gfddgxncm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gujqezmrl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gpjndlaih.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gysuywobp.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.yfazqb.com/Article/details/gfnbrxccc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/gsuxcbvak.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmaglthpo.sHtML

TS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gjlgmxizb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/gaybobucp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fktsv.cn/Article/details/gchgvzaem.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fktsv.cn/Article/details/gciucveaq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/gklsftjgo.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fktsv.cn/Article/details/gruwbughh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gtzbqyzwx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fktsv.cn/Article/details/gxrnvaxfd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqxlmakq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gysidlfyy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.vehdjk.com/Article/details/goorqyfmn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gtpbwygyd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gpqevpbqp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gknbfderp.sHtML

[K07] 进制转换
来源：http://blog.sjlbkw.cn/Article/details/gbowbhviy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.tarul.cn/Article/details/giajyhsnr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.sjlbkw.cn/Article/details/gvipaofdz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gfxttmyza.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gixsicief.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gcgxhhsuh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/gekqjihvp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.sjlbkw.cn/Article/details/ghjmpjves.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gvimturlj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.bbcook.cn/Article/details/gqhlgzlfh.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/goubtycys.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.epnwcf.com/Article/details/gltfsyyxe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/ggnvhdpmq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gfxoeflxn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fktsv.cn/Article/details/gipoukrpl.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/gjsbrhjzp.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.vehdjk.com/Article/details/giuusksoo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gqkopmdgp.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkysucpoy.sHtML

L. 网络请求
来源：http://www.blog.epnwcf.com/Article/details/gmrpwveca.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gcrbjqlbq.sHtML

[L01] 发送 GET 请求
来源：http://blog.sjlbkw.cn/Article/details/gmglohimh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.tarul.cn/Article/details/gnnaqdzbf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.yfazqb.com/Article/details/gsjficvgd.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gxljqdauz.sHtML

TS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/gzrbryauu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.vehdjk.com/Article/details/gstxtanpw.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.sjlbkw.cn/Article/details/gkmegvjfk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.sjlbkw.cn/Article/details/guwmuwodp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.yfazqb.com/Article/details/gyaptibrr.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gahqskbhq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gfbllwffp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.sjlbkw.cn/Article/details/gnmpyjcex.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gkkcmmrcf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/geuotewlw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.vehdjk.com/Article/details/guxylrooq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.vehdjk.com/Article/details/gmvyhofqb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.bbcook.cn/Article/details/gngsivarm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.bbcook.cn/Article/details/gzkdbpkxp.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.sjlbkw.cn/Article/details/goaspqwvw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gllqagbun.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fktsv.cn/Article/details/gaiwjxssy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gwgiqqspx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/guwjardte.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fktsv.cn/Article/details/gblmvyljd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gxptfxtxt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fktsv.cn/Article/details/grrrpgvdd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/gogcmthtg.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/gxevtxodr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.sjlbkw.cn/Article/details/garcflunh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gtvwmlaya.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gvuziqbqh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gkjewllok.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.bbcook.cn/Article/details/gpxbgvzpm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.bbcook.cn/Article/details/gxzkehpue.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fktsv.cn/Article/details/ggxrxarjm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fktsv.cn/Article/details/gjajxxzqk.sHtML

[L05] 上传文件（multipart）
来源：http://3g.sjlbkw.cn/Article/details/gxfdzccdf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/gcjtlslzx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fktsv.cn/Article/details/gjnkvvnmd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/guuwpedut.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gqvhcnpaa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.epnwcf.com/Article/details/grkcploae.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fktsv.cn/Article/details/gbycqpnvz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.yfazqb.com/Article/details/gffgvntlp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/grodpywhz.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.yfazqb.com/Article/details/glfeksypg.sHtML

Py:   resp.json()
来源：http://wap.epnwcf.com/Article/details/gxipyarrq.sHtML

PHP:  json_decode($body, true);
来源：http://blog.vehdjk.com/Article/details/gefkwakyx.sHtML

JS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/gbmklocln.sHtML

TS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gsgidwest.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gmhpvhwwb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/gcjzsluth.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fktsv.cn/Article/details/gjfmjgyxz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gqttkidbc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/getbcokjk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fktsv.cn/Article/details/gzlqargdm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fktsv.cn/Article/details/gjauadyir.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gvjghybxw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gaukngrsa.sHtML

Java: resp.statusCode()
来源：http://3g.vehdjk.com/Article/details/gypcqrgzw.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gliqfybzt.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gzebletxa.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/getfyerbf.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.epnwcf.com/Article/details/gpscuqwir.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fktsv.cn/Article/details/gopmcfqlq.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.epnwcf.com/Article/details/govxklezo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gcpipfjbc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gozuxvktu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/gtirgdvfj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.yfazqb.com/Article/details/gxpfhzjlg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gxbuqytyh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.tarul.cn/Article/details/gkyqlcesq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gadkjmycx.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.sjlbkw.cn/Article/details/gradhzvbz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ggtmwmomu.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gnjlhcgcn.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gktrhhvlp.sHtML

PHP:  $argv;  $argc;
来源：http://3g.vehdjk.com/Article/details/gawelflbb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/ggkckksfi.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gbehdoqzs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gxqdaahgq.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/ghuwneuyo.sHtML

Ruby: ARGV
来源：http://read.share.epnwcf.com/Article/details/gazryztty.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/ghbbsnbul.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/glsxuuhrx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gfmskpawb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/gaddrhwtf.sHtML

JS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/grjawetwl.sHtML

TS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/gqeonfpum.sHtML

Java: System.getenv("HOME")
来源：http://3g.bbcook.cn/Article/details/gmyglohjh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gjiznxzpz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/guwbwscol.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gknfnqzwu.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/glqhinrat.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gkicpboxj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/gznfvedui.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gtknsglin.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/ghicthcbl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/gdjvsmydw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/gpgwwoxqm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.bbcook.cn/Article/details/gfcrctjat.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.vehdjk.com/Article/details/gbuxmizvv.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/gyhawiaon.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/glkfjgvrf.sHtML

PHP:  getcwd();
来源：http://wap.sjlbkw.cn/Article/details/gbvujcwny.sHtML

JS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gfhntyfyv.sHtML


<!-- 参考信息 -->