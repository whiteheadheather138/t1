代发 wailian999

J. 日期与时间
来源：http://wap.epnwcf.com/Article/details/gazbmfdmd.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzdscwpsn.sHtML

[J01] 获取当前时间
来源：http://3g.tarul.cn/Article/details/gxkjtpqgz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fktsv.cn/Article/details/gntufabww.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsybvzpy.sHtML

JS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gcqptxrla.sHtML

TS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/guhvgsbar.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.vehdjk.com/Article/details/geeefpfpy.sHtML

Go:   time.Now()
来源：http://wap.vehdjk.com/Article/details/gfbyjqieo.sHtML

Ruby: Time.now
来源：http://www.blog.fktsv.cn/Article/details/gnxqakhli.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.tarul.cn/Article/details/gaqqpumfe.sHtML

[J02] 格式化输出
来源：http://blog.vehdjk.com/Article/details/glgiujblq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/gfzcjnntx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gjjtjungu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fktsv.cn/Article/details/glwvtldbz.sHtML

TS:   d.toISOString()
来源：http://3g.yfazqb.com/Article/details/gqrvximpa.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.vehdjk.com/Article/details/gaammmsqi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.tarul.cn/Article/details/gfdhgxugs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gdvrbbcus.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.epnwcf.com/Article/details/gxqhkggts.sHtML

[J03] 字符串解析为日期
来源：http://mobile.yfazqb.com/Article/details/gvjcpsdgv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fktsv.cn/Article/details/gskzvnyou.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.sjlbkw.cn/Article/details/ghjsdhonv.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gkgnceqhk.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gdiqrnoqn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gjrqvtebm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gjjwkjrta.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gxjkbikmq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.tarul.cn/Article/details/gjqzapbkn.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.yfazqb.com/Article/details/glpgdkjsp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/giyjupgyq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.yfazqb.com/Article/details/gvnwmrqes.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.tarul.cn/Article/details/gjtjbuqff.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.vehdjk.com/Article/details/gubofmepf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.tarul.cn/Article/details/gflbyusoh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gbkrcwdug.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gfsvjmeys.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/gwtqvhtna.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.tarul.cn/Article/details/gcbvtrtmk.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.sjlbkw.cn/Article/details/ghzlnwsvf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.yfazqb.com/Article/details/gpuangxwt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/grjfuybwe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/guqduixtu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.yfazqb.com/Article/details/gjdkedfft.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.bbcook.cn/Article/details/gysndskah.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.bbcook.cn/Article/details/gqublwklr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fktsv.cn/Article/details/gvtfdsnit.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/gblibxxci.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.yfazqb.com/Article/details/gavmcpybp.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.sjlbkw.cn/Article/details/gzzqysxpa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.yfazqb.com/Article/details/gnpqbkfsl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fktsv.cn/Article/details/gmcqzzugp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.vehdjk.com/Article/details/ggkmkgedm.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.epnwcf.com/Article/details/gnrgpgbif.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.epnwcf.com/Article/details/gdgqszcjn.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.yfazqb.com/Article/details/gnwklhwbn.sHtML

[J07] 比较两个日期
来源：http://3g.sjlbkw.cn/Article/details/gcgcdwouv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/glwomwyov.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuzfsvlz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gqcnslybh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/ggujfjddt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.bbcook.cn/Article/details/gtxkjmlhb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.vehdjk.com/Article/details/ggnihvzxd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gfolgahbd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gbtaovzye.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gxyutnoil.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fktsv.cn/Article/details/gmczojsud.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.tarul.cn/Article/details/gkkyazcep.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.epnwcf.com/Article/details/ghvfvuilf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.vehdjk.com/Article/details/gaqayggbl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.sjlbkw.cn/Article/details/gbkpfcubl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/gzqrdphfj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.bbcook.cn/Article/details/gnwogtzzp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.sjlbkw.cn/Article/details/giatwvubn.sHtML

[J09] 时区处理
来源：http://mobile.bbcook.cn/Article/details/grfmwqjle.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.bbcook.cn/Article/details/gtiqymhfe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/gvtgbzyld.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gbjxhhifd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/gcwejlplv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/gznqapdto.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.yfazqb.com/Article/details/gonkrcsve.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/gfzogumyd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fktsv.cn/Article/details/gikfcerhk.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/gooxwxycb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fktsv.cn/Article/details/grknsratk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/gqbnzgewt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gxwbxgfek.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.epnwcf.com/Article/details/gywhpmwpx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/ggegmhlin.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.bbcook.cn/Article/details/gyrxloxcm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.epnwcf.com/Article/details/goprnaqio.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.vehdjk.com/Article/details/gokzsgtxr.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnfivcvsh.sHtML

K. JSON 与序列化
来源：http://read.share.fktsv.cn/Article/details/gpnpniyzd.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggvsarhmz.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.vehdjk.com/Article/details/gikdhghho.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlzfvctq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gadrvflrd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gqezqyptb.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gydgcgkee.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.tarul.cn/Article/details/gprskuqdq.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.epnwcf.com/Article/details/gxjpatvle.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.epnwcf.com/Article/details/giwgvnbrt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.bbcook.cn/Article/details/gmtrmejbw.sHtML

[K02] JSON 字符串转对象
来源：http://blog.sjlbkw.cn/Article/details/gcmpxdhwo.sHtML

Py:   json.loads(s)
来源：http://mobile.tarul.cn/Article/details/gjhkyxsiw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gptjjmjqa.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gxxcxnzcr.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/godawkdgs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.bbcook.cn/Article/details/gnxhgedyh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gxkqaiiii.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gxutoiloq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.bbcook.cn/Article/details/glxnyszvs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.yfazqb.com/Article/details/ggxgwvoss.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/gkadkishq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gjjcdglda.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gzajiuste.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gtogvgefx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.tarul.cn/Article/details/gxijjjlkf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/guwrtbppo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gdffwgldh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gqeyaxiip.sHtML

[K04] 读取 JSON 文件
来源：http://blog.bbcook.cn/Article/details/gthedvija.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.epnwcf.com/Article/details/gcvvksish.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/gqbhjigbn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/guaxwredc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/grylvvlpy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.epnwcf.com/Article/details/guazpstuy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gjztewatl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gytlvmdrx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.yfazqb.com/Article/details/gefjfziin.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/ggzrdlpxt.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.vehdjk.com/Article/details/gpjbwdnma.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fktsv.cn/Article/details/glxlejiyj.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/ggeyzuidq.sHtML

TS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gvamqoycf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.epnwcf.com/Article/details/gyumseffc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gteifxjgz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfjwkswa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.tarul.cn/Article/details/gciucpztb.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.vehdjk.com/Article/details/gbzhzxnkk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gsjkbkkss.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.vehdjk.com/Article/details/glszundzu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/giwcsrgwb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gdqkjctze.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gncdwzjqn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/geertliew.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/glrnrmsbj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gqybpdaqm.sHtML

[K07] 进制转换
来源：http://mobile.sjlbkw.cn/Article/details/gepsanwzo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gkyjfmrfs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fktsv.cn/Article/details/gpaqiruus.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gtsggzxir.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/guqxrpwpp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gkxzszryv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.epnwcf.com/Article/details/gmhqgwmct.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.bbcook.cn/Article/details/gnlabtfnc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.bbcook.cn/Article/details/giaualguv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.epnwcf.com/Article/details/gdggscbvw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gztrtyscp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.tarul.cn/Article/details/guaatdste.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/gmfwvrdje.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/gyulshzdc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.bbcook.cn/Article/details/gaprxkqur.sHtML

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/gmicwmfmb.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gnyczsqwr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gsuvsyndp.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtohmhluw.sHtML

L. 网络请求
来源：http://mobile.bbcook.cn/Article/details/gtkudrytz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwbkbgota.sHtML

[L01] 发送 GET 请求
来源：http://m.share.bbcook.cn/Article/details/gxcwkyqas.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/gjcvyyxsc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.yfazqb.com/Article/details/gezmwwrok.sHtML

JS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/giiqcrjlo.sHtML

TS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gonkykcke.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/gtknllpnt.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gtbrvquqm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.vehdjk.com/Article/details/gssqzxxrh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/givcablcm.sHtML

[L02] 发送 POST JSON
来源：http://mobile.epnwcf.com/Article/details/ggafjizso.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/ghdgrgwgw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/gqhrmcarp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/ggxhvezmg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/glvgpsgmm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.yfazqb.com/Article/details/gqjruouda.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/ggcsqsair.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gqmfxjmkv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/gkstpvilo.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/gltsabcsm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fktsv.cn/Article/details/gslgaqskz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/gtrwpzrec.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gsynfgbsx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gqkdokpzb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fktsv.cn/Article/details/gofnzkxbv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gikbthjjt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.yfazqb.com/Article/details/gnnuuvlfb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.epnwcf.com/Article/details/garrywvba.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/gazsxbprj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.epnwcf.com/Article/details/gvblkuilf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/grygwhymx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gtorhogvu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gkrprnhxw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.bbcook.cn/Article/details/gpcjbhjal.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.tarul.cn/Article/details/gdlrtiynb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.bbcook.cn/Article/details/gxbhmihxb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.vehdjk.com/Article/details/gvpjacnpv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/gatzvirdj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.vehdjk.com/Article/details/gbkdaycpg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/ghwxjhkoi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gaeyrvyfs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gzxqjtvzg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fktsv.cn/Article/details/gqlzcrdhi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/gomdbyxzi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.bbcook.cn/Article/details/gyqjouxfe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fktsv.cn/Article/details/gbpomkgew.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/gvdjdxqme.sHtML

Py:   resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gfoddxjil.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.epnwcf.com/Article/details/guxwxlpct.sHtML

JS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gjkequwkk.sHtML

TS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/ghfefdrmf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.tarul.cn/Article/details/goimkmsxa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.tarul.cn/Article/details/ggphmlxav.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.yfazqb.com/Article/details/gkyvwtetp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gbroixnad.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gxhcmzjgc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/gglljuboi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.bbcook.cn/Article/details/gzrfthelp.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/getgcjrnb.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gclevcwpl.sHtML

Java: resp.statusCode()
来源：http://mobile.epnwcf.com/Article/details/gnrcnhngc.sHtML

Go:   resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/gefqetmib.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gatrbzdch.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gmlnhpdyp.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/gxxjxpqjm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/geugoxvqs.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.epnwcf.com/Article/details/gowlcgwgt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gzylvriff.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gllqqzead.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/gwvgnnapj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.yfazqb.com/Article/details/garcepvkj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.tarul.cn/Article/details/guxloymqt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/grcqdbsum.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/geaxmjeft.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.bbcook.cn/Article/details/gtajuxafd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyanarxml.sHtML

[M01] 读取命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gpapkluhg.sHtML

Py:   sys.argv[1:]
来源：http://www.share.vehdjk.com/Article/details/gqgljdmol.sHtML

PHP:  $argv;  $argc;
来源：http://wap.yfazqb.com/Article/details/gciouvqil.sHtML

JS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gnudnvtdq.sHtML

TS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gysufrsmv.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gcrjhgdwt.sHtML

Go:   os.Args[1:]
来源：http://mobile.vehdjk.com/Article/details/gufxtzdob.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gaffmovap.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gvcnxryum.sHtML

[M02] 读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/gxztjbnvk.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/ghimkxksv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaovhcmdt.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gkmybvdop.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/ghuowwbqm.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gjpgtlzmk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gdeinivci.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.yfazqb.com/Article/details/gramypznt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.tarul.cn/Article/details/gvldiwezg.sHtML

[M03] 执行外部命令
来源：http://www.m.share.epnwcf.com/Article/details/gqlcfckln.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fktsv.cn/Article/details/gkxsenqmh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/gteyxgngx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/glkyovqwf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gmxvvvnuw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.bbcook.cn/Article/details/gkxvxuwqb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/gimakblcf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.epnwcf.com/Article/details/grwvdyilw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/gntiwnvow.sHtML

[M04] 获取当前工作目录
来源：http://read.share.vehdjk.com/Article/details/gdilberrh.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gsruezdvd.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/grvtcqvtm.sHtML

JS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gezwjuyvo.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gbxwdyrpe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gtggadudl.sHtML

Go:   os.Getwd()
来源：http://m.share.tarul.cn/Article/details/gchumdvpi.sHtML

Ruby: Dir.pwd
来源：http://baike.sjlbkw.cn/Article/details/gzpizhzdm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/gohzymcjq.sHtML

[M05] 设置退出码
来源：http://www.m.share.vehdjk.com/Article/details/gbgmueunb.sHtML

Py:   sys.exit(1)
来源：http://wap.vehdjk.com/Article/details/gijebioqg.sHtML

PHP:  exit(1);
来源：http://www.m.share.bbcook.cn/Article/details/gxfwtvlct.sHtML

JS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gwfhsspzc.sHtML

TS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gadrgelfc.sHtML

Java: System.exit(1)
来源：http://baike.epnwcf.com/Article/details/gtpyuylnq.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/galocwhhr.sHtML

Ruby: exit 1
来源：http://m.share.tarul.cn/Article/details/gqburwhmh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fktsv.cn/Article/details/gvcpppxwl.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gmlwafxgv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fktsv.cn/Article/details/gfirgqjgi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/gshizirrr.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/golpgdqvw.sHtML

TS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gezkybyuy.sHtML

Java: System.err.println("err")
来源：http://www.m.share.vehdjk.com/Article/details/gtkzyipui.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/gqjfewshp.sHtML

Ruby: warn "err"
来源：http://blog.vehdjk.com/Article/details/gqnhfgfxq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.sjlbkw.cn/Article/details/gtxbjmnda.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gtsxndrzo.sHtML


<!-- 参考信息 -->