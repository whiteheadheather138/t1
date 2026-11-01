代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.yfazqb.com/Article/details/gqrnwvqbu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.vehdjk.com/Article/details/gwshhjwtp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gvwjvmxcn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.bbcook.cn/Article/details/gvzzqepbl.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/gocwxwuhm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.tarul.cn/Article/details/glkhrhqaj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.bbcook.cn/Article/details/gautlcrfn.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/garrkhepx.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/guntecftu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/guipgizii.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gaedvzbzz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/giqdrrdzo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.yfazqb.com/Article/details/gispintlt.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fktsv.cn/Article/details/gksjipoxl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.tarul.cn/Article/details/glookwooa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.bbcook.cn/Article/details/gcelyrsmi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.tarul.cn/Article/details/gosivdcqy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.sjlbkw.cn/Article/details/ghggepnjm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.epnwcf.com/Article/details/gjpijblbb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.yfazqb.com/Article/details/gxefpaikk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.yfazqb.com/Article/details/ghjdivull.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.yfazqb.com/Article/details/gfbaplpcv.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.tarul.cn/Article/details/guaejnvnr.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.yfazqb.com/Article/details/gmbkapqrg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/ghqoilkkf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/gcxutilih.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gkexjliuq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fktsv.cn/Article/details/gjgqmqnen.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fktsv.cn/Article/details/gfwfvnagt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.sjlbkw.cn/Article/details/gognpukvj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fktsv.cn/Article/details/goanfshpb.sHtML

[J06] 计算两时间之差
来源：http://baike.tarul.cn/Article/details/gzvlpbceh.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gkrkkkafp.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.vehdjk.com/Article/details/gpzgpmipc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fktsv.cn/Article/details/gxfcbexpw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.vehdjk.com/Article/details/gkdkqauft.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.bbcook.cn/Article/details/gddxjkrkn.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.tarul.cn/Article/details/gixpwphhf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.sjlbkw.cn/Article/details/galbpkddw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.epnwcf.com/Article/details/glojqkdom.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/ghupzsldy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gxrpslcvz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.sjlbkw.cn/Article/details/gjdkrwxhl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gaiigrrbj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/grgbgfefz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/gdbwdxuxv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.yfazqb.com/Article/details/glitfjanr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gsloyaiac.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gtrpwquiz.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/gygdsxoml.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.yfazqb.com/Article/details/gnlqmatjm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.vehdjk.com/Article/details/gafqfsvew.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.tarul.cn/Article/details/gkryiyfrq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.yfazqb.com/Article/details/gebjriljr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.yfazqb.com/Article/details/ghmhjyqrh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.tarul.cn/Article/details/gdwwpejky.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fktsv.cn/Article/details/gbrmdcgdj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.bbcook.cn/Article/details/gbfirtqfg.sHtML

[J09] 时区处理
来源：http://3g.bbcook.cn/Article/details/gskcpbtsu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.tarul.cn/Article/details/gxgrqomjh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.tarul.cn/Article/details/gtkczoqov.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/gasoxjlzx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/gnudwslmm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.epnwcf.com/Article/details/gxbzvttfz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fktsv.cn/Article/details/gfdxkaqab.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.vehdjk.com/Article/details/ghtatcrrj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.bbcook.cn/Article/details/gudycxbtg.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fktsv.cn/Article/details/gucjgwfvv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.tarul.cn/Article/details/gsdpuehvr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.yfazqb.com/Article/details/gskmvdwdw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.epnwcf.com/Article/details/gchzqmjfm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/grcygjqmn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.yfazqb.com/Article/details/gqjrjpjiu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.vehdjk.com/Article/details/gwxbybsrv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.bbcook.cn/Article/details/grodxuoue.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gpeywziwt.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzwhrntgh.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gdttxbhyl.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/givemiqav.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.tarul.cn/Article/details/gvmtuoblg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gduixrlzb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gajsngsin.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gbfswuxyq.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gvrtkjsub.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fktsv.cn/Article/details/ghqzxcrdl.sHtML

Go:   json.Marshal(obj)
来源：http://wap.sjlbkw.cn/Article/details/gcgpeoigs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fktsv.cn/Article/details/gmiyhtcpa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gndiuymhh.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.yfazqb.com/Article/details/gxudclxyn.sHtML

Py:   json.loads(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gawrqbqsc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.sjlbkw.cn/Article/details/glidladjm.sHtML

JS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gpxhhcwne.sHtML

TS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gikippdql.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.yfazqb.com/Article/details/gyudjqnus.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/gpmtpdggu.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/giqjsvttu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.yfazqb.com/Article/details/giurnqywm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/gkycripyo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/ghneduseu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gihjhgrcr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gjgesdczl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gfjwwxdtr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gmfvdgnam.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.epnwcf.com/Article/details/gluuqdcxq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gsbracqci.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.bbcook.cn/Article/details/gkfykmtaw.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/ggptmymcd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.bbcook.cn/Article/details/gqoyudvaq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.yfazqb.com/Article/details/ghowcbnaz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/girtpkury.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gmngsfjmj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.tarul.cn/Article/details/gteuqkbpu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/ggkkupsnq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gwnncbplb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fktsv.cn/Article/details/goexywexv.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkghbcjh.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.sjlbkw.cn/Article/details/gqeecablu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fktsv.cn/Article/details/grcqihisu.sHtML

JS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/grdjuwjcc.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/ghgzkqttj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/ggeavvdtd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gesuhzhon.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.tarul.cn/Article/details/gzwpgvsml.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gdphpbsna.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.vehdjk.com/Article/details/gftzbmitb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/goozhdaos.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.bbcook.cn/Article/details/gznllkcqu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/ghcatnqxd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gdkwxhycb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.vehdjk.com/Article/details/gbugwqcey.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gwrobtydp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gsbwfmupk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gufpyfvql.sHtML

[K07] 进制转换
来源：http://wap.epnwcf.com/Article/details/gezpygchr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gpbearnkr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gsxmobymo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/ggaeewslg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/ghxhcleac.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gacrqqowh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/gmxrjgtjc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gknxcqwri.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gboeesits.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.sjlbkw.cn/Article/details/gpbgkburo.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gcghthijz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.sjlbkw.cn/Article/details/gphjgztct.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gszeqliik.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gdtsvptnq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.epnwcf.com/Article/details/gbvclydtj.sHtML

Go:   encoding/gob
来源：http://www.share.sjlbkw.cn/Article/details/gwibrgryd.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.tarul.cn/Article/details/gnxefnwac.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.bbcook.cn/Article/details/grygqjocy.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/guhamyxpp.sHtML

L. 网络请求
来源：http://blog.yfazqb.com/Article/details/ggvrlytth.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpgrblemk.sHtML

[L01] 发送 GET 请求
来源：http://3g.epnwcf.com/Article/details/gnfejgnrr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/gwgmkurmw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/gwedqsmvj.sHtML

JS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/gtlkjmise.sHtML

TS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gyukaxlkr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.bbcook.cn/Article/details/gacqwjxej.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gfhsuoeaw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.vehdjk.com/Article/details/gfrxmlvat.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/gmncbkxhk.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gaeqbsgdj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/gfmxfmgex.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fktsv.cn/Article/details/guvrtzdmt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gacfbxfwn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/gntkvmtfy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.sjlbkw.cn/Article/details/gpbgircpe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fktsv.cn/Article/details/gstgvoaxr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.epnwcf.com/Article/details/gpresnnlt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gdkvzdtus.sHtML

[L03] 设置自定义请求头
来源：http://baike.vehdjk.com/Article/details/gfgasbuns.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.vehdjk.com/Article/details/gpceaelme.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.sjlbkw.cn/Article/details/gfjhabwum.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gnyicgfqa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gvnbuqymf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fktsv.cn/Article/details/gebcklvdy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gfmdzgrwc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.yfazqb.com/Article/details/gaxddtpcp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gzobuextd.sHtML

[L04] 设置超时
来源：http://read.share.yfazqb.com/Article/details/gplmwnxlk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/gqusytrhe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.vehdjk.com/Article/details/galflrttp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gcouqduym.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gpjhuudca.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqkjvjvf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.sjlbkw.cn/Article/details/gxshiunrx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/guxwarsuq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.bbcook.cn/Article/details/gneipzgbw.sHtML

[L05] 上传文件（multipart）
来源：http://3g.epnwcf.com/Article/details/gibdlufnr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.vehdjk.com/Article/details/gvqedjetb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.epnwcf.com/Article/details/gfeixtzcj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gmghwmuvm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gqlumabaf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.yfazqb.com/Article/details/gptkkhxwk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.tarul.cn/Article/details/gxpmgigmm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/gbtplklif.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.bbcook.cn/Article/details/ggjrqeqnd.sHtML

[L06] 解析响应为 JSON
来源：http://baike.bbcook.cn/Article/details/gglxzykkh.sHtML

Py:   resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gibrezewl.sHtML

PHP:  json_decode($body, true);
来源：http://3g.bbcook.cn/Article/details/gtahvuibs.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gxhpnsuwu.sHtML

TS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gkpkevyux.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.vehdjk.com/Article/details/gdhozaxvq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/gvdwtzqxu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gslrorybl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gedssqzqn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gcvbzuljw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.sjlbkw.cn/Article/details/gthkyjydv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.sjlbkw.cn/Article/details/gfihptiah.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gumkwzngy.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gqsngmaux.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/galfyctan.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gzmqjrtro.sHtML

Ruby: resp.code.to_i
来源：http://3g.sjlbkw.cn/Article/details/glbmafhhn.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gxdvhfqlx.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gmfhuiece.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.tarul.cn/Article/details/glmovxqcy.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.bbcook.cn/Article/details/gduqdsyqj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/ggbmyhcma.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gevjqwdft.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fktsv.cn/Article/details/gyddpisgi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fktsv.cn/Article/details/gtcxcetju.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gtkthpxdc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gbpiffzht.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/geflqnugz.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gncitikyq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxduityky.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gsukqeqpp.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/gwzkiyymb.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/gfrqqzbrc.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gksywibui.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/glxhjqjfh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gtujvfjrm.sHtML

Go:   os.Args[1:]
来源：http://baike.yfazqb.com/Article/details/giuqxotlz.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/gwtjidkad.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gpaypmgvc.sHtML

[M02] 读取环境变量
来源：http://wap.fktsv.cn/Article/details/gmkquttsb.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.bbcook.cn/Article/details/gcnfhvxxn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gueqboxna.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/guwdmpnee.sHtML

TS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gfzputtus.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gpmszvmxm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gepstnykp.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gmwpojkmf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.bbcook.cn/Article/details/gymnydynx.sHtML

[M03] 执行外部命令
来源：http://blog.vehdjk.com/Article/details/givasyqie.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gqxuohvnv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/gcwcgknsd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/golbbzaxk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gxtwonmfx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.vehdjk.com/Article/details/gjzvlrscm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.vehdjk.com/Article/details/gimpvzcep.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/garbogykh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fktsv.cn/Article/details/gpjrjlzcq.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gkehqtalx.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/goaxywfxx.sHtML

PHP:  getcwd();
来源：http://www.blog.sjlbkw.cn/Article/details/gbyvmxnly.sHtML

JS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gnymuwpih.sHtML

TS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gzgpdqdus.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/gpgfkdzhm.sHtML

Go:   os.Getwd()
来源：http://read.share.sjlbkw.cn/Article/details/gescwtyce.sHtML

Ruby: Dir.pwd
来源：http://mobile.tarul.cn/Article/details/gqqyuuciz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fktsv.cn/Article/details/gulnvoied.sHtML

[M05] 设置退出码
来源：http://blog.sjlbkw.cn/Article/details/gystezdwo.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gyldfysgb.sHtML

PHP:  exit(1);
来源：http://read.share.fktsv.cn/Article/details/gocvagckf.sHtML

JS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gmmftjmcb.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gaxoyorlu.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gaxoycbuh.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gbqjbdtql.sHtML

Ruby: exit 1
来源：http://www.blog.bbcook.cn/Article/details/glgzfrvai.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gwlhamntr.sHtML

[M06] 向标准错误输出
来源：http://m.share.yfazqb.com/Article/details/gcmsgjcql.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gbnqyehqm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.sjlbkw.cn/Article/details/gneeuiivy.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gmkpkljua.sHtML

TS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/guouhpvri.sHtML

Java: System.err.println("err")
来源：http://www.m.share.vehdjk.com/Article/details/gfgtmngit.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/geqgsnkby.sHtML

Ruby: warn "err"
来源：http://www.m.share.vehdjk.com/Article/details/gstymsmtp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.epnwcf.com/Article/details/ghsaukuhe.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fktsv.cn/Article/details/gtdeuxofx.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.vehdjk.com/Article/details/gyqoopyje.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.epnwcf.com/Article/details/ghazucnar.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gseiuuzdi.sHtML

TS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gakuhkdyk.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/gjthpwdpo.sHtML

Go:   func main()
来源：http://wap.yfazqb.com/Article/details/gyorumjnt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gvvyupmpq.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/geupsgfyd.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gsakqlurs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/goavivztm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.sjlbkw.cn/Article/details/gqwaupesx.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/ghucylbrf.sHtML

TS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gzvkapzie.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/grvshohsj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.tarul.cn/Article/details/gtoshvjcb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/gpstopuft.sHtML


<!-- 参考信息 -->