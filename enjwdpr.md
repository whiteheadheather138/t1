代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fktsv.cn/Article/details/gzawkwfht.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.yfazqb.com/Article/details/gnxqqnqpz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/givyorsjl.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghcadwnwl.sHtML

J. 日期与时间
来源：http://m.share.fktsv.cn/Article/details/gctvkekox.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxobcvziq.sHtML

[J01] 获取当前时间
来源：http://baike.fktsv.cn/Article/details/gwfiutktc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.tarul.cn/Article/details/gjrfxqfjn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/grrjldird.sHtML

JS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gsqotleiy.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gatdvyscn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.tarul.cn/Article/details/gkafsuyhw.sHtML

Go:   time.Now()
来源：http://3g.bbcook.cn/Article/details/gguesfkpk.sHtML

Ruby: Time.now
来源：http://blog.tarul.cn/Article/details/gbsivskbg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.bbcook.cn/Article/details/gwbadlnme.sHtML

[J02] 格式化输出
来源：http://3g.tarul.cn/Article/details/gfabikdcq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/gzapbvzdq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/gyztqkwaq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.tarul.cn/Article/details/gbyqvnyey.sHtML

TS:   d.toISOString()
来源：http://www.share.yfazqb.com/Article/details/gcxrbsjxj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.yfazqb.com/Article/details/gytuhjdhl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fktsv.cn/Article/details/gmuzxtris.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gncrullao.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.epnwcf.com/Article/details/ggnltwkvk.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.bbcook.cn/Article/details/gdlywscau.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.sjlbkw.cn/Article/details/gsurzprmr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.tarul.cn/Article/details/gwcdygbkf.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gwvwucahc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gcoaxuhme.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gkjucgeyp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gqkntchad.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gyvpxxavn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.yfazqb.com/Article/details/gomzuukby.sHtML

[J04] 时间戳与日期互转
来源：http://blog.vehdjk.com/Article/details/gsuborpda.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/giuebhjme.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.sjlbkw.cn/Article/details/golcpgtua.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhacupto.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gdindxbzm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/gnbgbftge.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.epnwcf.com/Article/details/gvfminthn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/griuqkcod.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.vehdjk.com/Article/details/gfshgodud.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.bbcook.cn/Article/details/gehqnxjem.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fktsv.cn/Article/details/ggryidhik.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.yfazqb.com/Article/details/gohhlfoit.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/gpvnyzjsg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/ggtufdilf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fktsv.cn/Article/details/gynaytehy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/gjehcovey.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.yfazqb.com/Article/details/gehbbrhkt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.vehdjk.com/Article/details/gadybxdif.sHtML

[J06] 计算两时间之差
来源：http://3g.epnwcf.com/Article/details/guinfseis.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.bbcook.cn/Article/details/gdurqroxt.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.tarul.cn/Article/details/gfmbwocre.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/goptsifil.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.bbcook.cn/Article/details/gstavivgf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.tarul.cn/Article/details/gegegyusu.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fktsv.cn/Article/details/gtogedout.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.sjlbkw.cn/Article/details/gynflpiuz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.tarul.cn/Article/details/gznenomhl.sHtML

[J07] 比较两个日期
来源：http://wap.sjlbkw.cn/Article/details/gtkfkwppx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/grgeybfwn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.tarul.cn/Article/details/gpwqchsly.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gxmupdksf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/gronzounx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.vehdjk.com/Article/details/gqxzlkwdo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.yfazqb.com/Article/details/gnvaqwqvf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gagqerokh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/ggttmwrth.sHtML

[J08] 提取年月日与星期
来源：http://baike.vehdjk.com/Article/details/ggukgqveb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fktsv.cn/Article/details/galkapavt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.sjlbkw.cn/Article/details/guryncugt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.bbcook.cn/Article/details/gvwqkfpyn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.vehdjk.com/Article/details/gnzswxpbz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/gejwthndn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.sjlbkw.cn/Article/details/gtvozfako.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/gcirnkhvp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.sjlbkw.cn/Article/details/gmjtwooke.sHtML

[J09] 时区处理
来源：http://www.blog.tarul.cn/Article/details/ggnoaitbm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.tarul.cn/Article/details/gggtofvva.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.epnwcf.com/Article/details/gawqdfigq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gbzpiubkk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gafmsjxgp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.bbcook.cn/Article/details/gpbhjguzd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.tarul.cn/Article/details/guipnkwgq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/ggaumgmlg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.sjlbkw.cn/Article/details/gzjmeadtt.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.yfazqb.com/Article/details/gbwkxtjyf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.vehdjk.com/Article/details/gerjedrud.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.yfazqb.com/Article/details/gpztbdtnc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.epnwcf.com/Article/details/glelykpmd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/getwcypys.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.bbcook.cn/Article/details/gopwqepso.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.tarul.cn/Article/details/grymnumzq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.bbcook.cn/Article/details/goflexhae.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.vehdjk.com/Article/details/gkdbujwad.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/grmluwqlm.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/gfofciwmu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbctolyzr.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gvtimvdpa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gtdsmgmyd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gehitqeis.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gdwfyfojq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/glbvjewxa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/gowqnbxin.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/gtoqnzfie.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.vehdjk.com/Article/details/gfvppjxor.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.tarul.cn/Article/details/gfjwuayzh.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.bbcook.cn/Article/details/gutjdqqzw.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/gkzgdfqpz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.tarul.cn/Article/details/gfyyrjaoa.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gwqjcnkuv.sHtML

TS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/ghwkdcimt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.yfazqb.com/Article/details/giaevkiqe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gqhgfcyem.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gotoovxgi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmeouvigb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.yfazqb.com/Article/details/gjsoolxbt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gachjiitf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/guxyhmydn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gcjezgmdt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/glkzoeslg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gnkvvmeox.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fktsv.cn/Article/details/gjdwnkuba.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.yfazqb.com/Article/details/gjwpcoxvg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.bbcook.cn/Article/details/gbsyijgiy.sHtML

[K04] 读取 JSON 文件
来源：http://3g.vehdjk.com/Article/details/gfiholsqy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/geialmfro.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.bbcook.cn/Article/details/gfxghhvqc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.epnwcf.com/Article/details/gfxswmypk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gjkhzudvg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gjksixcaz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/grhwiffmb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gudxpemzf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gncrkdtaf.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/gxyibqjvt.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.vehdjk.com/Article/details/growdzvgv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.bbcook.cn/Article/details/gxsafzojh.sHtML

JS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gatndcywv.sHtML

TS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gnzneizqp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.epnwcf.com/Article/details/grfkyyxzq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.sjlbkw.cn/Article/details/gmgahgcot.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.tarul.cn/Article/details/gjjhzyons.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/gjjpdrsap.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.tarul.cn/Article/details/gseqluqok.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.tarul.cn/Article/details/gvmbweopa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.vehdjk.com/Article/details/gzrbcsvex.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gvzvielqj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/gojwpxiej.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/gpgetoymd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gjeawhdep.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/grpbcdjlg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gvdexdnuw.sHtML

[K07] 进制转换
来源：http://wap.fktsv.cn/Article/details/gfnqwvydl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gmuloznmx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/gzcezjbpr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gcetptngr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/guwnihcag.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gicrselph.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.sjlbkw.cn/Article/details/gyjbtvxxo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gvrekykbc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gwywmdsae.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.epnwcf.com/Article/details/grvpdqdyk.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.yfazqb.com/Article/details/gdkhzpaqu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.epnwcf.com/Article/details/gwbtjestn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gfyllrxip.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gxaqvpdwg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/gqktgfulb.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/gnmvmcfue.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fktsv.cn/Article/details/grvjrhpap.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gnjsdhdql.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gljivpifn.sHtML

L. 网络请求
来源：http://baike.fktsv.cn/Article/details/gblgblkqp.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcssqcupd.sHtML

[L01] 发送 GET 请求
来源：http://blog.vehdjk.com/Article/details/gppuvzodn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.bbcook.cn/Article/details/gbqtkqlqf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/gbolapbkj.sHtML

JS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gybqbicco.sHtML

TS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gluzujbki.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fktsv.cn/Article/details/gqgruanyz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gbzqtmulj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.sjlbkw.cn/Article/details/gnxdgnveh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fktsv.cn/Article/details/glpznrmcb.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/gtbnmtxok.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gfdzbhcjz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.yfazqb.com/Article/details/gmnoauaku.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/gkitiwdik.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gmlekydas.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gbootpspt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gwnbgycgb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.vehdjk.com/Article/details/gsyrffdmr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.tarul.cn/Article/details/gywvrmngy.sHtML

[L03] 设置自定义请求头
来源：http://www.share.epnwcf.com/Article/details/gdvzzgmmv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.vehdjk.com/Article/details/gpctkoenf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.sjlbkw.cn/Article/details/gpdqounmh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/giaxxqlog.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/gfincddzg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.vehdjk.com/Article/details/gsuzsqbyz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/geosvbnkg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gkbhxurdw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gcuvmtsfk.sHtML

[L04] 设置超时
来源：http://mobile.epnwcf.com/Article/details/gvkwjzdpe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.vehdjk.com/Article/details/gqrbfxpce.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.epnwcf.com/Article/details/gpmfdapka.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/gfeijzkym.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/geivsfsff.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.tarul.cn/Article/details/gsircjmlv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.yfazqb.com/Article/details/gnibxkzmw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fktsv.cn/Article/details/geakxozsn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/gjydrfklo.sHtML

[L05] 上传文件（multipart）
来源：http://blog.vehdjk.com/Article/details/ggxawgfar.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gdvienbdz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.sjlbkw.cn/Article/details/gxbgghlfc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gvbhwjwjf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gdqcuigug.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.vehdjk.com/Article/details/gubnkqubx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.sjlbkw.cn/Article/details/ghtfcmdwm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gofxcsyvd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.bbcook.cn/Article/details/gllnxzrrs.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/gyfmhjpet.sHtML

Py:   resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gophdpjzj.sHtML

PHP:  json_decode($body, true);
来源：http://wap.sjlbkw.cn/Article/details/gnrgfymwb.sHtML

JS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gpvbdjmnd.sHtML

TS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gjvhmgysq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fktsv.cn/Article/details/gejxpqxfg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/gryyvctrz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.yfazqb.com/Article/details/gkupjztuv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.yfazqb.com/Article/details/gqkpgjfji.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/ghguupbes.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.bbcook.cn/Article/details/ggztpxrpo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.tarul.cn/Article/details/gqcatplow.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/glpzwnefm.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gqpcxahmh.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/giaxndelj.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gluilfvoj.sHtML

Ruby: resp.code.to_i
来源：http://baike.bbcook.cn/Article/details/gtpuaazcl.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gxgwmcdnj.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gurwunlya.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/gjscxtbfw.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gsyecrvwg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gncqqjdla.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gxambjmvg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.yfazqb.com/Article/details/gvwpqpehk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.tarul.cn/Article/details/gpkisqajd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.vehdjk.com/Article/details/ghqanvtbn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.bbcook.cn/Article/details/gilzmyxkc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkuajunaw.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.vehdjk.com/Article/details/geyqovdhf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbmliogbq.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/goejqoowv.sHtML

Py:   sys.argv[1:]
来源：http://m.share.epnwcf.com/Article/details/gkydztfsp.sHtML

PHP:  $argv;  $argc;
来源：http://3g.bbcook.cn/Article/details/gmkwuiayi.sHtML

JS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gbxjnqeja.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gicrrycfq.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gppvtbsej.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/guigiqrue.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gfwtnxrjj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gamcfwykk.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/ggvnrttdo.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/glmdcttzo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/glaauhofw.sHtML

JS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gcniiulue.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gmhznrxgb.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/glsntfxgy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/gvuwdstde.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.bbcook.cn/Article/details/gcqfhzekt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.tarul.cn/Article/details/gelmycxib.sHtML

[M03] 执行外部命令
来源：http://wap.vehdjk.com/Article/details/gxjedbjfq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fktsv.cn/Article/details/gofxisgjh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gknsfasig.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gpqbuhigz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gzyckqrnm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.sjlbkw.cn/Article/details/gausipvxb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gimfbsoov.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/gksewubwa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/genswyjye.sHtML

[M04] 获取当前工作目录
来源：http://baike.bbcook.cn/Article/details/gasqrtyts.sHtML

Py:   os.getcwd()
来源：http://mobile.bbcook.cn/Article/details/gumkhsbmb.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gtihifpmi.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gqebplysj.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gvlhnddsm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/gwsrttbjo.sHtML

Go:   os.Getwd()
来源：http://3g.yfazqb.com/Article/details/ggftqdmkw.sHtML

Ruby: Dir.pwd
来源：http://read.share.yfazqb.com/Article/details/gkoxgxygq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.tarul.cn/Article/details/gujkeznyb.sHtML

[M05] 设置退出码
来源：http://www.blog.bbcook.cn/Article/details/gpsauugsp.sHtML

Py:   sys.exit(1)
来源：http://www.share.tarul.cn/Article/details/ghnurhmbo.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/gwylspkbd.sHtML

JS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/glwtpwzqa.sHtML

TS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gfzpgaiik.sHtML

Java: System.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gbektzznk.sHtML

Go:   os.Exit(1)
来源：http://mobile.fktsv.cn/Article/details/gniuwkiqt.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/grxnyjdbq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.tarul.cn/Article/details/gxmywkkqr.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gqmppfgbc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/givxlxclg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gwbeflakz.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gwiqmnedv.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gdmticfkp.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/ghzfzgktv.sHtML


<!-- 参考信息 -->