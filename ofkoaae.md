代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.sjlbkw.cn/Article/details/gmulmbpwm.sHtML

TS:   /error/gim
来源：http://baike.vehdjk.com/Article/details/gqiqlvrss.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/gewruqskr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fktsv.cn/Article/details/ghzmpzxom.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/gggutdxud.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.bbcook.cn/Article/details/gfoqfqsey.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.epnwcf.com/Article/details/gzsphkoqp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.vehdjk.com/Article/details/gzacsiymg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/gkrtfmofl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gimhvgwhh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gfyhxswzf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/ghzxpmead.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/gjjaxmowu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.yfazqb.com/Article/details/gallrydyc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/gwgpyojxu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/giigruwzm.sHtML

J. 日期与时间
来源：http://baike.epnwcf.com/Article/details/gvjjnzmmv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcqadwsrq.sHtML

[J01] 获取当前时间
来源：http://www.share.bbcook.cn/Article/details/gguhgjelg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.vehdjk.com/Article/details/gkgbnwsiu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/gnusoedmt.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/gdhonyowi.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gdigyjzcc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.sjlbkw.cn/Article/details/gbngpljrd.sHtML

Go:   time.Now()
来源：http://www.blog.tarul.cn/Article/details/gjwlsvauh.sHtML

Ruby: Time.now
来源：http://3g.sjlbkw.cn/Article/details/gxgnnawiy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.vehdjk.com/Article/details/gkrhxiuvu.sHtML

[J02] 格式化输出
来源：http://3g.yfazqb.com/Article/details/gwjatzgov.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/ggqcuinbb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gbigmpvza.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fktsv.cn/Article/details/gxanwnmpe.sHtML

TS:   d.toISOString()
来源：http://mobile.bbcook.cn/Article/details/goqwpfhwr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.bbcook.cn/Article/details/gtfxmcytx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.epnwcf.com/Article/details/gkoclwksx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gwoonbmip.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.vehdjk.com/Article/details/gmjiavgte.sHtML

[J03] 字符串解析为日期
来源：http://www.share.tarul.cn/Article/details/guflisaev.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.bbcook.cn/Article/details/gjzkhjhvh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.bbcook.cn/Article/details/ghhhedyyo.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gxsyvudpn.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gawjvqeic.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gyyjlaodp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.tarul.cn/Article/details/gaokbhzot.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gpyfzgvrs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.yfazqb.com/Article/details/gmrjrlbsg.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.bbcook.cn/Article/details/gdwkpsrvv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.tarul.cn/Article/details/gqtwtwmvm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fktsv.cn/Article/details/gtujwdcyj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.epnwcf.com/Article/details/gxzgjxsqy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.epnwcf.com/Article/details/gqgarorln.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fktsv.cn/Article/details/goffxrhij.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.tarul.cn/Article/details/gxxnbwvov.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gtwsrpwug.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.epnwcf.com/Article/details/glkfpfbxc.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fktsv.cn/Article/details/gtwntgxbn.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.vehdjk.com/Article/details/gfppxqlld.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.bbcook.cn/Article/details/gboolkgmc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gdnuorcel.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/gzkxizgze.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gpukptdas.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/gtrdqrhil.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.vehdjk.com/Article/details/gdjysspna.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.bbcook.cn/Article/details/gblzmljmu.sHtML

[J06] 计算两时间之差
来源：http://mobile.sjlbkw.cn/Article/details/gutmooicc.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/grgbecnmv.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gubadclbu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.vehdjk.com/Article/details/gxihfzmyl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gfyrmjjfp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.tarul.cn/Article/details/gzhurreyr.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.bbcook.cn/Article/details/gkhoucljp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.sjlbkw.cn/Article/details/grppkyzqp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.sjlbkw.cn/Article/details/gocvrbxsm.sHtML

[J07] 比较两个日期
来源：http://blog.tarul.cn/Article/details/gfqdyzlaq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gkfspplbm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fktsv.cn/Article/details/gtyjvppju.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gfpochukr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/giiecmujx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.vehdjk.com/Article/details/gymndomcj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.epnwcf.com/Article/details/glwwqiwbc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/goieihppw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gpzujdjur.sHtML

[J08] 提取年月日与星期
来源：http://baike.epnwcf.com/Article/details/goxtprkhj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fktsv.cn/Article/details/grrwpibug.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gvdmzuprq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/gbrxtfxne.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.epnwcf.com/Article/details/gwobftbkp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.sjlbkw.cn/Article/details/giqqgfylm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.epnwcf.com/Article/details/gsbzrxaiq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/gbbichwwg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.vehdjk.com/Article/details/gzdjqrgcd.sHtML

[J09] 时区处理
来源：http://blog.fktsv.cn/Article/details/gkobrpxnv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.bbcook.cn/Article/details/gvvdhrmfs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.bbcook.cn/Article/details/gyeocupae.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gzkcsegrm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gknoyeafi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.bbcook.cn/Article/details/gzupppwvm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.epnwcf.com/Article/details/gymvbfizq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/gfievpvhd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.bbcook.cn/Article/details/glilafane.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.vehdjk.com/Article/details/gsocmgeib.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fktsv.cn/Article/details/ghixyweof.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gsvqpgaib.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.epnwcf.com/Article/details/gxhulviky.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmolkultb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fktsv.cn/Article/details/gckkivzqr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.tarul.cn/Article/details/gsvimozgg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.vehdjk.com/Article/details/gnjzmmovb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gngnlljdz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gyotlayoj.sHtML

K. JSON 与序列化
来源：http://www.m.share.vehdjk.com/Article/details/gdbezfrpp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcnaajyqg.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/gqricwyba.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gkdpmjphd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/glimdatwy.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/gtzntajdv.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/gywybrooi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.epnwcf.com/Article/details/gcxkbovdr.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gkyvueiac.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.epnwcf.com/Article/details/gcrfxuwko.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.bbcook.cn/Article/details/gcjkyvzgx.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gtlguchmb.sHtML

Py:   json.loads(s)
来源：http://read.share.epnwcf.com/Article/details/gdumtrjwb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/gxmxcdyvy.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gkeuvggkn.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gzqymvamz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gpmjbagkw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gatzbcmea.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gicyqjrus.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/gepnwymiv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/gddewgljw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/greugrwuu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/gsrieowhr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gbflpbajk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/gnizymjat.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.tarul.cn/Article/details/gdjzjvvwr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/gerocscwh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gsfdojjen.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.epnwcf.com/Article/details/gijclcclk.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.sjlbkw.cn/Article/details/glhcknqvz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.tarul.cn/Article/details/gidtlwrpe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.bbcook.cn/Article/details/gmgogwuro.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gkywyhcds.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/grxyqokne.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.yfazqb.com/Article/details/gfjqoilqz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/grydyjcnu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gcitztdyg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gitmkiqxy.sHtML

[K05] 深拷贝对象
来源：http://www.share.vehdjk.com/Article/details/gofjjtors.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gtbhrlawt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.tarul.cn/Article/details/gcytcolws.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gasbydjic.sHtML

TS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gwngutrvg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fktsv.cn/Article/details/gkiobxufl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.yfazqb.com/Article/details/gfmqvinjr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/gfmbdyfdu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.yfazqb.com/Article/details/gdabvjawj.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyhpvpjb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fktsv.cn/Article/details/gaoycpmrt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.epnwcf.com/Article/details/gwbsubcvo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gulgbicom.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/ghrskmzvf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.bbcook.cn/Article/details/gpnslufwr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/ggfqaebkh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gruslzhfc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gfpmzgloc.sHtML

[K07] 进制转换
来源：http://m.share.bbcook.cn/Article/details/ghxvznnja.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gixwefrdm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/gzjuuwubq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gsfqtyfcr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gqhuxydqp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/ggewvezzp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.bbcook.cn/Article/details/gsqkdvxhv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.sjlbkw.cn/Article/details/glwyvwgeg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gqkjwrphz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.vehdjk.com/Article/details/gkrbthchg.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/gqnbxzcjk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.bbcook.cn/Article/details/gphlnjomo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gpviymxao.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/ghvehqwlv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fktsv.cn/Article/details/gglkwltvp.sHtML

Go:   encoding/gob
来源：http://3g.sjlbkw.cn/Article/details/ghtytckwe.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.bbcook.cn/Article/details/gjjmjdxfk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gxrnsdflt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gcbwiwitq.sHtML

L. 网络请求
来源：http://www.m.share.epnwcf.com/Article/details/gxhzggurj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxssmocuf.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fktsv.cn/Article/details/gsjbcmmvy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gjncxvzbo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gzgokrvzh.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gbaiscslr.sHtML

TS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gqmjfmqdw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.sjlbkw.cn/Article/details/gfmwvvfzk.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.epnwcf.com/Article/details/gsrswloum.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.yfazqb.com/Article/details/gdjjcihnu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/gnikcjtwg.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/gqxbymcyj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gzzocmzxt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fktsv.cn/Article/details/gkevemkso.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gocntzppk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gwzjzjuho.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.sjlbkw.cn/Article/details/gnjtfmrfn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.vehdjk.com/Article/details/gzivxfdey.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.vehdjk.com/Article/details/gsckomget.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gruluhnql.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fktsv.cn/Article/details/gldlsnggd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/gidljgjsu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.bbcook.cn/Article/details/gyzimerwg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/grvziorfw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/ghghcyotf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.yfazqb.com/Article/details/gpjcrkhsm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gorwhxnlb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.sjlbkw.cn/Article/details/grrtfzdkp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/glgfjbxqe.sHtML

[L04] 设置超时
来源：http://baike.vehdjk.com/Article/details/gercpxzct.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.yfazqb.com/Article/details/gxpferjli.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fktsv.cn/Article/details/gvggtrnku.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/guwejfvqd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gnrroucce.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.vehdjk.com/Article/details/gmyshehsi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gtbwbjzqq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.bbcook.cn/Article/details/gswwrasar.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.vehdjk.com/Article/details/gmqzwcajz.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/grbaawwjk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/gpqazknkl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/glqlpsqhn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gwdzblsxq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/griudpndm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.bbcook.cn/Article/details/gzsollfnc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.bbcook.cn/Article/details/goebiceld.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.sjlbkw.cn/Article/details/ggkuganjg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fktsv.cn/Article/details/godzyeqfv.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/gdtqpkqkk.sHtML

Py:   resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/ggdjklhub.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.sjlbkw.cn/Article/details/gkpfrjwrm.sHtML

JS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlmfvwxr.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gjgnthusc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.tarul.cn/Article/details/gslebejga.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.bbcook.cn/Article/details/gvdagerbl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fktsv.cn/Article/details/gonigicus.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gtxapmpoq.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/geethtvxh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.bbcook.cn/Article/details/gvebfieff.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/ggrbpxmhj.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gumgbqjds.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gvofkmplw.sHtML

Java: resp.statusCode()
来源：http://m.share.epnwcf.com/Article/details/gzhdrggrw.sHtML

Go:   resp.StatusCode
来源：http://blog.tarul.cn/Article/details/ghiemipev.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.bbcook.cn/Article/details/giyqzszvq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfhxvvig.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/gecqtrwqo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.epnwcf.com/Article/details/gsdwqlchi.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.tarul.cn/Article/details/gqsmdjjcp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gawifqlkw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gnnysicaw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.sjlbkw.cn/Article/details/gjfbdbqda.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.bbcook.cn/Article/details/ghqeckaom.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.yfazqb.com/Article/details/ggzmqkiyl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fktsv.cn/Article/details/gleelwctv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsujpnnim.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.sjlbkw.cn/Article/details/gonxjmbfe.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gicchnzfi.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/goiozbheb.sHtML

Py:   sys.argv[1:]
来源：http://mobile.yfazqb.com/Article/details/gdasnzgde.sHtML

PHP:  $argv;  $argc;
来源：http://3g.tarul.cn/Article/details/ginditnne.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gwmrgmlfn.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/glvysalti.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/getjulpfw.sHtML

Go:   os.Args[1:]
来源：http://mobile.bbcook.cn/Article/details/gxvtwifuw.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gsvxwizso.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gbfdwwqar.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gbitzvykm.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.epnwcf.com/Article/details/grnovkriq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gjtxkqqze.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gothnzigc.sHtML

TS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gmoqfvgfh.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/guhudqoqf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gzhrvfevz.sHtML

Ruby: ENV["HOME"]
来源：http://wap.epnwcf.com/Article/details/gxtsfdmvp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gvvahxoda.sHtML

[M03] 执行外部命令
来源：http://m.share.bbcook.cn/Article/details/gxgqucgny.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.vehdjk.com/Article/details/gidaccxhh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fktsv.cn/Article/details/gjzfezekk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/ganxhwpxy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gnelwtrax.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gzolumxrg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.tarul.cn/Article/details/ggcthavqm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.epnwcf.com/Article/details/geuvxfihn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.sjlbkw.cn/Article/details/gntketdqg.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjuztpzt.sHtML

Py:   os.getcwd()
来源：http://www.m.share.tarul.cn/Article/details/gzmccjbrj.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gzzdtgkcc.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gxehvkfdp.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gxyhsvyko.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/gahmgdyvy.sHtML

Go:   os.Getwd()
来源：http://www.blog.vehdjk.com/Article/details/gjsanljhe.sHtML

Ruby: Dir.pwd
来源：http://read.share.tarul.cn/Article/details/gzugkcuxh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.vehdjk.com/Article/details/giimybupb.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/glxrmzbby.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/gmcojobdq.sHtML

PHP:  exit(1);
来源：http://www.share.sjlbkw.cn/Article/details/gzrpvitfi.sHtML


<!-- 参考信息 -->