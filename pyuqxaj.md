代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gvdyexxcc.sHtML

JS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/ganyhtilb.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gpanjsbep.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.epnwcf.com/Article/details/gqmpdxtzd.sHtML

Go:   time.Now()
来源：http://blog.tarul.cn/Article/details/grljrbjvq.sHtML

Ruby: Time.now
来源：http://www.m.share.fktsv.cn/Article/details/gtwviegcl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.vehdjk.com/Article/details/gzqfozbfv.sHtML

[J02] 格式化输出
来源：http://blog.tarul.cn/Article/details/gjarpdsro.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gfkkueqlh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gscynpfox.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fktsv.cn/Article/details/gmbqleivi.sHtML

TS:   d.toISOString()
来源：http://m.share.sjlbkw.cn/Article/details/gfyvffuzs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fktsv.cn/Article/details/grcqgmstk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.tarul.cn/Article/details/glvaxwzdu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gvahhbfyr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fktsv.cn/Article/details/gqutqdweu.sHtML

[J03] 字符串解析为日期
来源：http://3g.yfazqb.com/Article/details/gbckkyljz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fktsv.cn/Article/details/grcqskhyu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.yfazqb.com/Article/details/gzcwewhap.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/giokxieqh.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gcdefbfew.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gqansctqy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gbtbnctxw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gzhvbelra.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.epnwcf.com/Article/details/gcyqenocb.sHtML

[J04] 时间戳与日期互转
来源：http://baike.vehdjk.com/Article/details/gbyrdfzkn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.yfazqb.com/Article/details/gjprksyod.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/gkjlomksg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.tarul.cn/Article/details/gqvlvmtkd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcexkpuhs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/ghcxruylp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fktsv.cn/Article/details/gjlvfgitj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.sjlbkw.cn/Article/details/gwfyfdlxj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.sjlbkw.cn/Article/details/goddsztpu.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.sjlbkw.cn/Article/details/gwsvzurlt.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fktsv.cn/Article/details/gnxeoedla.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.yfazqb.com/Article/details/gmmefcxiu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gwjgzryje.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/ghhevstll.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.sjlbkw.cn/Article/details/ggbxnynvs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fktsv.cn/Article/details/gibgmypjb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.tarul.cn/Article/details/grtcvvpff.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/ggjoxqcgy.sHtML

[J06] 计算两时间之差
来源：http://m.share.vehdjk.com/Article/details/grmxvqvcp.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.yfazqb.com/Article/details/grlcswdab.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.bbcook.cn/Article/details/gldbapdpa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/gjurweqqp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fktsv.cn/Article/details/gvjfuxbmd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.vehdjk.com/Article/details/gfcgstzke.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gvroepvwl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.sjlbkw.cn/Article/details/gngxedjnv.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fktsv.cn/Article/details/gccxbieqr.sHtML

[J07] 比较两个日期
来源：http://wap.epnwcf.com/Article/details/gwyrepctk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/grqiossyn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gkmtewatf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/goxxfdtpi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gcakgnjkw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.tarul.cn/Article/details/ghfqxumxq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.yfazqb.com/Article/details/gjphoruza.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gmtkdokrs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gtooxrqfn.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gpkfwqgxb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.vehdjk.com/Article/details/ggwcapwkp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/gxffglmgj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.bbcook.cn/Article/details/gqmgaeylt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/gozisylyx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.tarul.cn/Article/details/grwcgnshg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.sjlbkw.cn/Article/details/gfgrptsrq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.sjlbkw.cn/Article/details/gitkgotfi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.sjlbkw.cn/Article/details/gxdcrwpxk.sHtML

[J09] 时区处理
来源：http://blog.vehdjk.com/Article/details/gbybpnkre.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.yfazqb.com/Article/details/gwdpzmlld.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.tarul.cn/Article/details/guptbuzmp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gepsgwqet.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gkexjztro.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.yfazqb.com/Article/details/gfmiicnhv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.epnwcf.com/Article/details/glfwtthds.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.tarul.cn/Article/details/gvhwtxtcw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.tarul.cn/Article/details/gkrzinkjh.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fktsv.cn/Article/details/gdpswmtfs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.vehdjk.com/Article/details/geprkocrt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.vehdjk.com/Article/details/gmqcsfdkj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.vehdjk.com/Article/details/gviwnlmcu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gweurmwim.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.epnwcf.com/Article/details/gydhcndam.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/ggwyhossz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/ggsjlaxlt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.sjlbkw.cn/Article/details/gpbtzwicg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmkfhpegs.sHtML

K. JSON 与序列化
来源：http://3g.bbcook.cn/Article/details/gxqqutwki.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxlireljj.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.tarul.cn/Article/details/gzjzlfmfy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gszpjwsnu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/guvkebffl.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gycyrrztr.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gysbindjn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/gpxdaejbd.sHtML

Go:   json.Marshal(obj)
来源：http://baike.tarul.cn/Article/details/gsmgixibf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fktsv.cn/Article/details/gzzgdticw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.tarul.cn/Article/details/gxnjlyukp.sHtML

[K02] JSON 字符串转对象
来源：http://blog.epnwcf.com/Article/details/gggygcstf.sHtML

Py:   json.loads(s)
来源：http://baike.fktsv.cn/Article/details/gfkcaenmu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.sjlbkw.cn/Article/details/gekaswliq.sHtML

JS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gkelbogjc.sHtML

TS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gnhhahacc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcmvipac.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gdsffhwne.sHtML

Ruby: JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gwhocukuf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnwfsevd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.tarul.cn/Article/details/gvsllzofg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gosruegph.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/gplcigwiu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gwczdjqxc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/gybpydbyo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gnmwgmfcf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.sjlbkw.cn/Article/details/gzxsnzlnu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.vehdjk.com/Article/details/grcffywxr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.tarul.cn/Article/details/gtxblqpxk.sHtML

[K04] 读取 JSON 文件
来源：http://wap.yfazqb.com/Article/details/gqnksllaa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.epnwcf.com/Article/details/gwzgkitkq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.tarul.cn/Article/details/gosedmnfo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gjkccfpgv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/gcdojsvdd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gbcsmhxph.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gofnfssob.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gghmmnbuv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.tarul.cn/Article/details/ggmtqihkj.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.yfazqb.com/Article/details/gevbzfgdg.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/glzgebpmn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.sjlbkw.cn/Article/details/gnvtbxvye.sHtML

JS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/goithmbmg.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gebrigjum.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/gwtzzapht.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.tarul.cn/Article/details/gqeanxkpx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/guvgrxibz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.epnwcf.com/Article/details/ggsuupkck.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/ggwykcbsc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gktfcktem.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.sjlbkw.cn/Article/details/gqubjkhpi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gbfifeemt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/guzreastb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.bbcook.cn/Article/details/gxogfozoi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/glhgxetwy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gmkmlqpxx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gvcewtehu.sHtML

[K07] 进制转换
来源：http://www.blog.tarul.cn/Article/details/glmafiaqk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gjhyywemx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/gnacjidnm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gykhyotto.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gjykkhcbt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gtmzbkmfy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gdivyodyn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.epnwcf.com/Article/details/gjzlpbgke.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gglxrtexi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.tarul.cn/Article/details/gfhitedqn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gmhypfmmg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.yfazqb.com/Article/details/gtlueumuv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/gkqyoblhg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gupkkvbyc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.vehdjk.com/Article/details/glkrpjido.sHtML

Go:   encoding/gob
来源：http://mobile.fktsv.cn/Article/details/gtazqrrvv.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gqouutsiw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/galathlgz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbnvltdqa.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/gjoyxiltw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grrffjaih.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fktsv.cn/Article/details/gzfpjpsqn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/gqsqkhraq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fktsv.cn/Article/details/grrryacii.sHtML

JS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gjfkottlq.sHtML

TS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gvdvafgcr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/gcebybdfe.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/gatojhnrk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/gvvfzxzkk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/gmltumfia.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gpsrlithj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/gmefonzvp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gusjowruf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gqhllwnoh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gylrjjgia.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.tarul.cn/Article/details/gimktroju.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.vehdjk.com/Article/details/gvkblppig.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.sjlbkw.cn/Article/details/gtmkaeosi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.vehdjk.com/Article/details/gphvitutn.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpdxbxen.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.yfazqb.com/Article/details/gqdyglzlc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.tarul.cn/Article/details/gvtdmqkjd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gcniviwsu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gjddimxpf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.epnwcf.com/Article/details/gorzliaeb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gacxjopcn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.sjlbkw.cn/Article/details/gicbtqbdq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gosjubcad.sHtML

[L04] 设置超时
来源：http://read.share.sjlbkw.cn/Article/details/gllxoffhi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.yfazqb.com/Article/details/gpgqowekq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.sjlbkw.cn/Article/details/gtlebjbyc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gcaoguptt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gmspkheqg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gwjfninyz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/giplhaied.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.yfazqb.com/Article/details/gkuksyljs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/ganxydloc.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fktsv.cn/Article/details/gjmerahse.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/gdkhujfpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.tarul.cn/Article/details/gajuawnvh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gvjnscqyc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gfzclsyum.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.sjlbkw.cn/Article/details/gpkpqjako.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.bbcook.cn/Article/details/gosognktw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fktsv.cn/Article/details/guhphsryr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fktsv.cn/Article/details/gvkslwkvm.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gnrnbswft.sHtML

Py:   resp.json()
来源：http://mobile.vehdjk.com/Article/details/gtmgkfevk.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.epnwcf.com/Article/details/gsrpnyskb.sHtML

JS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gyijjbrfc.sHtML

TS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gtaxencbq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.epnwcf.com/Article/details/gctwgyliw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.bbcook.cn/Article/details/gxdfnoemv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gajmbfvap.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.vehdjk.com/Article/details/gyumjgtgq.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gbaxkrqnf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.bbcook.cn/Article/details/gojtjfbfg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/gtbhsbokm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gmquztusy.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gosocmbic.sHtML

Java: resp.statusCode()
来源：http://www.share.epnwcf.com/Article/details/grpffmqfo.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gnhhopwkf.sHtML

Ruby: resp.code.to_i
来源：http://mobile.bbcook.cn/Article/details/grpmimwjk.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gcpqfyvaj.sHtML

[L08] 并发请求多个地址
来源：http://www.share.vehdjk.com/Article/details/grktbtlxg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.tarul.cn/Article/details/gvfvlugas.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/goswyackx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/ghtrtsiqr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gkfzyivnx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.sjlbkw.cn/Article/details/gvbhkainl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.vehdjk.com/Article/details/grzesxiso.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/gtsmkbhld.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.bbcook.cn/Article/details/gpyropqac.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gmirkbood.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/gpoxosyvu.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdedawjbm.sHtML

[M01] 读取命令行参数
来源：http://wap.vehdjk.com/Article/details/gsanztkqv.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gmcpxusxw.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/gtcsoequh.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gegefzpvj.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/ggcxgocio.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/ghgmkljfc.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gesvlwlrc.sHtML

Ruby: ARGV
来源：http://baike.tarul.cn/Article/details/gmvjqrudd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/ghxnlkaxm.sHtML

[M02] 读取环境变量
来源：http://blog.vehdjk.com/Article/details/gsncwqpnl.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gsnrqtkax.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gowhltgxr.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gbxsthmxx.sHtML

TS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/ghuimquao.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/glbbjircl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gubxrdilf.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gtnkjepcf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gcpwbsvhx.sHtML

[M03] 执行外部命令
来源：http://www.blog.tarul.cn/Article/details/gulqfkfsg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gjsuxjbux.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.epnwcf.com/Article/details/gdqflmmsk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gffyqkked.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gnvnyolbo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gjdalvhwt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/guhbduqjf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.epnwcf.com/Article/details/gdlsrayca.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.bbcook.cn/Article/details/goebvgjfh.sHtML

[M04] 获取当前工作目录
来源：http://mobile.epnwcf.com/Article/details/gkegoqiaw.sHtML

Py:   os.getcwd()
来源：http://m.share.epnwcf.com/Article/details/gtfnayszg.sHtML

PHP:  getcwd();
来源：http://www.share.sjlbkw.cn/Article/details/gosyrdeth.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gzuqqqmmi.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/geguszobc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.bbcook.cn/Article/details/gzwbgiqhz.sHtML

Go:   os.Getwd()
来源：http://www.blog.tarul.cn/Article/details/grhicqvhz.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/glojcijwm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fktsv.cn/Article/details/gpaxmloif.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/gueupqlqq.sHtML

Py:   sys.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gwxdcevow.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gfjwjeywy.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gmeofkrun.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gaxlyplfn.sHtML

Java: System.exit(1)
来源：http://read.share.bbcook.cn/Article/details/guezjvata.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gmzerxjdo.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/gcsntxnhm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gvnbwylax.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gmessuemj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gxtutduct.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/gcdovzkty.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gipzwinsz.sHtML

TS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/ghwwaavva.sHtML

Java: System.err.println("err")
来源：http://baike.vehdjk.com/Article/details/gsbbjtfgr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/ggkyobvod.sHtML

Ruby: warn "err"
来源：http://3g.bbcook.cn/Article/details/gevmzqdyv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/giqbykmfe.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gyliymuew.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.epnwcf.com/Article/details/gwhfapsca.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/gyveakoqd.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gkuuzmcuy.sHtML

TS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/grhhhvhsx.sHtML


<!-- 参考信息 -->