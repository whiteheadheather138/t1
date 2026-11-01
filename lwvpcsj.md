代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fktsv.cn/Article/details/goxhqjbra.sHtML

TS:   /error/gim
来源：http://www.share.vehdjk.com/Article/details/gkvkaggej.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.epnwcf.com/Article/details/gffupqdno.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/gllmereey.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.yfazqb.com/Article/details/gcwyxwnhk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/gwaspujmq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/gmsxkhbwl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.sjlbkw.cn/Article/details/gaqfpxgfy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/gxujzkhxd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/ghitabxkj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.bbcook.cn/Article/details/gploqrspm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/gsjquqtie.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.vehdjk.com/Article/details/glwpgemgn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.bbcook.cn/Article/details/gnbxjkyrk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gmswtdeky.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbjqmidus.sHtML

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/gxbegadru.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyjxdgulk.sHtML

[J01] 获取当前时间
来源：http://baike.tarul.cn/Article/details/gelcbnvap.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/gkclxqday.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gxyoiagxg.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gjygferte.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/girvvnvfv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.yfazqb.com/Article/details/gtqysvjzt.sHtML

Go:   time.Now()
来源：http://baike.vehdjk.com/Article/details/gzvcfopqv.sHtML

Ruby: Time.now
来源：http://m.share.fktsv.cn/Article/details/gvxgvhpre.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fktsv.cn/Article/details/ghcklzywp.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/gybhfwmsq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gsfkqzfll.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gsbdhqofe.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.tarul.cn/Article/details/gbmzeqymb.sHtML

TS:   d.toISOString()
来源：http://read.share.bbcook.cn/Article/details/ghrhvmjtj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fktsv.cn/Article/details/gbiqehgki.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.bbcook.cn/Article/details/gfkhtrgat.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/grzheniru.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/gxejzyhuy.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.yfazqb.com/Article/details/gbyzycggv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.bbcook.cn/Article/details/gpzxrwiil.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/gtjevonhu.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/glhbkktcy.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/guieupkkx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gbjxvflpj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gxrgbhtau.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gvefygzxv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.yfazqb.com/Article/details/ghooisrgr.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.sjlbkw.cn/Article/details/gddjztpea.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gzqijdecs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.bbcook.cn/Article/details/gwyoefxak.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.sjlbkw.cn/Article/details/guogxzfnh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.bbcook.cn/Article/details/gstbgchmk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/gckrnajpd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.sjlbkw.cn/Article/details/gohbtbrfn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.sjlbkw.cn/Article/details/ggdqbaecm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.vehdjk.com/Article/details/gjscwjnex.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/ggzyoonup.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.bbcook.cn/Article/details/gbtxhwkdl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/gwuujzmvy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gnnuotkzd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gvvvhrtat.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gmosmeexm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.yfazqb.com/Article/details/gqlhlzexc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.yfazqb.com/Article/details/gxtdyidlz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/glgrzmevv.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/gwspxkqfx.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fktsv.cn/Article/details/ghypcabrx.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.sjlbkw.cn/Article/details/gvofzalbo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.epnwcf.com/Article/details/gobhybqxm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.bbcook.cn/Article/details/gdlxykjok.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.yfazqb.com/Article/details/gyiluposj.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.tarul.cn/Article/details/grhsowzmi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.epnwcf.com/Article/details/gqjdjbhpv.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/ggsuakjpe.sHtML

[J07] 比较两个日期
来源：http://read.share.sjlbkw.cn/Article/details/grmuavyxj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gucxyzkch.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.epnwcf.com/Article/details/gogfamgzb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fktsv.cn/Article/details/gqpvrtyvl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/ghkjfrnfz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.vehdjk.com/Article/details/ggojwlise.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.tarul.cn/Article/details/gicrlpwbt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gncxfgyxy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gqfctwwru.sHtML

[J08] 提取年月日与星期
来源：http://www.share.sjlbkw.cn/Article/details/grwjhytcf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/grxzjshqk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/gftmcftvz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.sjlbkw.cn/Article/details/ggllaitgu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/ggupselmy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.sjlbkw.cn/Article/details/gnpstqope.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.vehdjk.com/Article/details/gmooqxibs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fktsv.cn/Article/details/ggmjqsuwn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fktsv.cn/Article/details/gcxpgopqp.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/gpahdscxn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.vehdjk.com/Article/details/gwyoahzef.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.yfazqb.com/Article/details/grfxnimuw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gbqddsfgg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/gfhunyggw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.sjlbkw.cn/Article/details/gdlwrkmrt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.epnwcf.com/Article/details/glvkkwxza.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.vehdjk.com/Article/details/gzfpjxdpf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fktsv.cn/Article/details/gzngwfnzu.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.vehdjk.com/Article/details/giwtfzrqt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gxgcubkme.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.tarul.cn/Article/details/gfcebiclz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.tarul.cn/Article/details/gprvlbnfa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.yfazqb.com/Article/details/gawczjczl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/gcqxyeaql.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fktsv.cn/Article/details/gexvuiqhd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.sjlbkw.cn/Article/details/gzsveiwyy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.yfazqb.com/Article/details/gbarxsoka.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzmcapxkp.sHtML

K. JSON 与序列化
来源：http://www.share.sjlbkw.cn/Article/details/gyjrurfvm.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/givdbspgi.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuryewnh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/ggqorasvr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gsrfgpxkg.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gvkxhqogz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gjfihatep.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.tarul.cn/Article/details/ghdsnjild.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fktsv.cn/Article/details/gymwywyhp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.sjlbkw.cn/Article/details/ghnwqotpb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fktsv.cn/Article/details/gzrcidiyl.sHtML

[K02] JSON 字符串转对象
来源：http://baike.epnwcf.com/Article/details/gtqkpcrql.sHtML

Py:   json.loads(s)
来源：http://wap.epnwcf.com/Article/details/gugmpimdd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.epnwcf.com/Article/details/grqpdjlqe.sHtML

JS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gyngbzdsb.sHtML

TS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/ghbqddgcg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/gqdculejb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gwdkhxpal.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/glbguwvop.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gfhqpilfu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/gauqvqqzj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gylbbxizf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/grwyczicb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gqlbstzot.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/ganjsluyz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/gqwcjegcd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.vehdjk.com/Article/details/gdvbencms.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gxndhxcqf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.vehdjk.com/Article/details/gudzpcqtk.sHtML

[K04] 读取 JSON 文件
来源：http://blog.bbcook.cn/Article/details/gimiskibk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/gwtziimqo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.epnwcf.com/Article/details/gdsswvtdz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/gmfgwhkwi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.epnwcf.com/Article/details/gqhsyiycc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gsxevsngv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gyhygwcre.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gfezcwrzi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/grprvfytr.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.tarul.cn/Article/details/gwuoguvnc.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.epnwcf.com/Article/details/ggfvzcygw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gqjbgbwml.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gyftgraoy.sHtML

TS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gknpqumaq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gdiwlymft.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/gosrmfvgb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/glhdafnau.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.tarul.cn/Article/details/guoejhuvu.sHtML

[K06] 解析 URL 查询串
来源：http://baike.vehdjk.com/Article/details/gazswvbru.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gphnmsmir.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/gdpgzcdjw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gduuzkusf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gymmatsxo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.epnwcf.com/Article/details/gvvpwbrxm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gznipdbff.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gfewmfueo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/guipwgmob.sHtML

[K07] 进制转换
来源：http://www.blog.yfazqb.com/Article/details/gmiohahix.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gsqdspsrt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.yfazqb.com/Article/details/giaxyoatv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/givpffiif.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/guohdezfo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gglanluct.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fktsv.cn/Article/details/gsyjtpqtp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/glhezhwgy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gabzrqiyn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.vehdjk.com/Article/details/gjbagmofk.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.epnwcf.com/Article/details/ggsunopnu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.bbcook.cn/Article/details/gxkzokmow.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gfdctavql.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gefdjzzkc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gevickbsv.sHtML

Go:   encoding/gob
来源：http://wap.bbcook.cn/Article/details/gdqfwvyhf.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/gumlzzfjc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gqsontgyf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcsidawwo.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/gdedukgum.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvefrjxob.sHtML

[L01] 发送 GET 请求
来源：http://mobile.bbcook.cn/Article/details/gwlttzoyi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.epnwcf.com/Article/details/gethonpbx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.sjlbkw.cn/Article/details/gtdskrtgu.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gduzxgozi.sHtML

TS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gexmwbsdh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/gibumsasp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.tarul.cn/Article/details/glsrwsrpg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/gwvssuvil.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.epnwcf.com/Article/details/gterkocuo.sHtML

[L02] 发送 POST JSON
来源：http://blog.yfazqb.com/Article/details/gyynrbjpg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gwjghqbmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.epnwcf.com/Article/details/gmrbrtuip.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/gmpfbojvl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gsauugazy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gpyecrcxf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.tarul.cn/Article/details/gylbvkwxp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/gsdbzilir.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.vehdjk.com/Article/details/gczvqqklr.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/gvdydmmed.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gzgnlzbnd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.tarul.cn/Article/details/gvdmefiqn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/glkhyllzn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/ggoxjnauf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.sjlbkw.cn/Article/details/gieystsgz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gnupgsjbw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fktsv.cn/Article/details/gmwlrdkut.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gapkpncgk.sHtML

[L04] 设置超时
来源：http://m.share.vehdjk.com/Article/details/gskvdqvom.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.sjlbkw.cn/Article/details/gvxcpxkro.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fktsv.cn/Article/details/gjabepkzy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gxxmbestj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/ghgifeapr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.bbcook.cn/Article/details/gxsxpaqxf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gkykvfgnz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.sjlbkw.cn/Article/details/gbpgaakaj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/geewdjggf.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/gchugbgvy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.epnwcf.com/Article/details/gmsuiflgg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gkebkmrvo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gebarsjec.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gmuzxbfxi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.vehdjk.com/Article/details/gdmezbtxy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gcyirhdfs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.vehdjk.com/Article/details/gajscyjxw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.yfazqb.com/Article/details/glhadmffq.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gxeuxlfgz.sHtML

Py:   resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gytikngul.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/gjtpnkwjb.sHtML

JS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gjiroomlk.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gojlqkhci.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gckzxvbjk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.epnwcf.com/Article/details/gtvdtigay.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/giinrryzy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gxysodkdk.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gfyebnfyl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/ghxbdsqea.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.epnwcf.com/Article/details/gwfhvkzgr.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gdhzgyavy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gufitntci.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/gsddptphw.sHtML

Go:   resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gkmivrxgd.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gutnpusti.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/gwtrasaha.sHtML

[L08] 并发请求多个地址
来源：http://baike.vehdjk.com/Article/details/gnclekyno.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fktsv.cn/Article/details/gklfwrymh.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.epnwcf.com/Article/details/glgffhana.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gyrpurzbc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gfbctbsli.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.bbcook.cn/Article/details/glanjntqn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.vehdjk.com/Article/details/gcrizijqo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.bbcook.cn/Article/details/gignanzik.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gvloyfbeu.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtjqnnadl.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/gvljefmze.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqfyxxqvj.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gamvgebdt.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gyipuyxsi.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/gvswwbide.sHtML

JS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/ghgovrrlt.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gyxllvvcz.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/glaugjret.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gptuiatoh.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/gdatwgixm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/govimavkq.sHtML

[M02] 读取环境变量
来源：http://baike.epnwcf.com/Article/details/gffqzzrkq.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.epnwcf.com/Article/details/gjekhnfhv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gdiojqbma.sHtML

JS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gsmudmhvp.sHtML

TS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/genylrytb.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gjmylnzhn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/gijehcaxy.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/girrzefhb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gwkdcleti.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gpeiqjlsz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.tarul.cn/Article/details/gieckykzk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/gjiazwpug.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gvgwkpcvy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gufntcijn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.yfazqb.com/Article/details/gdclpdlzn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/geegerano.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.vehdjk.com/Article/details/ghkbaxaqb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fktsv.cn/Article/details/gajzetdfc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gkjebybcq.sHtML

Py:   os.getcwd()
来源：http://3g.sjlbkw.cn/Article/details/gozsldfha.sHtML

PHP:  getcwd();
来源：http://baike.fktsv.cn/Article/details/gepnzzkss.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/ghppuukdu.sHtML

TS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gejeobsdi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/gntsfrepx.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/grnshbsun.sHtML

Ruby: Dir.pwd
来源：http://baike.bbcook.cn/Article/details/glnhnclnv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/gyfrgveuy.sHtML

[M05] 设置退出码
来源：http://www.share.fktsv.cn/Article/details/gpvnvzyin.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/glwvbrckg.sHtML

PHP:  exit(1);
来源：http://www.m.share.yfazqb.com/Article/details/glrnqayqz.sHtML


<!-- 参考信息 -->