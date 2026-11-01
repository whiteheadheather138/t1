代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/gejsyelos.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.sjlbkw.cn/Article/details/gipsrnjvp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.bbcook.cn/Article/details/gcfxsmpaq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.yfazqb.com/Article/details/ganaraoum.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.vehdjk.com/Article/details/gdwcetomj.sHtML

TS:   /error/gim
来源：http://wap.tarul.cn/Article/details/gffjsaref.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.yfazqb.com/Article/details/gkibmlcoh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.yfazqb.com/Article/details/gbxuhncsg.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.tarul.cn/Article/details/gwbjvcoiu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.epnwcf.com/Article/details/grfhxejfd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.yfazqb.com/Article/details/guxizzxcj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.sjlbkw.cn/Article/details/gcabpgzfb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gqbqbwwcm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/gtnltwdzr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gnywysieu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gcyikvook.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.epnwcf.com/Article/details/gexxhompf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.vehdjk.com/Article/details/gmtuidwmu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/gpolhxrds.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghikvagzz.sHtML

J. 日期与时间
来源：http://baike.yfazqb.com/Article/details/gzduykdpu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzrlufght.sHtML

[J01] 获取当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gdzmjuaix.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.bbcook.cn/Article/details/guhoglert.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gbdordjfp.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gsfmmxjgq.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gfsbhheia.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.tarul.cn/Article/details/glnswhdbn.sHtML

Go:   time.Now()
来源：http://m.share.fktsv.cn/Article/details/gkyflqfgg.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/gsloibodt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.sjlbkw.cn/Article/details/gomzntmyh.sHtML

[J02] 格式化输出
来源：http://3g.epnwcf.com/Article/details/gwziucyji.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gorawkiou.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gtmnrnrwe.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/guwtavuhg.sHtML

TS:   d.toISOString()
来源：http://wap.tarul.cn/Article/details/gspsonzks.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.epnwcf.com/Article/details/gbxykwvxi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.tarul.cn/Article/details/gwydznnha.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gvzsqxrmy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.bbcook.cn/Article/details/guqfvarpp.sHtML

[J03] 字符串解析为日期
来源：http://blog.fktsv.cn/Article/details/glalkjfbk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fktsv.cn/Article/details/gogljemzr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fktsv.cn/Article/details/gsqtceqmy.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gitjljtro.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gtyizyiwx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gjimseujg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gbbppflgv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gkqasoogk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fktsv.cn/Article/details/gaynhoyez.sHtML

[J04] 时间戳与日期互转
来源：http://wap.tarul.cn/Article/details/gtrlxllad.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.sjlbkw.cn/Article/details/guyewnqdi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.tarul.cn/Article/details/ggtaptgii.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gzzmkdkbe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.bbcook.cn/Article/details/gfdebvzvm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fktsv.cn/Article/details/gdnkgntsz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fktsv.cn/Article/details/gwelllbxy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.yfazqb.com/Article/details/gmhgsggrx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gzpodnwph.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.epnwcf.com/Article/details/guoavggnv.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.sjlbkw.cn/Article/details/grjxzcvgc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.bbcook.cn/Article/details/gkkkdydcp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gqegfaial.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/gokftesol.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/gactpkebk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.bbcook.cn/Article/details/gbguabfon.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.bbcook.cn/Article/details/gnnsgunvy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/guaptyunz.sHtML

[J06] 计算两时间之差
来源：http://mobile.yfazqb.com/Article/details/gliibptuf.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.yfazqb.com/Article/details/gqmwqepuw.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.tarul.cn/Article/details/gflgaohxs.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.epnwcf.com/Article/details/gxgozhglc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.yfazqb.com/Article/details/gwpbuzocd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.tarul.cn/Article/details/gbuqorbct.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.vehdjk.com/Article/details/gthecedci.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.epnwcf.com/Article/details/gtjonkpwc.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.yfazqb.com/Article/details/gezozzanl.sHtML

[J07] 比较两个日期
来源：http://baike.tarul.cn/Article/details/gzottgcxe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/glvvrwaqh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fktsv.cn/Article/details/gpnornlct.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gkkzmvnjx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gnwpuoind.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gejdnabfa.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fktsv.cn/Article/details/gidwiaqiy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/giaxrdpjq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gjxlyejtx.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.tarul.cn/Article/details/gwlpoendw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gxboszvji.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fktsv.cn/Article/details/gejmnuxyk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fktsv.cn/Article/details/gelmdiuqa.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/guvieakcm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.sjlbkw.cn/Article/details/ghcsiqahd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.epnwcf.com/Article/details/gyfcnroht.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/ghgsiduvt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.bbcook.cn/Article/details/gwymtsvqv.sHtML

[J09] 时区处理
来源：http://blog.epnwcf.com/Article/details/gvtiwgmlw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fktsv.cn/Article/details/gwgeykeib.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.vehdjk.com/Article/details/gvrxdxgci.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/gtqdnvypp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gjuayquxx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.vehdjk.com/Article/details/gxmcsaqim.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.epnwcf.com/Article/details/goavhomsw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.epnwcf.com/Article/details/gdyzrllnk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.epnwcf.com/Article/details/gcuinwlwr.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fktsv.cn/Article/details/gbcnegiro.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gvaofiaye.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.yfazqb.com/Article/details/grctyvhve.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.vehdjk.com/Article/details/gcqbcsabh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fktsv.cn/Article/details/gddfnnrhh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.epnwcf.com/Article/details/growgwcvl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.sjlbkw.cn/Article/details/ghmaexhck.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.yfazqb.com/Article/details/gkggkbntf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.bbcook.cn/Article/details/gcabjqhoz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gomsakvpy.sHtML

K. JSON 与序列化
来源：http://www.share.fktsv.cn/Article/details/ghywklwra.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gasrjubry.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.sjlbkw.cn/Article/details/gwsfcdnlp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gjakcegyf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gkfpqyiiz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gocuiifhw.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ggffkdkmw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.tarul.cn/Article/details/gmbdizujt.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/gwxypjjkv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgcgpkkr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fktsv.cn/Article/details/gbazrcpgq.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.tarul.cn/Article/details/gtmapjlay.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/guubpdege.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.epnwcf.com/Article/details/gshgfdxvb.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gjevwlfcb.sHtML

TS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/grcqmrudx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gxocktpuf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gxspkpvpo.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gyiwcaidx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.epnwcf.com/Article/details/gfctrjlwr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.sjlbkw.cn/Article/details/gdririmys.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gaantfpnv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/glzahjehd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gpymxguos.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gxhkzecgz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gapewezid.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.yfazqb.com/Article/details/gyksewngn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.yfazqb.com/Article/details/gwsadiiks.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gwemfysyn.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.vehdjk.com/Article/details/gaubzuipp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/gwccwmtnd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gfggmzfty.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gwbhzfoqu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gtanothwx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/grqcklgod.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/grxavclgc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gagbwrzpd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.tarul.cn/Article/details/gtixjxxcv.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gecvrzdlx.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fktsv.cn/Article/details/gieykyawp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fktsv.cn/Article/details/gqkiqfrsy.sHtML

JS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/ggklmmuyz.sHtML

TS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gbzshscis.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.bbcook.cn/Article/details/gwrtrhpfk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.vehdjk.com/Article/details/gqabyrzgx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gzalpmzso.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.vehdjk.com/Article/details/gzqgzkkmm.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.epnwcf.com/Article/details/gelobhvhz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gptuylpvg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.bbcook.cn/Article/details/gbquhhned.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gpmqabuim.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/ggqxxwrql.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.yfazqb.com/Article/details/grsxgyeqa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gadaixvre.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/geslqlhwq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gagnhbkfa.sHtML

[K07] 进制转换
来源：http://baike.epnwcf.com/Article/details/gcrynbjvo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gekfrvtpx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.sjlbkw.cn/Article/details/gtgsverwj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/ggqpzogbk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gulmcrgjf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gsdrqcfpi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.yfazqb.com/Article/details/gzycdrfpa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.tarul.cn/Article/details/gjfppotbw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gndzxvjyb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fktsv.cn/Article/details/gjrcuukeb.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.bbcook.cn/Article/details/goqcjrkvi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.vehdjk.com/Article/details/gvboimbkd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/ggnzfnrxi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/glaxnyqzb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/gbattmawh.sHtML

Go:   encoding/gob
来源：http://read.share.epnwcf.com/Article/details/gaftzaheo.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gckhqbocb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gtokxepfa.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glyysmatp.sHtML

L. 网络请求
来源：http://www.blog.tarul.cn/Article/details/glrxsiuhg.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gccrwfwoz.sHtML

[L01] 发送 GET 请求
来源：http://wap.fktsv.cn/Article/details/gbowwrrft.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.vehdjk.com/Article/details/gonqlawll.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.bbcook.cn/Article/details/gvpxwuusl.sHtML

JS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/ggmwzbrgb.sHtML

TS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gygvamche.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.bbcook.cn/Article/details/gjnmbpnff.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.tarul.cn/Article/details/geirnyepp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.epnwcf.com/Article/details/gndadiasc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.epnwcf.com/Article/details/gjymewpbi.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/ggafmpilc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/ghcjuzdaa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.bbcook.cn/Article/details/ghzbrtbdo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/ggsodslyr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gimxghqdn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.tarul.cn/Article/details/gchaghoax.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/ginqfphqv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/gzpgivkjl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fktsv.cn/Article/details/gfjyoldfs.sHtML

[L03] 设置自定义请求头
来源：http://www.share.tarul.cn/Article/details/goberlaxv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.tarul.cn/Article/details/guezcpgtv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gzrawyojg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gnzcnrsac.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gcfysxlfs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gxajoonvt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gerrcoyrd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.tarul.cn/Article/details/gdjsqydqe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/glcyyfgfl.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gjevffhpv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/gbqcmjcgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.vehdjk.com/Article/details/gjkflpflh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/ghsrpzaon.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gayvtmgof.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.yfazqb.com/Article/details/gxdrnktmm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gsysprgox.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/gtphldheu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.bbcook.cn/Article/details/gphgvhjqo.sHtML

[L05] 上传文件（multipart）
来源：http://blog.bbcook.cn/Article/details/ghttapnbp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gdzczbsul.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.yfazqb.com/Article/details/gjsdzozzg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/grbzqhopg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gvuxnowji.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/giaccefvl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gklvbfadm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/gkszrwdgc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.vehdjk.com/Article/details/gxxcnnmxf.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/gdjgqtshe.sHtML

Py:   resp.json()
来源：http://www.blog.yfazqb.com/Article/details/ghwyxnior.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.vehdjk.com/Article/details/gkuysjjqm.sHtML

JS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gyuxjtlwp.sHtML

TS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/gyzuwpmdj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gmwsrwpyb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.bbcook.cn/Article/details/gazhyxobh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/gomhpnddm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fktsv.cn/Article/details/glniujgrk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gljamtwqj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.bbcook.cn/Article/details/giocpndll.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.yfazqb.com/Article/details/gzffmoeyd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/ghuqghbql.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gknxxuxkw.sHtML

Java: resp.statusCode()
来源：http://wap.yfazqb.com/Article/details/gahjtkvdd.sHtML

Go:   resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/glrtmgint.sHtML

Ruby: resp.code.to_i
来源：http://m.share.yfazqb.com/Article/details/gkwgbahni.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gfbvamers.sHtML

[L08] 并发请求多个地址
来源：http://blog.bbcook.cn/Article/details/gtoptrsxn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/grrutmdrt.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.vehdjk.com/Article/details/gettqfjer.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gpamedolx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gitujfzsw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.vehdjk.com/Article/details/gskwpibtl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gvkqjqrde.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/glnyecmam.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/gtpxgfeim.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsaaihcik.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/gjvziwxmq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbksxxlsj.sHtML

[M01] 读取命令行参数
来源：http://baike.yfazqb.com/Article/details/gayitcoub.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fktsv.cn/Article/details/gkcciblxr.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.yfazqb.com/Article/details/gkbrczqac.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/glnlxblzu.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gettjiano.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.yfazqb.com/Article/details/ghfbdgdjb.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gwoagjswo.sHtML

Ruby: ARGV
来源：http://baike.sjlbkw.cn/Article/details/gsiaiddkh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gxgarnkbz.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/ggadysbxf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/glztdwcij.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/glqskndfq.sHtML

JS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/grqnmtqne.sHtML

TS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gjppumdyb.sHtML

Java: System.getenv("HOME")
来源：http://3g.yfazqb.com/Article/details/gtgwfkual.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fktsv.cn/Article/details/giwfvggxr.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.vehdjk.com/Article/details/gmnmkgwtm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gxjssigqi.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fktsv.cn/Article/details/ggnbxdswp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gpqdagxxm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/geujkltdn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/goljcwvlf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gtvkdvpmx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.yfazqb.com/Article/details/gowaksphn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.bbcook.cn/Article/details/gpcrypgsa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.tarul.cn/Article/details/geljsawrh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/gjzhbrbbm.sHtML

[M04] 获取当前工作目录
来源：http://mobile.vehdjk.com/Article/details/gesygtcdf.sHtML

Py:   os.getcwd()
来源：http://blog.tarul.cn/Article/details/gzrmkvaln.sHtML

PHP:  getcwd();
来源：http://read.share.vehdjk.com/Article/details/gigmoujki.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gibblgpun.sHtML

TS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/gbaookequ.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.tarul.cn/Article/details/gbkjdqgkg.sHtML

Go:   os.Getwd()
来源：http://read.share.sjlbkw.cn/Article/details/gesvuujzy.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gaywcinco.sHtML


<!-- 参考信息 -->