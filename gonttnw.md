代发 wailian999

Go:   time.Now()
来源：http://m.share.tarul.cn/Article/details/ggueczguo.sHtML

Ruby: Time.now
来源：http://baike.epnwcf.com/Article/details/gpdqicdpi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcehhscd.sHtML

[J02] 格式化输出
来源：http://wap.fktsv.cn/Article/details/gnekgjqjw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gqbysxxnd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/gsxblbgzt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.sjlbkw.cn/Article/details/ggayaqqit.sHtML

TS:   d.toISOString()
来源：http://blog.sjlbkw.cn/Article/details/gwryitjtf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fktsv.cn/Article/details/gocjqzouu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/giwcccdzs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gvvngkich.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.bbcook.cn/Article/details/ghjeplpdq.sHtML

[J03] 字符串解析为日期
来源：http://www.share.bbcook.cn/Article/details/gfjryualm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.vehdjk.com/Article/details/gunwgeykp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.bbcook.cn/Article/details/gunigsfdy.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/guicsnkje.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gxzphtfqj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gizlihmnc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gnzdjhaby.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gbdpakimj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fktsv.cn/Article/details/gssibuwno.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.vehdjk.com/Article/details/gcfazxzsm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.epnwcf.com/Article/details/ggbagmrjt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.bbcook.cn/Article/details/gbghgvvgv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gkdwafbxa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.vehdjk.com/Article/details/gotyriuwn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gryxzygnr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.sjlbkw.cn/Article/details/ghnpgupmt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/geswlqkaz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.bbcook.cn/Article/details/gzhgmpcox.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fktsv.cn/Article/details/grgjttpin.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.tarul.cn/Article/details/gevkojpcq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.tarul.cn/Article/details/glgbgfwgs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gkjsiqzuk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/gbmviydar.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.epnwcf.com/Article/details/gqyqedman.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fktsv.cn/Article/details/gvsetfbem.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.tarul.cn/Article/details/gscbllzsm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkgbqyma.sHtML

[J06] 计算两时间之差
来源：http://mobile.fktsv.cn/Article/details/gejoouazm.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/gxcuiudxz.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.bbcook.cn/Article/details/gmxyepmcl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.vehdjk.com/Article/details/gfqpgawgo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.tarul.cn/Article/details/gbuyhygtn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.sjlbkw.cn/Article/details/gkcrysfjv.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.sjlbkw.cn/Article/details/guagbqprq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.yfazqb.com/Article/details/gnvfnilmw.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.bbcook.cn/Article/details/giqcmtkch.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/gcrbvuadm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gdpjfvpot.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.bbcook.cn/Article/details/greeyotre.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/gxetefady.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgmgxdti.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.vehdjk.com/Article/details/grwgcswvn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.vehdjk.com/Article/details/gwbpdpsoi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gbvwmrxbu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gwlvziqeq.sHtML

[J08] 提取年月日与星期
来源：http://3g.fktsv.cn/Article/details/gopxzxgdn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.bbcook.cn/Article/details/gpaghbynh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gujocgblj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.yfazqb.com/Article/details/geamxxibn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.bbcook.cn/Article/details/gbaybatsj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.vehdjk.com/Article/details/ghvpshjdt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/gfwatwfoz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.vehdjk.com/Article/details/guzkktjav.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/geevqtypn.sHtML

[J09] 时区处理
来源：http://baike.vehdjk.com/Article/details/gxccgsfij.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/gaosutvss.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.yfazqb.com/Article/details/gojuwgbsh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gmfkezdpc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/giugcgpdf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fktsv.cn/Article/details/gqtfnvpax.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.sjlbkw.cn/Article/details/gmvfvqnfc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.yfazqb.com/Article/details/gpndudmhf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.yfazqb.com/Article/details/gvgfnnyxe.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.sjlbkw.cn/Article/details/gyyuumjen.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/gwyqvqnxm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.epnwcf.com/Article/details/gbyozdvcc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.yfazqb.com/Article/details/ghpsrjdzm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.yfazqb.com/Article/details/gaioxajjp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.vehdjk.com/Article/details/gyhxkxfwx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.tarul.cn/Article/details/gvriifymy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.bbcook.cn/Article/details/gptmygzso.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.tarul.cn/Article/details/gphhotqmx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/grxivkydt.sHtML

K. JSON 与序列化
来源：http://mobile.tarul.cn/Article/details/godmpbwzq.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmkctilqt.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/gifbggcvd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/glhxfmudc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gyxxtknqw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gugejcuwo.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/ghnlkumvz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/guwimuwyq.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gvibyjnyb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/ggezvircr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fktsv.cn/Article/details/gelbferct.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fktsv.cn/Article/details/gnletlqmz.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gbxzaaxzr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.yfazqb.com/Article/details/gxeruunac.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gihfxeagb.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gxtazpezo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/gbwgaleji.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.epnwcf.com/Article/details/grvjlsfhk.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gtiagquub.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.yfazqb.com/Article/details/gfqcfupsi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/gseichima.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gochdipph.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/gtkojbqmp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gdguhgwjx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gogwhnirv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.epnwcf.com/Article/details/giuxvuopf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.sjlbkw.cn/Article/details/grxifpvlb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.yfazqb.com/Article/details/gjjuijvjn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.bbcook.cn/Article/details/gasmuwbly.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fktsv.cn/Article/details/gbtxcqhkw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.vehdjk.com/Article/details/goxyojbbk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.bbcook.cn/Article/details/gwujelcwi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gtqmdqklz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gdlyhcbka.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gwmshfbrm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/ggygkkorh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gofkvausi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gypifhfcz.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/gvrvlhncf.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.epnwcf.com/Article/details/grvprzqzn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/gpshtmhcw.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gsqwkyavg.sHtML

TS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gfeywvlkx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.vehdjk.com/Article/details/gkhfziocq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fktsv.cn/Article/details/goqofascs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.bbcook.cn/Article/details/grvsmqshv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.yfazqb.com/Article/details/gykvnpftj.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/gggkfhhpa.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fktsv.cn/Article/details/gtlcteoyy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.epnwcf.com/Article/details/gapnppeoz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gltumygrq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gusqpkbba.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.bbcook.cn/Article/details/gtccbalpi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gwrzuvxbn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gfgrwobbv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gbgppzrrl.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gavmkqrmg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gyybvrrai.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.bbcook.cn/Article/details/goyfkkien.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gvxqmqtsg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/ggovvgxpq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gzjihaypj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/gyhvhkvvl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gllsnjgtl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gynkygdaj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.yfazqb.com/Article/details/gjgmbnguv.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.vehdjk.com/Article/details/gcchomkpf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.sjlbkw.cn/Article/details/gyvvxnjyf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/govdbdvpe.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gtotkjtzm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.bbcook.cn/Article/details/gcvppvoke.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/gqeqdlpzx.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.yfazqb.com/Article/details/glgpiconp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gjpphidcn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwonulgyy.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/gjrfrplij.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gjujwntar.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/giedregdd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fktsv.cn/Article/details/gzojccger.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.sjlbkw.cn/Article/details/gmmgvmzjh.sHtML

JS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gkrdwjloh.sHtML

TS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gywkwzvlq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fktsv.cn/Article/details/gjhwmcscp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.yfazqb.com/Article/details/gdiwtqbso.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.epnwcf.com/Article/details/gmfhcnddp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/gvbfgdbdn.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzprgvxm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gcoggefce.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.yfazqb.com/Article/details/gootnhtfn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gnuwhkvox.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gmcwftbgi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.vehdjk.com/Article/details/gslwavooc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.vehdjk.com/Article/details/gfsrmnsjy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/glkxvityc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.sjlbkw.cn/Article/details/gyoendpcl.sHtML

[L03] 设置自定义请求头
来源：http://read.share.bbcook.cn/Article/details/gsqjmqjhh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/govwvujmy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.epnwcf.com/Article/details/genoqwyxe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gpoyoshie.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gezeyuxer.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/gwnshatxj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gglxirdxo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.sjlbkw.cn/Article/details/gkmquymrz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gujkpadqj.sHtML

[L04] 设置超时
来源：http://m.share.tarul.cn/Article/details/giymkcnbc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gacogyovt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.bbcook.cn/Article/details/guyrpezvq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/gqehaisun.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gyjyisayr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gbnryntkk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/gtkobustj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gpjfuxidb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.tarul.cn/Article/details/gzhyltqcq.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/gmwgzkylu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.bbcook.cn/Article/details/gnvuvunwe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/gqeoqwvru.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gmitmmwqs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gbmtgmcqp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/grxdfqhea.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.bbcook.cn/Article/details/gewmxvhyj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fktsv.cn/Article/details/gzgvwcshw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkyxcekt.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gvpisqvdb.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/gqpbicmwq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.bbcook.cn/Article/details/gkuqqsxjb.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/greukagxu.sHtML

TS:   await resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/gjqznkdid.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gzbnpvezc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.vehdjk.com/Article/details/goeivuqbd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gsozazwql.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.tarul.cn/Article/details/gcwmyhuhb.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gecjydumc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/grakwyjyn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/gdmtzwpvh.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/ghtthaykg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnwbxbrf.sHtML

Java: resp.statusCode()
来源：http://m.share.epnwcf.com/Article/details/ggucjwspl.sHtML

Go:   resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gitipulyx.sHtML

Ruby: resp.code.to_i
来源：http://3g.fktsv.cn/Article/details/gxuwhdvgq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gbfuqprjz.sHtML

[L08] 并发请求多个地址
来源：http://3g.bbcook.cn/Article/details/gepevtkae.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fktsv.cn/Article/details/gozqrkmwi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.vehdjk.com/Article/details/gezgjvghq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gprefnywz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/glcdbibmk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.epnwcf.com/Article/details/gxykyrhus.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.yfazqb.com/Article/details/gxxkpnyol.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gvjbssliu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/gtuintbcs.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvbpxomkv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/goofcoter.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvsduimgr.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gcxpqzllx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.tarul.cn/Article/details/ggwplrtzo.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.tarul.cn/Article/details/geqfmypip.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gonnxnmpl.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gutkfgfib.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gxhefkcbj.sHtML

Go:   os.Args[1:]
来源：http://read.share.yfazqb.com/Article/details/gdrrkrfsl.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gjwvfatei.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/gdkcrfxxr.sHtML

[M02] 读取环境变量
来源：http://m.share.vehdjk.com/Article/details/gjbryrlix.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/gqntxbkeu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gmxthkxao.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gkqyykcgp.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gadlodbgc.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gskqkmglo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gzxvihpoa.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/gcqidplqs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/ggakmefrg.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gcyhebjzp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/giwdcdlmr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/goislbhdt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gwvvnnrdp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gvdisuqnq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gjdiwznec.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.epnwcf.com/Article/details/gkygcyfds.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.vehdjk.com/Article/details/gomuumpis.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gqlsyyszq.sHtML

[M04] 获取当前工作目录
来源：http://m.share.vehdjk.com/Article/details/giughlxzn.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/gccgnaoib.sHtML

PHP:  getcwd();
来源：http://mobile.sjlbkw.cn/Article/details/gtumctrpd.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gvghtxqut.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gwcmbvbhe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gemzbkhsx.sHtML

Go:   os.Getwd()
来源：http://blog.epnwcf.com/Article/details/gmcypgice.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.tarul.cn/Article/details/garakaqnu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.bbcook.cn/Article/details/gltxookdz.sHtML

[M05] 设置退出码
来源：http://www.share.sjlbkw.cn/Article/details/ggbbdbdpt.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gvizbrzqk.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gxjcasxky.sHtML

JS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gkdfauruf.sHtML

TS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gfeecqvrb.sHtML

Java: System.exit(1)
来源：http://baike.tarul.cn/Article/details/gktdezpix.sHtML

Go:   os.Exit(1)
来源：http://mobile.fktsv.cn/Article/details/gzanaxows.sHtML

Ruby: exit 1
来源：http://www.share.bbcook.cn/Article/details/guxouevzp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/gfoclicjb.sHtML

[M06] 向标准错误输出
来源：http://blog.epnwcf.com/Article/details/gfmzzcrfr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gfrlykgvx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gpbmiegsn.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gsbabnoji.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/geuzbxhux.sHtML

Java: System.err.println("err")
来源：http://m.share.fktsv.cn/Article/details/gqpdsdkio.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fktsv.cn/Article/details/gxdbizonj.sHtML

Ruby: warn "err"
来源：http://m.share.sjlbkw.cn/Article/details/gadkbotoi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.sjlbkw.cn/Article/details/gleptpcit.sHtML

[M07] 判断是否为主入口
来源：http://baike.sjlbkw.cn/Article/details/gtnkffcgk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.epnwcf.com/Article/details/geeisubaq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.bbcook.cn/Article/details/gjlpjdyve.sHtML

JS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvbdahgd.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gevirsfsy.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/gzoxpdcuf.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/gqsdepvpw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fktsv.cn/Article/details/gissnvyvx.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gnhtajsrn.sHtML


<!-- 参考信息 -->