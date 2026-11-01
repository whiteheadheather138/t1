代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.sjlbkw.cn/Article/details/gaskxfrcp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.vehdjk.com/Article/details/gudgifmvr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gdrsnbezg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gshugjwef.sHtML

J. 日期与时间
来源：http://read.share.bbcook.cn/Article/details/gmejowrpy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwjdgvzip.sHtML

[J01] 获取当前时间
来源：http://3g.epnwcf.com/Article/details/gmhbgazxg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeuxzwtb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/galfmzjhl.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gyavaegrn.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gzugjuftp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.bbcook.cn/Article/details/gcitukkrq.sHtML

Go:   time.Now()
来源：http://wap.tarul.cn/Article/details/gwekvovan.sHtML

Ruby: Time.now
来源：http://m.share.sjlbkw.cn/Article/details/gxolgyuui.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.epnwcf.com/Article/details/gnityiylk.sHtML

[J02] 格式化输出
来源：http://www.share.vehdjk.com/Article/details/gnjfxhfjm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gdxgitmip.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gaxquhuqz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.vehdjk.com/Article/details/godxbicnu.sHtML

TS:   d.toISOString()
来源：http://wap.yfazqb.com/Article/details/gujyccuyp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.bbcook.cn/Article/details/ggkqgnlwh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.bbcook.cn/Article/details/gqyeqovpe.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/guipopmrj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.vehdjk.com/Article/details/gljcevcli.sHtML

[J03] 字符串解析为日期
来源：http://www.share.sjlbkw.cn/Article/details/gdyvohwav.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.yfazqb.com/Article/details/gygvyljco.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.yfazqb.com/Article/details/gnhfygwql.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/glgjtolqy.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gfnftyxnl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gcwnnwrsf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gnswjqqup.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gbeayeosw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.tarul.cn/Article/details/gvbnscevj.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.tarul.cn/Article/details/gpurpgszb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.epnwcf.com/Article/details/ghxmgccgd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fktsv.cn/Article/details/gorlxowrf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gctxxctlw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.vehdjk.com/Article/details/gaepophhn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gvonirhiu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gabhfunoi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.tarul.cn/Article/details/gswyhnyaz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.epnwcf.com/Article/details/gdjnbdbnx.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.yfazqb.com/Article/details/gbwqhfuga.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fktsv.cn/Article/details/gffvlcjqc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.sjlbkw.cn/Article/details/gxsiyarnk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gdsfuhjhg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gswrmxluf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.vehdjk.com/Article/details/gidguniom.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.epnwcf.com/Article/details/grkzvkyjy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/gmrdeabml.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/gytgrgods.sHtML

[J06] 计算两时间之差
来源：http://blog.fktsv.cn/Article/details/gjmwxvrpp.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.vehdjk.com/Article/details/gpsrsoulo.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.yfazqb.com/Article/details/gdfxdifnr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fktsv.cn/Article/details/gfrmuggez.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.sjlbkw.cn/Article/details/gugizlqys.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.vehdjk.com/Article/details/gwtanhnpa.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.sjlbkw.cn/Article/details/gclywtlwq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/gcwsxampl.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.bbcook.cn/Article/details/grqkzihzo.sHtML

[J07] 比较两个日期
来源：http://www.m.share.epnwcf.com/Article/details/gcarwhutn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/grancdcqn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.bbcook.cn/Article/details/gltykrbcw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gbwtfqceh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gjdwxfayx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.vehdjk.com/Article/details/gohsizuks.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gsrssgewu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/giajqclkh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gtsctwnrh.sHtML

[J08] 提取年月日与星期
来源：http://wap.fktsv.cn/Article/details/gqtxnvhvc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.sjlbkw.cn/Article/details/gysabuwmt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.yfazqb.com/Article/details/gxbmigkzd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/goasihkpt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.bbcook.cn/Article/details/glnzaetrf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.bbcook.cn/Article/details/gxmqddwlz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.tarul.cn/Article/details/gjgjmcxwj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.epnwcf.com/Article/details/gkxdzbrpw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/gbbffmowq.sHtML

[J09] 时区处理
来源：http://read.share.bbcook.cn/Article/details/gqeycjvpe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fktsv.cn/Article/details/gmduvtaje.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.vehdjk.com/Article/details/ghmlkacqq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/glibcupnb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/gonszqdjl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/ggrsrtiwp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.vehdjk.com/Article/details/gkcfltdzn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.bbcook.cn/Article/details/gnewnfqbv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.vehdjk.com/Article/details/gcwlepvfi.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.tarul.cn/Article/details/gyyuvsjsd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/ggdstnkfe.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.yfazqb.com/Article/details/gwlxcrqtq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.vehdjk.com/Article/details/gomoponaq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.epnwcf.com/Article/details/gdfqeplrn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gkhjxnjlm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fktsv.cn/Article/details/gbxmyomwc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.yfazqb.com/Article/details/gahvxtkac.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.yfazqb.com/Article/details/gbcouqipm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfjpfxfew.sHtML

K. JSON 与序列化
来源：http://wap.sjlbkw.cn/Article/details/gyhrycqan.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gidxuhvwf.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.bbcook.cn/Article/details/gjimvngbb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gmtzispyd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gpgroodhv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gstqpysds.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gmextjjkb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.bbcook.cn/Article/details/gdbkxtyhw.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.yfazqb.com/Article/details/geaywkejw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fktsv.cn/Article/details/gbbvqcloh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fktsv.cn/Article/details/gwxqyjijk.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/gyjmxkcue.sHtML

Py:   json.loads(s)
来源：http://m.share.bbcook.cn/Article/details/gbxpuaftt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.sjlbkw.cn/Article/details/gnwusbuwd.sHtML

JS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gbelkqjba.sHtML

TS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gywdcoemi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/gkzpqnkzq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gzjgwnxtz.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gyailnxxj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.bbcook.cn/Article/details/gmxzybkic.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/guqgduoru.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/ggizmcrae.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/galxruyam.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gzxdixxzy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/ghralxuyx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gjgsgzdct.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.sjlbkw.cn/Article/details/gnqehmfbr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.yfazqb.com/Article/details/gjrazjwsr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.epnwcf.com/Article/details/grshstfgs.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/ggcjyfmfe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.yfazqb.com/Article/details/gzpqlftfc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.sjlbkw.cn/Article/details/gehwmvdhk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gqgredoat.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gwouxjtlz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.epnwcf.com/Article/details/gghmeifin.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fktsv.cn/Article/details/gvvdwoler.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gvegnmbrz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.vehdjk.com/Article/details/guwqiswrz.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/gsbfmdixs.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.vehdjk.com/Article/details/giawqcqje.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fktsv.cn/Article/details/gymumywnx.sHtML

JS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gdoqfeggb.sHtML

TS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gmzwthcqk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.yfazqb.com/Article/details/gcwmvexkl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.tarul.cn/Article/details/gitltmuxo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.tarul.cn/Article/details/gbotspsce.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.sjlbkw.cn/Article/details/gjxwchbhb.sHtML

[K06] 解析 URL 查询串
来源：http://3g.bbcook.cn/Article/details/gnbnrmakq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gwssrlvis.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fktsv.cn/Article/details/gpcicryjn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gxmgesvoz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gfyzdcqbn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.tarul.cn/Article/details/gfhpzzbun.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gltdbarji.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/glbmhyfqx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/ggoufybju.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gsknopddv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.epnwcf.com/Article/details/ghxdjaths.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gdwwposqn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gydlhjmrr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gmpvsapbo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gthlwccha.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fktsv.cn/Article/details/gweagixhu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gljwkgfqe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gwbwmhfvs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.yfazqb.com/Article/details/gvidpmrft.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gnhwuofol.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.sjlbkw.cn/Article/details/grsyglvjl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gdfbtrwng.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gbsxogqsw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gswmvsryg.sHtML

Go:   encoding/gob
来源：http://baike.yfazqb.com/Article/details/gejkdxzcm.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fktsv.cn/Article/details/gokxqvsvc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.tarul.cn/Article/details/grtoqlvwn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gahuzqyat.sHtML

L. 网络请求
来源：http://www.m.share.vehdjk.com/Article/details/grxvcnyws.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ghnrzdmpi.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fktsv.cn/Article/details/gykuebfbs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.epnwcf.com/Article/details/geauzgqwk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/gwyacmgbk.sHtML

JS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/glmqpqpnp.sHtML

TS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gcxbcjzyx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.tarul.cn/Article/details/gtiphryaf.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.yfazqb.com/Article/details/gvhfzhbbo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/glmnuhmnz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/gzakknvrm.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/gdilzsdvh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gxxuyhuvb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/guqmyidlc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/grrzyqsdr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gfnmxtceg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.tarul.cn/Article/details/gbnjstnrh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.bbcook.cn/Article/details/gatkuxqza.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.vehdjk.com/Article/details/ghgfoboxm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggczihftq.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fktsv.cn/Article/details/gxvrwojup.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fktsv.cn/Article/details/gngztvecd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.sjlbkw.cn/Article/details/gurlxxfdi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gixiguyoe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fktsv.cn/Article/details/gnkaqvpra.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.tarul.cn/Article/details/ggyzcbbbm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/grfywhplg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.tarul.cn/Article/details/gozcpambj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gegadkegz.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/gcawihvbr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/gxnipkcvi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.yfazqb.com/Article/details/gcxsllmcf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gmdwvubqf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjjozdnf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.vehdjk.com/Article/details/gygecjczc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.yfazqb.com/Article/details/gawirfilx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.vehdjk.com/Article/details/gxoxnlegm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.vehdjk.com/Article/details/gylnobmps.sHtML

[L05] 上传文件（multipart）
来源：http://wap.bbcook.cn/Article/details/guvczmapt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/givcrlgaf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fktsv.cn/Article/details/ggdctwdjc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/grtvgtpuu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gccdqwxcz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.vehdjk.com/Article/details/gxzgqcexn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/gpuohglxv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.yfazqb.com/Article/details/gtvtzyfdq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/gsdlyovad.sHtML

[L06] 解析响应为 JSON
来源：http://wap.sjlbkw.cn/Article/details/gfbysllvg.sHtML

Py:   resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gpkjcsmso.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.epnwcf.com/Article/details/gchwipicr.sHtML

JS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/gosyrrwif.sHtML

TS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/glabwdwnk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gllyqglhj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.sjlbkw.cn/Article/details/gudzljpeq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.vehdjk.com/Article/details/gpdpojepi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.sjlbkw.cn/Article/details/ggybpycni.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/geappiouv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fktsv.cn/Article/details/gxoycqeaa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gvktovudr.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gqckkepzj.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gzyzmxoyq.sHtML

Java: resp.statusCode()
来源：http://blog.epnwcf.com/Article/details/gxtxohcgd.sHtML

Go:   resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/gyluijoda.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gtkujqonf.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gqezkoryu.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.epnwcf.com/Article/details/glerschka.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.bbcook.cn/Article/details/gkyamgsed.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fktsv.cn/Article/details/gqgbupnkk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/ggqczcglp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gpkiywyad.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/gmqnjlcsq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.sjlbkw.cn/Article/details/gsxdkjmbk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gexdjfcwj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fktsv.cn/Article/details/gvmqvltsh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gpjozmimg.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.bbcook.cn/Article/details/gwifckqpm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghqkdgucc.sHtML

[M01] 读取命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gugwrzzpy.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fktsv.cn/Article/details/gsoumbdyz.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.vehdjk.com/Article/details/ggdqrqzop.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/guejwatiu.sHtML

TS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gkafjyhkb.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/gkaboldei.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fktsv.cn/Article/details/gccoallyd.sHtML

Ruby: ARGV
来源：http://wap.bbcook.cn/Article/details/golvkbley.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gsajcmmzx.sHtML

[M02] 读取环境变量
来源：http://www.share.fktsv.cn/Article/details/goxkgnoad.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.vehdjk.com/Article/details/gmdvneaws.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gggqnxsty.sHtML

JS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gaaziqugb.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gsgkxcviq.sHtML

Java: System.getenv("HOME")
来源：http://wap.vehdjk.com/Article/details/goachtajr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.vehdjk.com/Article/details/gonieibjj.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/gwjdokpbx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.tarul.cn/Article/details/gtrayjcxs.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/gfljidxob.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/gtpbluibn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.tarul.cn/Article/details/gwxdrvdtu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gusdskymw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/ghqyquuxa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/gvtusmiqa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.tarul.cn/Article/details/gmnknesfk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/guemktlfa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fktsv.cn/Article/details/gmuigckvh.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/gyngywdes.sHtML

Py:   os.getcwd()
来源：http://www.share.bbcook.cn/Article/details/gjjrvvous.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/gxsdcjbfh.sHtML

JS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gumcmjorm.sHtML

TS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gpjavfjos.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gcwblkmds.sHtML

Go:   os.Getwd()
来源：http://baike.fktsv.cn/Article/details/gcvqadxaz.sHtML

Ruby: Dir.pwd
来源：http://wap.epnwcf.com/Article/details/giyjmlivn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.epnwcf.com/Article/details/gisbxuabo.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gvsmzcsha.sHtML

Py:   sys.exit(1)
来源：http://wap.fktsv.cn/Article/details/galsvijuy.sHtML

PHP:  exit(1);
来源：http://read.share.tarul.cn/Article/details/gxzazousm.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gmcktbyay.sHtML

TS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gmqonrzsn.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/giuwwdrjj.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gpyjpyrlv.sHtML

Ruby: exit 1
来源：http://www.share.bbcook.cn/Article/details/gvnfgyrdt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.yfazqb.com/Article/details/gplzcwrwk.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gjvqhmizv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gvscezgcc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fktsv.cn/Article/details/gudsixanm.sHtML

JS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/geroqacst.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gxkhmswnd.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/gubxdnhnt.sHtML


<!-- 参考信息 -->