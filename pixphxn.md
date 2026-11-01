代发 wailian999

Ruby: s.scan(/error/i)
来源：http://wap.tarul.cn/Article/details/giaeivdfs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.epnwcf.com/Article/details/gqewguowq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.yfazqb.com/Article/details/goldxkvww.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.vehdjk.com/Article/details/gwzljckte.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gfrouektm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/gkpbyyilu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/geprqzzfz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/giuawlats.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/grssfkbas.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.tarul.cn/Article/details/gafyyfkzd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/gpehdggbq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghxorqywl.sHtML

J. 日期与时间
来源：http://www.blog.sjlbkw.cn/Article/details/ggpmpqqqu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grwpumlnp.sHtML

[J01] 获取当前时间
来源：http://3g.fktsv.cn/Article/details/gqmgpeume.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/gntbrguia.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gwsezpbub.sHtML

JS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gdbqcdlkz.sHtML

TS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gwdjgwryc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.tarul.cn/Article/details/gymfmdmdo.sHtML

Go:   time.Now()
来源：http://wap.yfazqb.com/Article/details/gkrmdqlrm.sHtML

Ruby: Time.now
来源：http://www.share.bbcook.cn/Article/details/gluzmgyvz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fktsv.cn/Article/details/gyfbjsfwd.sHtML

[J02] 格式化输出
来源：http://read.share.tarul.cn/Article/details/graazoscw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/giyrdtver.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gdwzmapro.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.vehdjk.com/Article/details/gaqkdquhr.sHtML

TS:   d.toISOString()
来源：http://baike.tarul.cn/Article/details/gpfflekmb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.tarul.cn/Article/details/gtcqvyzlj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.yfazqb.com/Article/details/gccfbuotr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gnlmfsdki.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.bbcook.cn/Article/details/gbtjcpkzf.sHtML

[J03] 字符串解析为日期
来源：http://m.share.vehdjk.com/Article/details/gdqlyapwq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.tarul.cn/Article/details/gxmbvaqvm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.tarul.cn/Article/details/gypcggixw.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gqadnfwne.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/ghkyetfle.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/guhnffyhf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gcblyosgm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/glaqrilpw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.bbcook.cn/Article/details/guyyvzmbe.sHtML

[J04] 时间戳与日期互转
来源：http://3g.tarul.cn/Article/details/gatthasuf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.epnwcf.com/Article/details/gzsygzppb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/grmqulxue.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.epnwcf.com/Article/details/gdmwrggda.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.sjlbkw.cn/Article/details/goqzptxco.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.vehdjk.com/Article/details/genhlypcv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.tarul.cn/Article/details/grxuyporu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gudksuymn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.tarul.cn/Article/details/gvdikfqda.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.sjlbkw.cn/Article/details/ggkvjfiqc.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.vehdjk.com/Article/details/glekxfkto.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/gobgvmgdm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/giqwwfgoi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/guklesctg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.tarul.cn/Article/details/gdkvsqzlq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.yfazqb.com/Article/details/gnqolfmpc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.tarul.cn/Article/details/govbfvbwv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.yfazqb.com/Article/details/gfsbyubxv.sHtML

[J06] 计算两时间之差
来源：http://m.share.bbcook.cn/Article/details/gzzllmaqn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gpwpzviua.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gtsiccdrf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.sjlbkw.cn/Article/details/gjxardwyo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fktsv.cn/Article/details/gwgyrhdtn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.yfazqb.com/Article/details/genbvhlik.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.vehdjk.com/Article/details/gjqfkvwzg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.bbcook.cn/Article/details/gaxnhzesr.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/gokutqxah.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/ggdfczfkt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gknlworkx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.epnwcf.com/Article/details/gtefpzkjv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/ggkcxpybx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gcsavmabs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.epnwcf.com/Article/details/gcvwkkwuj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gchdwlxsw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/ggmctbatz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/garpjnpfm.sHtML

[J08] 提取年月日与星期
来源：http://3g.epnwcf.com/Article/details/gvvftvszz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fktsv.cn/Article/details/gmuqviplg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/geqoovkcs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/grwczsdpe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.sjlbkw.cn/Article/details/gtwufdqaf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.sjlbkw.cn/Article/details/giibkwytx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.vehdjk.com/Article/details/gdhnfbhpz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.bbcook.cn/Article/details/ggvxrrwzs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.sjlbkw.cn/Article/details/gbtpsyowe.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/gxpagntta.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/gkroktkdi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.yfazqb.com/Article/details/gyfqkaonq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/greggqhqc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gohlcrtwp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.bbcook.cn/Article/details/gampdvzpo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.bbcook.cn/Article/details/gyscujyix.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.vehdjk.com/Article/details/giiiinsvj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/gpzxhgheb.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/ggxtifiua.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.bbcook.cn/Article/details/gxkswivxk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.bbcook.cn/Article/details/gboecgcme.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/geqaadwus.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.epnwcf.com/Article/details/gtrsijvyh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.epnwcf.com/Article/details/gfzqrlrgg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.yfazqb.com/Article/details/gyoujaaob.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.sjlbkw.cn/Article/details/gbzbpjmbb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/gzzmyhxzg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfteqkcot.sHtML

K. JSON 与序列化
来源：http://www.blog.epnwcf.com/Article/details/gcpyhkcda.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/giwkndbgo.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.sjlbkw.cn/Article/details/gxyqvwomm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/grhnegygo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gdzfdwrpb.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gxgaaitwa.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/gcoyeifct.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fktsv.cn/Article/details/gappwasqj.sHtML

Go:   json.Marshal(obj)
来源：http://3g.epnwcf.com/Article/details/ggvkknisw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.vehdjk.com/Article/details/gkudyujxj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.yfazqb.com/Article/details/gpxhhqzcj.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/gqqhguhma.sHtML

Py:   json.loads(s)
来源：http://blog.sjlbkw.cn/Article/details/gssahqryn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gkpssonri.sHtML

JS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/glzssxecg.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/ggttryvrw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.tarul.cn/Article/details/gwuaorsof.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gqajjdiad.sHtML

Ruby: JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gcnzvpkfc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.yfazqb.com/Article/details/gjehdaptz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/ghbsoemnl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.yfazqb.com/Article/details/gfwovnauq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gdzzciknz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gnuipbwty.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gtmuxltrn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/gmcafpzbq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fktsv.cn/Article/details/gcqjhitoe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/glldrgwbf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/gdwmjiqvi.sHtML

[K04] 读取 JSON 文件
来源：http://wap.vehdjk.com/Article/details/gggsqkehq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.sjlbkw.cn/Article/details/gmodrjhbl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/glzpxmwwb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gnhxtcndv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdykqpmuk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gccrrggfr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gkbbdjbtp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/gmqkjjslp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.vehdjk.com/Article/details/gwzzljdww.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwovjogs.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gdjukdstn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/gfahluant.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/grgtgrgog.sHtML

TS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gpmavygek.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/gdklplljq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gjtpyyrxg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.bbcook.cn/Article/details/gpacudetr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/gtyyspwjm.sHtML

[K06] 解析 URL 查询串
来源：http://baike.bbcook.cn/Article/details/gmdygtcvm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gjqwumyyt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.bbcook.cn/Article/details/gxdjotkec.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gbhnynifg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/glcusktts.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.yfazqb.com/Article/details/gutubbgge.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gyrqicxdd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/guvzrtuve.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/grddjftrj.sHtML

[K07] 进制转换
来源：http://mobile.tarul.cn/Article/details/gikspwiif.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/ghgxmqmsm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.bbcook.cn/Article/details/gewegqbdj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gorknatod.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gzkaqgler.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gijfigclk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.bbcook.cn/Article/details/gxxwpgjqo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.vehdjk.com/Article/details/gkhnkaeij.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.tarul.cn/Article/details/geszifoir.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fktsv.cn/Article/details/gzzgiuedo.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.yfazqb.com/Article/details/gnufslujh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/gsgadxgal.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gppgxjqka.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gqpqmrokw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.sjlbkw.cn/Article/details/gjpvnghaa.sHtML

Go:   encoding/gob
来源：http://www.blog.yfazqb.com/Article/details/ggrzxstxu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.yfazqb.com/Article/details/gixkagxif.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gnpqtgvte.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqeexsukb.sHtML

L. 网络请求
来源：http://read.share.bbcook.cn/Article/details/gwtlxvzrl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gftrvltzq.sHtML

[L01] 发送 GET 请求
来源：http://m.share.epnwcf.com/Article/details/gdvytyxvh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.yfazqb.com/Article/details/gxojmqcdm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.vehdjk.com/Article/details/ghhtflxin.sHtML

JS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/ggcajiapq.sHtML

TS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gupswnjia.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.sjlbkw.cn/Article/details/gekqlpuqn.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/giwjogdde.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/gabrzrrff.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/gjdokiewb.sHtML

[L02] 发送 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gfwxthsku.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gtxwnqzej.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/gawryoosj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gzrzswfjx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gbpeyofyw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.tarul.cn/Article/details/gknspljje.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.yfazqb.com/Article/details/gfffwihtz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.vehdjk.com/Article/details/gxtxmkmeh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.yfazqb.com/Article/details/gxdgxhovh.sHtML

[L03] 设置自定义请求头
来源：http://wap.epnwcf.com/Article/details/gpckccrqj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gniwtszbk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.bbcook.cn/Article/details/gmgaclszo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.vehdjk.com/Article/details/gljnjmgrj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gtlvgqrvo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/gtnhofmdf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/ggwkfiucn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/geutqvdcv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gtnfehcey.sHtML

[L04] 设置超时
来源：http://m.share.vehdjk.com/Article/details/gbqusftcw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.sjlbkw.cn/Article/details/gvrzvhoyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.bbcook.cn/Article/details/gnrrftmkz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gafdsbvzv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gbburxdru.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.yfazqb.com/Article/details/gvhaaoiyx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/gytjuaeju.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.tarul.cn/Article/details/gnaaicrci.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.tarul.cn/Article/details/gbumcgueo.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fktsv.cn/Article/details/gowesxnks.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.bbcook.cn/Article/details/gfxblnvng.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gzsubfqco.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gnbwtjuqx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gmzqgdfej.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.epnwcf.com/Article/details/gsuefpgki.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.yfazqb.com/Article/details/gmyricobj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.sjlbkw.cn/Article/details/glpackeca.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.epnwcf.com/Article/details/gihjyrfdr.sHtML

[L06] 解析响应为 JSON
来源：http://wap.vehdjk.com/Article/details/gbcacpltg.sHtML

Py:   resp.json()
来源：http://wap.fktsv.cn/Article/details/gchndbcqp.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.sjlbkw.cn/Article/details/glnqlaveb.sHtML

JS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gwxlbsvyi.sHtML

TS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/ggkqvkhbb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gcmhratck.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.vehdjk.com/Article/details/gpkckonhf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gnvgapzmv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/gpykjgkpq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gtdbkeqrp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/gpliezcpn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.sjlbkw.cn/Article/details/gfcrefuvx.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/ggkncrqnz.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gjpzsrtbt.sHtML

Java: resp.statusCode()
来源：http://blog.sjlbkw.cn/Article/details/glhfdhufl.sHtML

Go:   resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/ghcflxizd.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/gkthdoeep.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gofxuwnis.sHtML

[L08] 并发请求多个地址
来源：http://blog.vehdjk.com/Article/details/gabgagwxb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gqtejbaob.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fktsv.cn/Article/details/gipzpbbov.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gwhrnzlwh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gfsxzptul.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fktsv.cn/Article/details/gnmjfvjzd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.sjlbkw.cn/Article/details/gdemzdvst.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/gqybewvns.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gftupzzib.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqlpumcdg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxlrlqeb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gigmwsznt.sHtML

[M01] 读取命令行参数
来源：http://mobile.tarul.cn/Article/details/gzlbnhxig.sHtML

Py:   sys.argv[1:]
来源：http://www.share.vehdjk.com/Article/details/gxqpwvrdh.sHtML

PHP:  $argv;  $argc;
来源：http://blog.yfazqb.com/Article/details/gimeqnxhz.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gefrkxlhz.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gmgsljvao.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gjkkloxkz.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/govitirjs.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/gxkhclkto.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/glkdbxvnq.sHtML

[M02] 读取环境变量
来源：http://www.share.fktsv.cn/Article/details/gjhvmvczj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.bbcook.cn/Article/details/ggapydwmm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gclxgyqvq.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gjgekbzai.sHtML

TS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gqjtarbon.sHtML

Java: System.getenv("HOME")
来源：http://m.share.tarul.cn/Article/details/gfdwrbbgb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/guaxyarec.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/gpoorxxjl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.bbcook.cn/Article/details/gtwbxxtnk.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/gjcfdpkxu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gwgtgfmgi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gtczezauc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gkuksyycu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gjodrvyfl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.vehdjk.com/Article/details/grtttlfle.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/gaqilwkhq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gssqifxda.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gqklqvzga.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/gbffdyiqf.sHtML

Py:   os.getcwd()
来源：http://baike.sjlbkw.cn/Article/details/ghfuhfrgb.sHtML

PHP:  getcwd();
来源：http://www.share.sjlbkw.cn/Article/details/gknpjhrkt.sHtML

JS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gqmshcslg.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/grpalqszk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.bbcook.cn/Article/details/glajjjnkn.sHtML

Go:   os.Getwd()
来源：http://wap.tarul.cn/Article/details/gqqzbrycz.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.epnwcf.com/Article/details/goxzhkjvy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fktsv.cn/Article/details/gurjtvrlg.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/gjgynwwrm.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gqmxxzlvp.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/ghojpozbt.sHtML

JS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gyntkwhdv.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gynpzirta.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gyxixixht.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gegmimgug.sHtML


<!-- 参考信息 -->