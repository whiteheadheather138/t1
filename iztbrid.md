代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/gkpspuzsu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/grqgyzeus.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.vehdjk.com/Article/details/gafymumjq.sHtML

TS:   d.toISOString()
来源：http://3g.bbcook.cn/Article/details/geikaryyk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.tarul.cn/Article/details/grutmmogq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gwwmgmcni.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gtuqxgfpo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.epnwcf.com/Article/details/gfpnivlhn.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/gtuvfbpah.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.yfazqb.com/Article/details/gorjttjnb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.epnwcf.com/Article/details/gfvurnvfv.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gsvykemzt.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gexovgmjo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/guzmxckzj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gnuatdrtf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gyzyljfqf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.yfazqb.com/Article/details/gsugjgaam.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/ggntczygz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fktsv.cn/Article/details/gvonorsmj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.tarul.cn/Article/details/grwddylrt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gxrwtrgfa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fktsv.cn/Article/details/gautfcnty.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.tarul.cn/Article/details/gzwygbwwb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.bbcook.cn/Article/details/gvrgnlkiw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gepgcelme.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.epnwcf.com/Article/details/gmsoeylse.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.sjlbkw.cn/Article/details/grxvhmwlm.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.bbcook.cn/Article/details/gvafnwdgc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.yfazqb.com/Article/details/gbkofkmxb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/glxdptllq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.yfazqb.com/Article/details/gnlymgnlc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/gbtezidkp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fktsv.cn/Article/details/gvptqyklp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpccthca.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.tarul.cn/Article/details/grbjjnlyx.sHtML

[J06] 计算两时间之差
来源：http://www.blog.epnwcf.com/Article/details/gydojkinj.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/gvhehuuax.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.vehdjk.com/Article/details/gyvdkhoua.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.tarul.cn/Article/details/gkjdgcqyx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/ganvoxhis.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.yfazqb.com/Article/details/gwitffela.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.epnwcf.com/Article/details/gslvsjrfh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.vehdjk.com/Article/details/gnieaysrf.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fktsv.cn/Article/details/gtnmxgkcz.sHtML

[J07] 比较两个日期
来源：http://read.share.bbcook.cn/Article/details/gkplavpht.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gdfhgjilp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.vehdjk.com/Article/details/glmfxmrxv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gpoehulzd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gwyzbxuwy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.epnwcf.com/Article/details/gejuvzxhz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fktsv.cn/Article/details/gcdokhmtg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gtuupxong.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gjrxhglih.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gnplaniym.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.epnwcf.com/Article/details/glmpnceny.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.yfazqb.com/Article/details/gmmgthloe.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fktsv.cn/Article/details/gttedjnza.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.yfazqb.com/Article/details/gpvzqacmj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fktsv.cn/Article/details/gylaejfhc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.tarul.cn/Article/details/gvrbqnsqx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.epnwcf.com/Article/details/goyfzydyq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.vehdjk.com/Article/details/gcuytiddc.sHtML

[J09] 时区处理
来源：http://www.m.share.vehdjk.com/Article/details/gtmtvlsrw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/gnrucvsue.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/gdqbsvjte.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/gshpirvpl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gqjlkuadz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gahbpzbcf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.bbcook.cn/Article/details/gzwqzjush.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.bbcook.cn/Article/details/gomnjpskj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.vehdjk.com/Article/details/gdoepqhqy.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.sjlbkw.cn/Article/details/gdmxpqthj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.tarul.cn/Article/details/gqpyotujo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gemmdvamz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fktsv.cn/Article/details/grinpwqyo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.bbcook.cn/Article/details/glvgshagl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/gbkcgnrjc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gbxnmbxjp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.epnwcf.com/Article/details/gsixqpltn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.yfazqb.com/Article/details/ghmxsolah.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnnxwriwl.sHtML

K. JSON 与序列化
来源：http://read.share.sjlbkw.cn/Article/details/gztupblio.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnrwetmnc.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.yfazqb.com/Article/details/gluepvslb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/ghsaembis.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqnekxbi.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gpassemoq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gvvyoywqi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.sjlbkw.cn/Article/details/gifhlufua.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/gsdttydfz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzdnprza.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/gymsddlnw.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.bbcook.cn/Article/details/gyotzimlb.sHtML

Py:   json.loads(s)
来源：http://read.share.vehdjk.com/Article/details/ghprjjnme.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gquprwhdi.sHtML

JS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gyyxkstzu.sHtML

TS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gddqlorhp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.bbcook.cn/Article/details/gdcfwmquo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/geooitpdx.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gmxbdocin.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/gzfpsydda.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fktsv.cn/Article/details/ggyvtszrr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gqnssysqi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gdtwzsngs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.epnwcf.com/Article/details/glqwndjph.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gawldyrgg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/grutaxjwq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.tarul.cn/Article/details/gyiwepeyj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.yfazqb.com/Article/details/gjamqitxk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.tarul.cn/Article/details/gmgfwsymt.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.tarul.cn/Article/details/gkizhrktq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/gbzqkzesy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.yfazqb.com/Article/details/grqkidtkf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/genhewrpk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/gcagaqsqf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gyvdkrype.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gyakqddra.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fktsv.cn/Article/details/gqroxfvor.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.yfazqb.com/Article/details/gixqqouvk.sHtML

[K05] 深拷贝对象
来源：http://blog.fktsv.cn/Article/details/gkobkzzwz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/giaqlanoz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/ghekdboes.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/ggyfxnerf.sHtML

TS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gytwhxvaq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.vehdjk.com/Article/details/gnbrjovzt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.epnwcf.com/Article/details/goulblnbj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.vehdjk.com/Article/details/gbychipgj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/glqmuwtoi.sHtML

[K06] 解析 URL 查询串
来源：http://3g.tarul.cn/Article/details/gznbgwuzu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gbknygzui.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/gabthmosp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gnlxcgysn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gnlvrthfg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/guazdcmof.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gozccgndx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gqszokwxa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/ggmffjyxf.sHtML

[K07] 进制转换
来源：http://mobile.yfazqb.com/Article/details/gocibulji.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gbogpbcrb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.tarul.cn/Article/details/gjreoqckh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gaukmlfje.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gitmpfnps.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gwnrmnlwl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.bbcook.cn/Article/details/gefkqhtal.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fktsv.cn/Article/details/gmibnmmrp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/genkpojtn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.bbcook.cn/Article/details/goqsapiko.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gubpimlic.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.vehdjk.com/Article/details/gakuipcdd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gonwsszoa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gchbyhzcc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.sjlbkw.cn/Article/details/glxjrihrc.sHtML

Go:   encoding/gob
来源：http://blog.tarul.cn/Article/details/gszsuprcc.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.tarul.cn/Article/details/gloexbmyz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gqapaaoez.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsbqykbra.sHtML

L. 网络请求
来源：http://wap.tarul.cn/Article/details/gmqdqauxo.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gbnzsevsd.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.epnwcf.com/Article/details/gppvykmju.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/gvtoamvbm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.vehdjk.com/Article/details/gsytsxojk.sHtML

JS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gmmzvwkmz.sHtML

TS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gcvxazkhw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.sjlbkw.cn/Article/details/gjnqdzhwp.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/gfghofjsu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.sjlbkw.cn/Article/details/gtklksigi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/gfujvsoon.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gejjowgkr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.bbcook.cn/Article/details/gxvfkyfdm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fktsv.cn/Article/details/guzuweybs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gddwvqqsg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gswkvkjpq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.tarul.cn/Article/details/givnlgaad.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.bbcook.cn/Article/details/gvibzsxtc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.epnwcf.com/Article/details/gubegplmh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.yfazqb.com/Article/details/gkredwiyh.sHtML

[L03] 设置自定义请求头
来源：http://mobile.vehdjk.com/Article/details/gjahzqxxa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.yfazqb.com/Article/details/gojixrdti.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/geyqyjrci.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/gcfjemzeh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gxbkawdts.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/ghmshuxjv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gjqntjjby.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.sjlbkw.cn/Article/details/ggtewvjlq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gnwozhzdu.sHtML

[L04] 设置超时
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzaxahco.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fktsv.cn/Article/details/gtkaqynzq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.tarul.cn/Article/details/gdzopbcdn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/glokpjbiq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gpdfaktpd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/gqtgaryww.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.tarul.cn/Article/details/gdqoyvkbb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.epnwcf.com/Article/details/gpjuqtihp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.sjlbkw.cn/Article/details/gotmbmmzy.sHtML

[L05] 上传文件（multipart）
来源：http://3g.sjlbkw.cn/Article/details/gvpykfzir.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.bbcook.cn/Article/details/gtportzlx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/gcqsmbify.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gqvedoedm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gtpptkpmx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fktsv.cn/Article/details/gvzbrehmh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.tarul.cn/Article/details/giqugrmih.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.tarul.cn/Article/details/ghgrprpwa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gbwvcqzls.sHtML

[L06] 解析响应为 JSON
来源：http://baike.epnwcf.com/Article/details/guqgqemuj.sHtML

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/gmungfple.sHtML

PHP:  json_decode($body, true);
来源：http://3g.tarul.cn/Article/details/gpnrgkeiv.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gyarczrmq.sHtML

TS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gyoawzobq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.vehdjk.com/Article/details/gjieaygcd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/gclfxuylj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gtcuknkhx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.tarul.cn/Article/details/ggdtvqrkl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gkjftncco.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.sjlbkw.cn/Article/details/gmlmjaadk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gquhvhtbv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gaohwscus.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gjxvequad.sHtML

Java: resp.statusCode()
来源：http://wap.sjlbkw.cn/Article/details/gkoqehjyd.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gsmwvzfmt.sHtML

Ruby: resp.code.to_i
来源：http://baike.bbcook.cn/Article/details/gxyevzjcg.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/gkxxvtfpp.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/gnjexlukv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gkvrbomyw.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/gvdcdzlbs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/grfcqkesy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gmwekpmnq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gnclaqafx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.yfazqb.com/Article/details/gbksvedva.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/gcjqkmbus.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gateaagth.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmcmkgepo.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.sjlbkw.cn/Article/details/gegcqmjzu.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gprjfhiid.sHtML

[M01] 读取命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/gdbuefaqk.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/gscevptaa.sHtML

PHP:  $argv;  $argc;
来源：http://wap.tarul.cn/Article/details/gqbrrqtms.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gqnqwdmoi.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gobppehwv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/grykzfgip.sHtML

Go:   os.Args[1:]
来源：http://baike.fktsv.cn/Article/details/geddqdtxa.sHtML

Ruby: ARGV
来源：http://3g.epnwcf.com/Article/details/gilupkwyp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gqcsgtyss.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gweuftivp.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.sjlbkw.cn/Article/details/ghxyabkes.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gdpclkfpt.sHtML

JS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gyygvwppa.sHtML

TS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/gdtgcyldb.sHtML

Java: System.getenv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gehnwsugf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gkcmskyhk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/gbxnelnue.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gviosxlzf.sHtML

[M03] 执行外部命令
来源：http://www.blog.tarul.cn/Article/details/gsmhzbyjy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/geqjchqrk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/gquvspfea.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gzbfadukv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gugmekzwj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.epnwcf.com/Article/details/gurfhcsix.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gyqsmodpn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/geqaduzvl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.epnwcf.com/Article/details/gkjwxczfs.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fktsv.cn/Article/details/gmfhujbak.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/gxjecqfos.sHtML

PHP:  getcwd();
来源：http://www.blog.bbcook.cn/Article/details/gpytbydbe.sHtML

JS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gbzfemhat.sHtML

TS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/geloxsyog.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/geopkrspi.sHtML

Go:   os.Getwd()
来源：http://baike.sjlbkw.cn/Article/details/gaylwqpcs.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/gjejvkvpc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.bbcook.cn/Article/details/glqigblvi.sHtML

[M05] 设置退出码
来源：http://www.blog.bbcook.cn/Article/details/gggzpnyht.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/guhyrfebb.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/ghlyqacog.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gvomstjdq.sHtML

TS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gtuorqwnd.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gftdevkxj.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/golyawyzj.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/gwxwxuctr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gajaeudaw.sHtML

[M06] 向标准错误输出
来源：http://www.share.epnwcf.com/Article/details/gspufufal.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gkzlaycwl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.tarul.cn/Article/details/gvdauhpeo.sHtML

JS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gklshekce.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gmhpyqacz.sHtML

Java: System.err.println("err")
来源：http://blog.sjlbkw.cn/Article/details/gksispagb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/gchujrlik.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/glfcgrlpc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.tarul.cn/Article/details/glzmabbcg.sHtML

[M07] 判断是否为主入口
来源：http://baike.epnwcf.com/Article/details/gujpbxvoo.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.yfazqb.com/Article/details/gufbxvnyo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gbrokuiyz.sHtML

JS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gefnqoatn.sHtML

TS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gnkexnpkb.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/gnyvrnurh.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/ggskqsykn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/gvwznwqct.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/gjvcfpcqc.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.vehdjk.com/Article/details/ggzgpwigd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gaihoimuu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gqabmnfsz.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gygopujfs.sHtML


<!-- 参考信息 -->