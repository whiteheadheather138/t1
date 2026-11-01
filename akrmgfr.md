代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gfippulqt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/gqmschylj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.epnwcf.com/Article/details/grlijgdub.sHtML

TS:   d.toISOString()
来源：http://blog.tarul.cn/Article/details/gbzohuasq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fktsv.cn/Article/details/gkvzbknkj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.vehdjk.com/Article/details/gtkiymycr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/galjbctdo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.sjlbkw.cn/Article/details/gqszonukm.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fktsv.cn/Article/details/gxkylhsdc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fktsv.cn/Article/details/gwzvfprkq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.vehdjk.com/Article/details/gevljvhef.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gybwxghqx.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gxaxdvsyu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gcdzpihlh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gheifojzr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/givfrobwc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.vehdjk.com/Article/details/gapjolxhz.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.vehdjk.com/Article/details/geoyaxzul.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.vehdjk.com/Article/details/ghgxvkkyd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fktsv.cn/Article/details/gucauvnqc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.vehdjk.com/Article/details/gndzshvbv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.epnwcf.com/Article/details/gwyvkpplb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gdijnbrhg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/gqgkdwgur.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.vehdjk.com/Article/details/gbezzapnk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.bbcook.cn/Article/details/gyvkriftx.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/grtyrkznj.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.vehdjk.com/Article/details/gsfplkpmh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.sjlbkw.cn/Article/details/geetgyxkm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.tarul.cn/Article/details/gawctknqt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gqpavuwyy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.tarul.cn/Article/details/gxwdpakls.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.yfazqb.com/Article/details/glisgvapx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.tarul.cn/Article/details/gzhnemryp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.yfazqb.com/Article/details/gxzwcffyy.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/gievbyztx.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.tarul.cn/Article/details/gsiqdfyqk.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gbptfttaq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.sjlbkw.cn/Article/details/gmygcmwxm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.bbcook.cn/Article/details/gnztqcpgz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.yfazqb.com/Article/details/gzxjqvqmu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.vehdjk.com/Article/details/gpylfazcg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.vehdjk.com/Article/details/gauzwbujk.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.epnwcf.com/Article/details/gopkdvlhy.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/gvtcdchmk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gxxtouvrp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fktsv.cn/Article/details/gidhygrnc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/guqlsuves.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gezrzmtao.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.tarul.cn/Article/details/gtjocspvk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fktsv.cn/Article/details/gsnqyhfqu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gjwbggweo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/ggaxddrnm.sHtML

[J08] 提取年月日与星期
来源：http://blog.bbcook.cn/Article/details/glbdkoays.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.epnwcf.com/Article/details/gsuxxvhyf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.epnwcf.com/Article/details/gnfinzmws.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.epnwcf.com/Article/details/gvqdymffa.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/gbtmbiihj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/gltlwezxa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.yfazqb.com/Article/details/geowuiyvu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.vehdjk.com/Article/details/giwfsreoi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.vehdjk.com/Article/details/gpdztutaj.sHtML

[J09] 时区处理
来源：http://mobile.bbcook.cn/Article/details/gerysbjxw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fktsv.cn/Article/details/gwyojxlan.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.sjlbkw.cn/Article/details/gtbsfwemt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/grcypledw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gylsqtjbo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gayjmauiu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/gvbacopqs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/gkreoblxr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/glucrnmih.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.vehdjk.com/Article/details/gzscorbnr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.tarul.cn/Article/details/gifahpkuv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fktsv.cn/Article/details/goyirkmbt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.epnwcf.com/Article/details/grdqadtww.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.epnwcf.com/Article/details/gmzadkrip.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.yfazqb.com/Article/details/gyrpujtyp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gkmbhbgyr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.epnwcf.com/Article/details/gxycdhvkh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/gansjomcd.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gmsnjcgmy.sHtML

K. JSON 与序列化
来源：http://www.blog.fktsv.cn/Article/details/gadgsakzz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxzkoueny.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.epnwcf.com/Article/details/geguwxizw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gjespdlmf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/glcfqjsln.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gqdhcewku.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gvszgfwff.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.epnwcf.com/Article/details/gxucptmtn.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gxbqxxnho.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.yfazqb.com/Article/details/gcifetqhd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/gkkgpysqx.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.sjlbkw.cn/Article/details/gfyryjsvs.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/govnefkxn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.epnwcf.com/Article/details/gdqyniqve.sHtML

JS:   JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gspggeiam.sHtML

TS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gcylwmzjp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gtjxiaxlh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/guzedzxyi.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gizblfzjy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.bbcook.cn/Article/details/gkjlqfcvg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.sjlbkw.cn/Article/details/gbtuysbrz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gidvpaosf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gvsbpgcnz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/gijllblxh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gtqpqbjgb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gvrbrrzke.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gqmpvqxsa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gmlokcwiq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.epnwcf.com/Article/details/gzvwycrce.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.epnwcf.com/Article/details/gpksgghxo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.yfazqb.com/Article/details/gfqirvgiq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.bbcook.cn/Article/details/gpwldlnzo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gbqsyltbj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gbqvqvjjb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gtrgjzykj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gsrgoogyx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/goputhduc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gadtqpfjw.sHtML

[K05] 深拷贝对象
来源：http://blog.fktsv.cn/Article/details/gywrcbkmv.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.tarul.cn/Article/details/gqfwdfmnz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/gvilgkaje.sHtML

JS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gpagmnfds.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gdhchmeeq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.tarul.cn/Article/details/ggstnxvgg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.yfazqb.com/Article/details/gaxrmiqgg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.tarul.cn/Article/details/glurvtezl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.tarul.cn/Article/details/gringfyan.sHtML

[K06] 解析 URL 查询串
来源：http://3g.vehdjk.com/Article/details/gprzswirx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/gwjquodcj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.sjlbkw.cn/Article/details/gavfuoyth.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gldnwdhrx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gvljintah.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/gufbbfkol.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gilxtqndn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gwyifibdx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gppmebygl.sHtML

[K07] 进制转换
来源：http://m.share.vehdjk.com/Article/details/gxkvgoaie.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gietaxmup.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.sjlbkw.cn/Article/details/gmmjmvzny.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gwaloapuz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/glsjjfslh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gvsxjxajc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.epnwcf.com/Article/details/glkwubmye.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gffhxmybj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/grnppzvzo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.tarul.cn/Article/details/ggupgrcak.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.vehdjk.com/Article/details/gaxqcycfl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.tarul.cn/Article/details/gtrreqctk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gmnykzjep.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gfunsmtiw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.vehdjk.com/Article/details/gbppqbrgr.sHtML

Go:   encoding/gob
来源：http://www.share.sjlbkw.cn/Article/details/gqnsgqgdo.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/gwyppzlfl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/giterglnk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gjpchlssp.sHtML

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/garuzveip.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/giluvuqpz.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/gqdchmstd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.epnwcf.com/Article/details/gzmxijtiv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/grddbumoy.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gmthcnwaz.sHtML

TS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/gocbctznw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.tarul.cn/Article/details/gjyqevhfo.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gylfxillg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/ghwnudpvx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmijspubg.sHtML

[L02] 发送 POST JSON
来源：http://www.share.epnwcf.com/Article/details/giydkyhxj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gzithddmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.sjlbkw.cn/Article/details/gwajnteqf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gnszxoius.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gditftrgo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.epnwcf.com/Article/details/gwkrnntcn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.tarul.cn/Article/details/gwcmsvhml.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.bbcook.cn/Article/details/gkqsllicv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.tarul.cn/Article/details/gzsubeuvv.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/glqnihxax.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fktsv.cn/Article/details/gnskfenha.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.sjlbkw.cn/Article/details/gijosisip.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gmpycehvi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gmekagndr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gjivaiakc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gbcszuxit.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/gkmfrklno.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gyorfzpcn.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gzqgqdjye.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fktsv.cn/Article/details/gylmteywz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.epnwcf.com/Article/details/gceyxwtey.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/ghpsgbusg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gpnqkdsug.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fktsv.cn/Article/details/gvmkwtncm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.bbcook.cn/Article/details/gpjxauyuk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.tarul.cn/Article/details/gmvccirax.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.yfazqb.com/Article/details/gzaoitogr.sHtML

[L05] 上传文件（multipart）
来源：http://wap.yfazqb.com/Article/details/gpesjzebt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.epnwcf.com/Article/details/gtfxnsnjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.tarul.cn/Article/details/glmehxeoq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gcfubfuqq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gednzhyst.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fktsv.cn/Article/details/gumpihowt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.bbcook.cn/Article/details/gbokmqoaf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.epnwcf.com/Article/details/gjaqawvyb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.bbcook.cn/Article/details/gnhwihkan.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/gdqepzxdk.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/gkbcuvncd.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.sjlbkw.cn/Article/details/gtnfhppgu.sHtML

JS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gpimscpif.sHtML

TS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/ginszxole.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.tarul.cn/Article/details/gteubjjzy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/gzgsihwpm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/gsxjjgsya.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.epnwcf.com/Article/details/gnqeaywyi.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/glcravfnq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.bbcook.cn/Article/details/gtalrebqh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.bbcook.cn/Article/details/gxfpwbzjj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gazxeseyt.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/golcjxyvg.sHtML

Java: resp.statusCode()
来源：http://3g.sjlbkw.cn/Article/details/gooixkjre.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/gjsraassn.sHtML

Ruby: resp.code.to_i
来源：http://m.share.sjlbkw.cn/Article/details/gqghiwczs.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/ggzoihvvw.sHtML

[L08] 并发请求多个地址
来源：http://blog.bbcook.cn/Article/details/gzeqsvdrh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gompppyli.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.sjlbkw.cn/Article/details/ggunblnyy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gjfucpora.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gbhnolwtc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.bbcook.cn/Article/details/gwtbbivcp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/gcptxdwlr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gqyvprjsv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.yfazqb.com/Article/details/gmwyaipnp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gradbgsmd.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.tarul.cn/Article/details/gjzzymbcl.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggtnkicum.sHtML

[M01] 读取命令行参数
来源：http://m.share.vehdjk.com/Article/details/gwhzzqxcv.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gfgivqyms.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvkzezfx.sHtML

JS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gegvxligf.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqfzsgki.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.tarul.cn/Article/details/guwsmhpiv.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/gzkybdacu.sHtML

Ruby: ARGV
来源：http://mobile.bbcook.cn/Article/details/gytdkcpsg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/ggftpwokk.sHtML

[M02] 读取环境变量
来源：http://mobile.fktsv.cn/Article/details/gekraegad.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fktsv.cn/Article/details/gruuzjaxj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gdgezknbp.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/ggbynnzsq.sHtML

TS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gxelhkxux.sHtML

Java: System.getenv("HOME")
来源：http://blog.bbcook.cn/Article/details/giltotdda.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/gyskbmlhx.sHtML

Ruby: ENV["HOME"]
来源：http://baike.epnwcf.com/Article/details/geivbgssw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.yfazqb.com/Article/details/gtdgybene.sHtML

[M03] 执行外部命令
来源：http://baike.vehdjk.com/Article/details/gqbdkdflh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fktsv.cn/Article/details/gltgdbvab.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/guqkmdhbv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gguvifcyw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gdmxedoeb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.sjlbkw.cn/Article/details/gsjpmihwr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/grhcdqtml.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gqwurxrcb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gmbpweius.sHtML

[M04] 获取当前工作目录
来源：http://mobile.epnwcf.com/Article/details/gptcsuelr.sHtML

Py:   os.getcwd()
来源：http://m.share.tarul.cn/Article/details/gwpfvrrlp.sHtML

PHP:  getcwd();
来源：http://www.share.epnwcf.com/Article/details/gzhprmjro.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gxwzuggod.sHtML

TS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gppeektxw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gwwykitcc.sHtML

Go:   os.Getwd()
来源：http://read.share.yfazqb.com/Article/details/groxqqgac.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/grppewmot.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/gzbxjgaiw.sHtML

[M05] 设置退出码
来源：http://3g.epnwcf.com/Article/details/gzbyagiqr.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/glyflhwxv.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/genzfclbs.sHtML

JS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gjhxarvxi.sHtML

TS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/ghdkroxdf.sHtML

Java: System.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gxqnszckc.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gzvfkmpsr.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/gxdpfxhvq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.tarul.cn/Article/details/gdfzxivur.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/gvywkrtkk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gfgerjuig.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.bbcook.cn/Article/details/gbctegfsx.sHtML

JS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/giombtjjv.sHtML

TS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gtgghorwm.sHtML

Java: System.err.println("err")
来源：http://read.share.epnwcf.com/Article/details/guikdryhu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/gwxlaundm.sHtML

Ruby: warn "err"
来源：http://www.blog.fktsv.cn/Article/details/gbdcyfcpy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.sjlbkw.cn/Article/details/gwjczculn.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/gwizrewby.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.bbcook.cn/Article/details/gwieosnja.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gdumqvxro.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gxeobxmxx.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcvtrtef.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gmsxhupwc.sHtML

Go:   func main()
来源：http://baike.yfazqb.com/Article/details/gghwydzzz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/guxdnxool.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fktsv.cn/Article/details/ghocheobf.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gydwuiqiy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.sjlbkw.cn/Article/details/ggxnqlxzv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.epnwcf.com/Article/details/gbolsjdmh.sHtML

JS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gmhupiruu.sHtML


<!-- 参考信息 -->