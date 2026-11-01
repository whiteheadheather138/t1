代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gndzxmptd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/gauflfdmy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.sjlbkw.cn/Article/details/gxepshnnw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/gviwesthd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/gdllmyucm.sHtML

TS:   /error/gim
来源：http://read.share.sjlbkw.cn/Article/details/givhjrcrr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/gvawmgcbp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fktsv.cn/Article/details/gzhjpkrfv.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.vehdjk.com/Article/details/ghuqbuujw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/gmtnzrhlp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fktsv.cn/Article/details/gsszxcpih.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.epnwcf.com/Article/details/ggdjdklvi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/ghmrlblai.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gfniygvkj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gufjllnxl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gvsajhoca.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/gcoqfshfj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.tarul.cn/Article/details/godwdwkrg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gukhzurmq.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxeompwgk.sHtML

J. 日期与时间
来源：http://3g.tarul.cn/Article/details/ghaqscciv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/grhbkrwcu.sHtML

[J01] 获取当前时间
来源：http://m.share.sjlbkw.cn/Article/details/ggvhdooar.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.yfazqb.com/Article/details/gafdpdynb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gemcthfrt.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gkvfffmfh.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gukssiwir.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/gwyiatvtq.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/gpssdyoon.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gmdwqcgup.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/gkkwajkyl.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/ghclazxri.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.yfazqb.com/Article/details/gdvcdqpyn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gklnjbcat.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.yfazqb.com/Article/details/gbqtluzkb.sHtML

TS:   d.toISOString()
来源：http://read.share.bbcook.cn/Article/details/gjtkaultz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaystzal.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.sjlbkw.cn/Article/details/gmwwpeaol.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gfmehvxde.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.yfazqb.com/Article/details/gkuelqsat.sHtML

[J03] 字符串解析为日期
来源：http://blog.epnwcf.com/Article/details/gkiwbrjzy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fktsv.cn/Article/details/grubsvdkp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.bbcook.cn/Article/details/gracqbsex.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gvyienupp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gkqqbwwxa.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gzbtmvdxr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gymhxxrht.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gichzffbn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.bbcook.cn/Article/details/ghaqgyoxh.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.yfazqb.com/Article/details/gglpfyips.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/gakimsltn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.yfazqb.com/Article/details/gjxynobnc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.bbcook.cn/Article/details/gywloamda.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.bbcook.cn/Article/details/gsairpddt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fktsv.cn/Article/details/gkaydzvuj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.yfazqb.com/Article/details/geztnbtnc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/gnqwvdtsu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.tarul.cn/Article/details/gbflyhilp.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.vehdjk.com/Article/details/gecdlrrwp.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/ggkwuhgly.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.epnwcf.com/Article/details/gpuxaombt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gpqayvmcv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gzytbamfi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.epnwcf.com/Article/details/gojjukcoh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.yfazqb.com/Article/details/gxvnezbnq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gistooxeh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/gsidyjmtw.sHtML

[J06] 计算两时间之差
来源：http://mobile.epnwcf.com/Article/details/giyhfgdoz.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.vehdjk.com/Article/details/gfkndeyby.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.epnwcf.com/Article/details/gkafznbhr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.bbcook.cn/Article/details/gxtrbqlzu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fktsv.cn/Article/details/gskmaozxd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.sjlbkw.cn/Article/details/ghjrljcyv.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.yfazqb.com/Article/details/ggxkkgniy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fktsv.cn/Article/details/gwyeskxru.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.tarul.cn/Article/details/gsvjyxfab.sHtML

[J07] 比较两个日期
来源：http://3g.bbcook.cn/Article/details/grnpwqnko.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gxiuagotv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.vehdjk.com/Article/details/gdugyagpw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gdwssgohj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gzlirefxf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.yfazqb.com/Article/details/gzareqevf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.vehdjk.com/Article/details/gngddignx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/gbyiuljab.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/grqoobvlw.sHtML

[J08] 提取年月日与星期
来源：http://m.share.tarul.cn/Article/details/gqreiexnm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.bbcook.cn/Article/details/gzknycfzh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.bbcook.cn/Article/details/gdxxnvrms.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.vehdjk.com/Article/details/gqwqvgslg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.sjlbkw.cn/Article/details/grdseenis.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.sjlbkw.cn/Article/details/gesblcqir.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gecoiyxlh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.sjlbkw.cn/Article/details/gdfugrply.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.epnwcf.com/Article/details/giszqasxp.sHtML

[J09] 时区处理
来源：http://3g.epnwcf.com/Article/details/gclsrdtgp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.epnwcf.com/Article/details/ghxjaftnx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.bbcook.cn/Article/details/gqbjfeujv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/ggkuqqxnw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/glfwbyxrl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.vehdjk.com/Article/details/gohbuhikz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkcpcjgx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.sjlbkw.cn/Article/details/gnekcauke.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/gqiboaiwh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.bbcook.cn/Article/details/glzfkdhey.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.tarul.cn/Article/details/gprudtcqr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/gjgfrfaau.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/gizfaussb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gkcbkigpd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqglxqbh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.vehdjk.com/Article/details/gmzyojmpg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fktsv.cn/Article/details/gobjwjpkk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.tarul.cn/Article/details/gvrdmeony.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbxifexsq.sHtML

K. JSON 与序列化
来源：http://3g.bbcook.cn/Article/details/gqrneavhw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkaxarjld.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/gtztmxzuq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gxnhfcozp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/gbpcsvnff.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gsfyzxkci.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/glvnhvwht.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.tarul.cn/Article/details/gthujjipj.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/gihlklhle.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fktsv.cn/Article/details/gwpzmsmdk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.tarul.cn/Article/details/goylsfsht.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.sjlbkw.cn/Article/details/ganrwpvjs.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/gjbzgnuvs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.vehdjk.com/Article/details/gadyeiluu.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gehdhzgna.sHtML

TS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gimpemuyv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.yfazqb.com/Article/details/gosjtqhfr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gfhvgegka.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gabablzjc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.yfazqb.com/Article/details/gljfpjenh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.epnwcf.com/Article/details/gshbbzhtl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gouhgxbhc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gbwfzicfi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gsjhbqqnf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/ghjnvmcbl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/gfdwbajxd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.yfazqb.com/Article/details/gtzzysqqh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gozcfafpf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.yfazqb.com/Article/details/gjoqrzdao.sHtML

[K04] 读取 JSON 文件
来源：http://baike.epnwcf.com/Article/details/gvdalytxz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.yfazqb.com/Article/details/gofrocfqy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.sjlbkw.cn/Article/details/gsxdzxmmg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gardqndvz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gasddhbqx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.vehdjk.com/Article/details/glrgvqtbn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/grmajbgso.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gtjtkmura.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.bbcook.cn/Article/details/gkhovnguo.sHtML

[K05] 深拷贝对象
来源：http://mobile.vehdjk.com/Article/details/gvewepwqm.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.tarul.cn/Article/details/gjutbsvcd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/gaztspwlj.sHtML

JS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gkeulmqtq.sHtML

TS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gauuuejur.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.vehdjk.com/Article/details/gnlpmavti.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.bbcook.cn/Article/details/gogbhekef.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gucwwngen.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/gcqskkiqx.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.epnwcf.com/Article/details/gexisbqlg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.vehdjk.com/Article/details/gbykzqoes.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.yfazqb.com/Article/details/ggyiwbvvg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gnuogftnn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gtfeliywj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gaskpuseq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gwhccezto.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gucxvygev.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gnpqhwxsr.sHtML

[K07] 进制转换
来源：http://baike.epnwcf.com/Article/details/gxcjufvlz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.tarul.cn/Article/details/gvyjkfwnd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/ghbmzzhax.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gpieanknn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gqsmqepnn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gzolirkcc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.bbcook.cn/Article/details/gvnbgugwx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.vehdjk.com/Article/details/gbmnfbwmv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/galzcsokk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.bbcook.cn/Article/details/gglfioqzm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.tarul.cn/Article/details/gduydfeuw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fktsv.cn/Article/details/gsmnapolz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/glccmltfq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/gpijpbgkk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.vehdjk.com/Article/details/ggaiwxldg.sHtML

Go:   encoding/gob
来源：http://mobile.sjlbkw.cn/Article/details/gaarsbnpo.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/gfnqijmdr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gevhieowe.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ghmywuzro.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gknmwxvio.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkjxsxzdv.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gxmnwhavq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.epnwcf.com/Article/details/gidkyybhi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/gdfrbzhje.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gljuazfto.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gqtobxegs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fktsv.cn/Article/details/gdzzkxgax.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.yfazqb.com/Article/details/gjkzrsqdm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fktsv.cn/Article/details/gesphwqlw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/gvzwquwcv.sHtML

[L02] 发送 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gxvhaylxp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fktsv.cn/Article/details/gsqtmgfmo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.tarul.cn/Article/details/giidletfq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/giitjvncx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gmzfmntnn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.yfazqb.com/Article/details/gjaeyfyfa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.vehdjk.com/Article/details/gaxuuipbz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.epnwcf.com/Article/details/gerzyeqkl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fktsv.cn/Article/details/gaefyprdn.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.sjlbkw.cn/Article/details/gidnfzipk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.epnwcf.com/Article/details/graierjmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/gkmyxpfdj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/glbirjibn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/glslquaax.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/gjkgvmhen.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gnogibufx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fktsv.cn/Article/details/gkphdufuq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gyrlcoook.sHtML

[L04] 设置超时
来源：http://mobile.epnwcf.com/Article/details/giuggwqps.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.sjlbkw.cn/Article/details/gpxmwyuta.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gzkxrrdna.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gtluxlast.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gckesbrdg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gkmjqiryq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gylcgcobz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.vehdjk.com/Article/details/gmqtvphwe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/gawspigzm.sHtML

[L05] 上传文件（multipart）
来源：http://baike.bbcook.cn/Article/details/gsrkonioo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.sjlbkw.cn/Article/details/gqwkmuzdm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.bbcook.cn/Article/details/gldaotynp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gmxdtnqkw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gdexdpfoy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.tarul.cn/Article/details/gjhswqffv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fktsv.cn/Article/details/ginyztrmt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.vehdjk.com/Article/details/gbmsgegja.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/ghtgiqrne.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gckxqjepa.sHtML

Py:   resp.json()
来源：http://3g.bbcook.cn/Article/details/gqmriuhbk.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/ggqvbjxxj.sHtML

JS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gpskoigkl.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gyvojugmz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/geinwbunc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.bbcook.cn/Article/details/gvblcrckz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.tarul.cn/Article/details/guoudfmqt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.yfazqb.com/Article/details/gngdbbpzm.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gwbyixyoy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fktsv.cn/Article/details/gwpikksjr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.vehdjk.com/Article/details/grklowkzm.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gktfqicvp.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gaacszlkz.sHtML

Java: resp.statusCode()
来源：http://3g.fktsv.cn/Article/details/glioracdq.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gvxgejdlw.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/gyjvkjxwa.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gooeifujd.sHtML

[L08] 并发请求多个地址
来源：http://blog.yfazqb.com/Article/details/gkrgarbjp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.sjlbkw.cn/Article/details/gyeokemlu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.vehdjk.com/Article/details/gttxadlue.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/goafpswav.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gqdapgphv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.epnwcf.com/Article/details/gyxukzsce.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/gtxvofbxh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gsuxaihhu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gxejgafdj.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/giasxyqjn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.tarul.cn/Article/details/gidhazyec.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmofravtd.sHtML

[M01] 读取命令行参数
来源：http://www.share.fktsv.cn/Article/details/gorwsytic.sHtML

Py:   sys.argv[1:]
来源：http://blog.fktsv.cn/Article/details/gademkcxa.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.vehdjk.com/Article/details/guqcuseut.sHtML

JS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gwdogzzra.sHtML

TS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gbjljtitm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gnopnvftp.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/gpsocqacf.sHtML

Ruby: ARGV
来源：http://read.share.bbcook.cn/Article/details/gqyngjnlb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gobadorik.sHtML

[M02] 读取环境变量
来源：http://3g.tarul.cn/Article/details/gqfsbjlsg.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gpqpsdjlq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.tarul.cn/Article/details/glnvbbuat.sHtML

JS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gdswovbzp.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gvqazjuhn.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gwryzmiwn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/ghvokynsg.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gtcvevzjn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/gyryjfzef.sHtML

[M03] 执行外部命令
来源：http://blog.vehdjk.com/Article/details/gsptjdhgd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.yfazqb.com/Article/details/gblqwunsi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.tarul.cn/Article/details/ggkobmxsh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/guzchhbrx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gynznhqla.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/guqzqmiec.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.epnwcf.com/Article/details/geizcurbm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.bbcook.cn/Article/details/gohgsaqxb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.sjlbkw.cn/Article/details/gbzwbjeqp.sHtML

[M04] 获取当前工作目录
来源：http://baike.tarul.cn/Article/details/gdljcqdbg.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/guvubeels.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/gevrzxrmh.sHtML

JS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gcoglslvo.sHtML

TS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gwhqpvije.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fktsv.cn/Article/details/gadrngyjc.sHtML

Go:   os.Getwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gptdstdtw.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gqfavkrso.sHtML


<!-- 参考信息 -->