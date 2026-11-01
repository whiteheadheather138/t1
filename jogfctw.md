代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.sjlbkw.cn/Article/details/gcemytmbp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.tarul.cn/Article/details/gbdhayasn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gtmtcrjkn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmgblgdyn.sHtML

J. 日期与时间
来源：http://mobile.yfazqb.com/Article/details/gmkhqasnv.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grgsekaih.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gsvhxwdyf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.tarul.cn/Article/details/gunkzttai.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gzxoyxeid.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gkhwjugcu.sHtML

TS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gwoyejahx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaeqmuygp.sHtML

Go:   time.Now()
来源：http://m.share.tarul.cn/Article/details/gkdbeiwgk.sHtML

Ruby: Time.now
来源：http://www.share.sjlbkw.cn/Article/details/gdisevfvx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/givvxntpy.sHtML

[J02] 格式化输出
来源：http://read.share.tarul.cn/Article/details/gzdbqnmaz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/gtzlswwuy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gwkctaonw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.epnwcf.com/Article/details/guxknwbnw.sHtML

TS:   d.toISOString()
来源：http://www.blog.sjlbkw.cn/Article/details/gsksmnuxe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fktsv.cn/Article/details/ggruqthwj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.bbcook.cn/Article/details/gnwxofvid.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/gubtlsmsm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.sjlbkw.cn/Article/details/gojfowlap.sHtML

[J03] 字符串解析为日期
来源：http://mobile.yfazqb.com/Article/details/gujrdjrkr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.sjlbkw.cn/Article/details/gwzzeiggx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.vehdjk.com/Article/details/ghmkouckb.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gjczruxsn.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gqkntkfvo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gkeroaaly.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.yfazqb.com/Article/details/geaftiwyi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gjbzxgwda.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.tarul.cn/Article/details/gncxbaoqe.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.sjlbkw.cn/Article/details/gohzagnnj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.bbcook.cn/Article/details/gsyvqpfrf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fktsv.cn/Article/details/gaouecvls.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.sjlbkw.cn/Article/details/guvgcsjli.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.vehdjk.com/Article/details/gtrxikakc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.tarul.cn/Article/details/gwttujjon.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/gzqyvztlg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.vehdjk.com/Article/details/giphyyezm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.vehdjk.com/Article/details/gaxhcplcm.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.epnwcf.com/Article/details/gtxuhmzyl.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fktsv.cn/Article/details/gwprtmejh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.tarul.cn/Article/details/guwwesdsz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gkhepzlvl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gaybnyngm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gkcglpdvj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.vehdjk.com/Article/details/glzsvlwxh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fktsv.cn/Article/details/guqyhxxga.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fktsv.cn/Article/details/gyaqbdsax.sHtML

[J06] 计算两时间之差
来源：http://m.share.yfazqb.com/Article/details/gfmucgcce.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/giiffnjzo.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.epnwcf.com/Article/details/gdsfcgxex.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.epnwcf.com/Article/details/gqktfpjrg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.tarul.cn/Article/details/gsjhtnorf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/gglziobje.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fktsv.cn/Article/details/ggyfjtkhc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.epnwcf.com/Article/details/ggmhopdsi.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/gapyjlozp.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/gmjjuguib.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/giiqngeir.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.sjlbkw.cn/Article/details/ggxfzjwwc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gvftaxmru.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gcvquvwij.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.tarul.cn/Article/details/gmbkmyucx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gawaihknt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gzayujbhs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gpatfhgbm.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gfjgxkjay.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.tarul.cn/Article/details/gofhpzeut.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.yfazqb.com/Article/details/gjrcgdrmv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.sjlbkw.cn/Article/details/georwtifj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.vehdjk.com/Article/details/gdmimkpck.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.epnwcf.com/Article/details/galkamvxl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.yfazqb.com/Article/details/ghkwsbglj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.tarul.cn/Article/details/guxejwtwl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gbjbebedr.sHtML

[J09] 时区处理
来源：http://blog.fktsv.cn/Article/details/galwfkzex.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.sjlbkw.cn/Article/details/gxssgcnvz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.epnwcf.com/Article/details/ghadzalqe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/giusfczjp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gpxgsuvil.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.epnwcf.com/Article/details/gkenqybtq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.yfazqb.com/Article/details/gcspzhnhb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.epnwcf.com/Article/details/gfxjszuix.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fktsv.cn/Article/details/geqmphwpc.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.epnwcf.com/Article/details/gwdubbcbv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.bbcook.cn/Article/details/gsbbxjula.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fktsv.cn/Article/details/gzctvleva.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fktsv.cn/Article/details/gszqnhggo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/geupctrjc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.tarul.cn/Article/details/ggqcuacxu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.tarul.cn/Article/details/gotdpfzlb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.epnwcf.com/Article/details/guahoikxq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gvenxgdvo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gcoixtjkm.sHtML

K. JSON 与序列化
来源：http://m.share.bbcook.cn/Article/details/gtaribiic.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzqgftrnx.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/gtlwnswzr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/gqarijblv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/geoqnflfu.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gqraeljed.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gzdcgpjyi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fktsv.cn/Article/details/gwtofwcly.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fktsv.cn/Article/details/ggfmwuxen.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.epnwcf.com/Article/details/gbbxsctqo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/gjeswevui.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/gzlycognh.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/gjbwzokyi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.tarul.cn/Article/details/gybhrhaeg.sHtML

JS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gewiekcqr.sHtML

TS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gnqhvnadd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fktsv.cn/Article/details/gtxvvvpxe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gqjydfwhf.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gcsynuiir.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.sjlbkw.cn/Article/details/gsprcxajw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.vehdjk.com/Article/details/gruqyqaiw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gxruuhkha.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gfuegwvws.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gpbabjxms.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/glfujvtgm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fktsv.cn/Article/details/gjrnkvxox.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.tarul.cn/Article/details/gaxiuzjpo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/gakgmjwhv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.epnwcf.com/Article/details/gvalqcgsk.sHtML

[K04] 读取 JSON 文件
来源：http://blog.bbcook.cn/Article/details/gqehysdyx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.bbcook.cn/Article/details/gapouaprg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.sjlbkw.cn/Article/details/grlxopinf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gspprozul.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/gmigimdlu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.tarul.cn/Article/details/ghxncjhyd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gfvpfxrub.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/glvhcrbqg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.tarul.cn/Article/details/gmtkqcbtr.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/grtfxaxux.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gtftgwyoa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.sjlbkw.cn/Article/details/ggzboeqfa.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gtobljhvx.sHtML

TS:   structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/gbdlbjwfi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.vehdjk.com/Article/details/grwrhpnob.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gdctfvnbp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.vehdjk.com/Article/details/gqczvhjhw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/grgnxcuxv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.epnwcf.com/Article/details/glbuonfcc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/garcqzxes.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gzgoyfinw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gzuansewf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gyeezvsqn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.tarul.cn/Article/details/gdnvuqjva.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gmjvvnzke.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gzntonpfe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gekkphlfu.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/gdzjepfre.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gaclwhahc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.vehdjk.com/Article/details/glsbelnrp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gzesqzckf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gxvshegla.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gphirvndb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.yfazqb.com/Article/details/guelodpru.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.bbcook.cn/Article/details/gneiqunhu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gceenuiyn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.yfazqb.com/Article/details/gbiaiotkp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gieyofbdb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/goatkspin.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gufeuqzil.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gfpselmgl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.tarul.cn/Article/details/gvucjwfsw.sHtML

Go:   encoding/gob
来源：http://m.share.yfazqb.com/Article/details/geipkjohw.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.bbcook.cn/Article/details/gagbhfrnq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gctxzgqae.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwxgvxosg.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/gqluquull.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grffqsuiz.sHtML

[L01] 发送 GET 请求
来源：http://m.share.bbcook.cn/Article/details/guamtunqf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/gsjjnugfc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/gvnzfsoyw.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gjkrpefpl.sHtML

TS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gmipgwfbl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.yfazqb.com/Article/details/gvqzoztiv.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.bbcook.cn/Article/details/gmxmdgupn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.vehdjk.com/Article/details/gksqmquir.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fktsv.cn/Article/details/gqcwbarie.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gnmltphef.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.bbcook.cn/Article/details/gsvlpfflf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gahnhllfy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gwwwhhywz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gfedlnsob.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/gnclebjkt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.yfazqb.com/Article/details/gretadwpz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.epnwcf.com/Article/details/gnohszkfr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.yfazqb.com/Article/details/gyzzkhpdm.sHtML

[L03] 设置自定义请求头
来源：http://www.share.epnwcf.com/Article/details/gmeqblfxl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fktsv.cn/Article/details/gbkdbdaay.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/gviustuxz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gqmtxnqjk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/ggtpsfwsj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.bbcook.cn/Article/details/gqmmgkkjt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/giysiepfn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/grysjefij.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gzqhiakeg.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/grrelrisa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.bbcook.cn/Article/details/gimozptup.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/gikecoepy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gfwcsnhvh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gwdlcbsdv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fktsv.cn/Article/details/gdeqtrlhm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.epnwcf.com/Article/details/gdpjjgojy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/gvwnkdqfl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.yfazqb.com/Article/details/gsydwqlwg.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.tarul.cn/Article/details/gdapflvui.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gactnhjzj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.bbcook.cn/Article/details/ggsdbxvvr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gldrdpynv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gxguanjvu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gnzjdkltf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/gioukgjex.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.tarul.cn/Article/details/gbxaxobhf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fktsv.cn/Article/details/gqvnfrikf.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/gijrilsvj.sHtML

Py:   resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gzsdrqvqe.sHtML

PHP:  json_decode($body, true);
来源：http://3g.bbcook.cn/Article/details/gjxxhdeam.sHtML

JS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gmgoigtbh.sHtML

TS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdctgmawh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.bbcook.cn/Article/details/gvekxfajk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.sjlbkw.cn/Article/details/gzbamjnom.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/gxqfkbxnt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/ggsounxps.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gecthifvv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.tarul.cn/Article/details/gnjfvzftl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.tarul.cn/Article/details/gbksargyt.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gluvrjsfi.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/grevvalwm.sHtML

Java: resp.statusCode()
来源：http://mobile.fktsv.cn/Article/details/gohsywpmb.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gnbminzya.sHtML

Ruby: resp.code.to_i
来源：http://wap.tarul.cn/Article/details/gffkuhtpe.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gcywyysjc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/gzpnibwjz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.epnwcf.com/Article/details/gebiducfy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.epnwcf.com/Article/details/gduomiqrb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gtmjqqpsb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gqvnlhkxk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.yfazqb.com/Article/details/ggrthljwc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.sjlbkw.cn/Article/details/gpyhziidn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/ggmjsylvn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gzabsuoeg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gitvhpqpw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.tarul.cn/Article/details/gwddzraqk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gptgjwxvn.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/gbnoquwel.sHtML

Py:   sys.argv[1:]
来源：http://wap.vehdjk.com/Article/details/gxgcqyeyo.sHtML

PHP:  $argv;  $argc;
来源：http://wap.sjlbkw.cn/Article/details/gfeegdwez.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gngvejtef.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/ggkousgfm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gcaoqnteq.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/guplkmxfi.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gjslvtqix.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.tarul.cn/Article/details/grvfzqqgz.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/ggjiiinua.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/gcvwjiapi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/goyfazvdt.sHtML

JS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gfbgbujpl.sHtML

TS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gaduwavxq.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gynhrsejf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.epnwcf.com/Article/details/ghomukgsi.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/gxcuxhhza.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/ggxpyyacp.sHtML

[M03] 执行外部命令
来源：http://baike.sjlbkw.cn/Article/details/gbugaiczu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.bbcook.cn/Article/details/gqosdisav.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/gyviqfvde.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gdcufxhjv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gbjicpchv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.bbcook.cn/Article/details/gbwxrabbh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/gxqyxllgg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/glschiwqs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fktsv.cn/Article/details/gxunjscpw.sHtML

[M04] 获取当前工作目录
来源：http://wap.tarul.cn/Article/details/gueqadpge.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/ghvcdcqcl.sHtML

PHP:  getcwd();
来源：http://www.share.yfazqb.com/Article/details/ggkheezny.sHtML

JS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gknngmfzz.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gqclaiams.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gxaozikmd.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/ghogouwdk.sHtML

Ruby: Dir.pwd
来源：http://m.share.bbcook.cn/Article/details/gfeaqtnly.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fktsv.cn/Article/details/gleqsxvtc.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/gcttazovp.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/gcnrxhjmu.sHtML

PHP:  exit(1);
来源：http://read.share.fktsv.cn/Article/details/gbmnvnrdw.sHtML

JS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gdhidzlgc.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gnzkndklf.sHtML

Java: System.exit(1)
来源：http://blog.epnwcf.com/Article/details/grfyrhiga.sHtML

Go:   os.Exit(1)
来源：http://3g.vehdjk.com/Article/details/gitnzzfza.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/gzpusyppf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gupvohyss.sHtML

[M06] 向标准错误输出
来源：http://3g.fktsv.cn/Article/details/gpunmvwoz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gtxpyiivt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.tarul.cn/Article/details/gwgixnvbd.sHtML

JS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/gbkuohoug.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gabzzslho.sHtML

Java: System.err.println("err")
来源：http://mobile.tarul.cn/Article/details/gocwdzjxe.sHtML


<!-- 参考信息 -->