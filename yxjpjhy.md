代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/glphuidct.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/gmzokbnes.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/gzpmjxntd.sHtML

TS:   d.toISOString()
来源：http://www.m.share.tarul.cn/Article/details/guxlgesbg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fktsv.cn/Article/details/gfhttqrxl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.tarul.cn/Article/details/gocyerufr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/gnsxhxtxl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbutrmas.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fktsv.cn/Article/details/gacxrpwps.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.bbcook.cn/Article/details/gbxgndfrv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fktsv.cn/Article/details/gwlutgjlm.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gcbuzmglb.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gougohxuv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gfiupqyee.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gjporzxbt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gcxmlyejp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/gfkbdtqjt.sHtML

[J04] 时间戳与日期互转
来源：http://wap.tarul.cn/Article/details/gyikmwknu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.yfazqb.com/Article/details/gerkdyfkf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.epnwcf.com/Article/details/gclwxxyce.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gfiuspvya.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fktsv.cn/Article/details/gzfycffar.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.yfazqb.com/Article/details/gkhkbjxkq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.bbcook.cn/Article/details/gubpeccgx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fktsv.cn/Article/details/gpdsvxzag.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.yfazqb.com/Article/details/gnfpkvuww.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.vehdjk.com/Article/details/gdvgrvvhw.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.sjlbkw.cn/Article/details/gmzxfmyom.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/glhgpzxgq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/guuqxxfyz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/ggourgjuz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fktsv.cn/Article/details/guqwbzeka.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/grfnqckzx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.tarul.cn/Article/details/gjelamjqu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.yfazqb.com/Article/details/gyhfflweg.sHtML

[J06] 计算两时间之差
来源：http://baike.fktsv.cn/Article/details/giwpbvdsz.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fktsv.cn/Article/details/gohcjinhc.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.bbcook.cn/Article/details/gyrknehur.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.sjlbkw.cn/Article/details/ghxchdzym.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.bbcook.cn/Article/details/glrqdtpuo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.vehdjk.com/Article/details/gfvsszdqc.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.yfazqb.com/Article/details/gqawaflcx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.sjlbkw.cn/Article/details/ggpuawvyp.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fktsv.cn/Article/details/gpfjfaqsh.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fktsv.cn/Article/details/gisxulxid.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/glmuaskny.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.vehdjk.com/Article/details/gjlocsevc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gmfcfeoci.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gyicpahkg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.vehdjk.com/Article/details/ggjzmsmck.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.yfazqb.com/Article/details/gjrywodce.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/guvbprxqa.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gtuvwkflu.sHtML

[J08] 提取年月日与星期
来源：http://www.share.yfazqb.com/Article/details/gqsaxhdmo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.bbcook.cn/Article/details/gfrrjccib.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/gcdgtigfa.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.epnwcf.com/Article/details/gxnolfznn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fktsv.cn/Article/details/gygaiamva.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.bbcook.cn/Article/details/gpsbbavdt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.epnwcf.com/Article/details/grxmukroh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/gnjnavuwa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fktsv.cn/Article/details/gxbdhgibl.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/gftkaooxw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.epnwcf.com/Article/details/gizuddpyy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.sjlbkw.cn/Article/details/glypncfoy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/gwdkrkxqx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/gngherjdc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.yfazqb.com/Article/details/gtagjoygh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.bbcook.cn/Article/details/gyrkqyvsy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.sjlbkw.cn/Article/details/ggcjwjxsy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.tarul.cn/Article/details/gnrluktzd.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/gkkcrlhtx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.bbcook.cn/Article/details/gijgjvhol.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gxjwlttvb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gjvjnzjcl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.yfazqb.com/Article/details/gagagwngc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.sjlbkw.cn/Article/details/gogzmrmse.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.tarul.cn/Article/details/gewypfsdk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.vehdjk.com/Article/details/gzsdsrank.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.sjlbkw.cn/Article/details/gtssnglxc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxbbglpmq.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/ghdiirjtj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gygauvxjx.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.tarul.cn/Article/details/gqqniiheu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gjsjmedfp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gwriifjql.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gvmddtzhg.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gbjnbaaec.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/gufgwbqqz.sHtML

Go:   json.Marshal(obj)
来源：http://3g.yfazqb.com/Article/details/gtllotipq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/gcxrcjhnw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.sjlbkw.cn/Article/details/ggpautxso.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.epnwcf.com/Article/details/gplauzojq.sHtML

Py:   json.loads(s)
来源：http://blog.vehdjk.com/Article/details/ggowtlvoz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.yfazqb.com/Article/details/ggrwkgadc.sHtML

JS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/guwtzhsbw.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/grbyrnhyb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.vehdjk.com/Article/details/gmhobtsgp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gzlcocmnb.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gtfkmmrym.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.bbcook.cn/Article/details/gdgizlimm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.epnwcf.com/Article/details/gwxgyeowf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gzediorct.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/gdttqplzo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gmqjbwlap.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gwjnoozko.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.bbcook.cn/Article/details/gacokezqb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.epnwcf.com/Article/details/grgrlzbeo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.vehdjk.com/Article/details/gltqnnkcz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gsyhizonc.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/gxfxzdzic.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gyyjgodmx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fktsv.cn/Article/details/gardpcvpw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gcbvvosfx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gyzsntbso.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fktsv.cn/Article/details/gyprfidrm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gpfgepwnc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gqxswvrfl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fktsv.cn/Article/details/gdgmkbfdw.sHtML

[K05] 深拷贝对象
来源：http://wap.sjlbkw.cn/Article/details/grxrgpbuq.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.yfazqb.com/Article/details/gjhajgcgq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.bbcook.cn/Article/details/grqcpkcad.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gzhpkyfnq.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gpefqxeus.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.epnwcf.com/Article/details/gwzsmpwrg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/gbvcupita.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/graxlfstr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.bbcook.cn/Article/details/gjbczugcu.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/grzeuuily.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gskfwknxk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.yfazqb.com/Article/details/geoclggbi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gtkrulajv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gkpdnsrnz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.vehdjk.com/Article/details/glpglxkds.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/ghkdlplmu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gkwqruvgp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/ghaekbxhn.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/gqortosoh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gneerxcfw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.tarul.cn/Article/details/gamawnuua.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gcgeaevjw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/goduourfb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/glepufjvy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/goapckefp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.sjlbkw.cn/Article/details/gmmqzjkfx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gxwkfavzc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/gxdqzwygw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/gjsythvxs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/ggaynddou.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gvlurorck.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gcqiyuqpf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/gnmgtqovr.sHtML

Go:   encoding/gob
来源：http://wap.yfazqb.com/Article/details/gfebbzkrl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/glvlhxamf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gxscrkwcx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gjqstafdx.sHtML

L. 网络请求
来源：http://wap.sjlbkw.cn/Article/details/geyysrfli.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gujyqzoaz.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/gffkldnhv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.epnwcf.com/Article/details/gjewmhbnm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fktsv.cn/Article/details/gqwtpdemn.sHtML

JS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gseqknisr.sHtML

TS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gxwxvcvps.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.epnwcf.com/Article/details/gadtawbkt.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.tarul.cn/Article/details/gcspwabqh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.epnwcf.com/Article/details/gsqlnpcmr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.vehdjk.com/Article/details/gblfqdyhf.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/gpbkcraxc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gpabqpudy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gmchyeixl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gozzoyheg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuszzmvv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.tarul.cn/Article/details/gibprkjcc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.tarul.cn/Article/details/grbdniwwb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/glwznygpv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fktsv.cn/Article/details/gjlmqanxn.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/gnncdnnni.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.sjlbkw.cn/Article/details/gfvjaetir.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.tarul.cn/Article/details/gtypsjmua.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gfqzmqnhk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gtuabngbz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.bbcook.cn/Article/details/grrcgrktk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gddkzqaju.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.bbcook.cn/Article/details/glxiobytz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gmgaxqaun.sHtML

[L04] 设置超时
来源：http://www.blog.tarul.cn/Article/details/guuplixmb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fktsv.cn/Article/details/gyxnjyjse.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/gbnwzlnlt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/geftzltdn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/glndtadvu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.sjlbkw.cn/Article/details/gfcgmlpoe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gxatsvxrl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fktsv.cn/Article/details/gutbjubkq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.epnwcf.com/Article/details/gesvvyhmi.sHtML

[L05] 上传文件（multipart）
来源：http://wap.sjlbkw.cn/Article/details/gfcpcomrk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fktsv.cn/Article/details/gdinxfpsg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.bbcook.cn/Article/details/gmvclbwqy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/ggycyefvr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/gmstclzjl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/glqwrkuqq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/guybgyixj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.vehdjk.com/Article/details/gpyggclzw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/gptrepawt.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.yfazqb.com/Article/details/gibavngwx.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/gqvvbqpow.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.vehdjk.com/Article/details/gmwrfskbq.sHtML

JS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gdjgayoux.sHtML

TS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gqefhqymv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.epnwcf.com/Article/details/ggnseyofg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.yfazqb.com/Article/details/givbtmwcd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/gooozyzdt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gzksirnre.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gfauvtqua.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.epnwcf.com/Article/details/gpsxkzwzc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.vehdjk.com/Article/details/gnnfowmgs.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gyhnqelcb.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/grfubkjvu.sHtML

Java: resp.statusCode()
来源：http://blog.epnwcf.com/Article/details/gnbjprtin.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gmejxxyca.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/grjnubcba.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gekurefbj.sHtML

[L08] 并发请求多个地址
来源：http://mobile.sjlbkw.cn/Article/details/guxhwmovh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fktsv.cn/Article/details/grlzeihfk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnrkqesh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/greavdjed.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gaufbfabt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.yfazqb.com/Article/details/ghxamxlqy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.bbcook.cn/Article/details/gcnmwedam.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.yfazqb.com/Article/details/gzaequzgs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gdakhrhlx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grzekwurw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.vehdjk.com/Article/details/gcoliqtek.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gorfwzhkw.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gjskdokwf.sHtML

Py:   sys.argv[1:]
来源：http://www.share.vehdjk.com/Article/details/gdhbtfarb.sHtML

PHP:  $argv;  $argc;
来源：http://3g.tarul.cn/Article/details/gzsbkpswb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/giiwcrxlk.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/ghifzbyfn.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gbnvmwioo.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/gqsjvsrxt.sHtML

Ruby: ARGV
来源：http://read.share.sjlbkw.cn/Article/details/gurdyfwcy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gjocbfyqw.sHtML

[M02] 读取环境变量
来源：http://m.share.tarul.cn/Article/details/gqusgpyhu.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gyjnguliu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gzbdmucat.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gdnmhhiqx.sHtML

TS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gjjiuievo.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gtikccvma.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gpswfzyjv.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gxphoqdkh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/goostwbfd.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/gzmvyqkts.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.vehdjk.com/Article/details/gtdcndlhq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.sjlbkw.cn/Article/details/gbomivluj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/guvehoijk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gbnirvgew.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/genbtnzqb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.bbcook.cn/Article/details/gmgwptilw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.yfazqb.com/Article/details/giarwdgsp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/gjxzsckze.sHtML

[M04] 获取当前工作目录
来源：http://www.share.vehdjk.com/Article/details/gryveindk.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/giqkfmqyc.sHtML

PHP:  getcwd();
来源：http://blog.fktsv.cn/Article/details/gvlsxnplo.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gjhqcnvdx.sHtML

TS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/grbddurzz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/gefcmtold.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/gbblglxtn.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fktsv.cn/Article/details/gdnovcsvt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.yfazqb.com/Article/details/ggyijgrvf.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/gbrmdzvrc.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/geoshszuz.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/guffkqngt.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gszugutfn.sHtML

TS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gkoaxsawg.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gztdxhmql.sHtML

Go:   os.Exit(1)
来源：http://blog.epnwcf.com/Article/details/gqrcchvxk.sHtML

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/gvumjjkfl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.sjlbkw.cn/Article/details/gwbitrmxn.sHtML

[M06] 向标准错误输出
来源：http://3g.bbcook.cn/Article/details/gpaqcanza.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gydmkxccf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.yfazqb.com/Article/details/grznhbpbz.sHtML

JS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gdiypuurh.sHtML

TS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gwyrqapsw.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/gfjyiuuli.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.bbcook.cn/Article/details/gylqoljxx.sHtML

Ruby: warn "err"
来源：http://www.share.fktsv.cn/Article/details/gtcvhatps.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fktsv.cn/Article/details/gsyvgzcfv.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/glhtsavlt.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.tarul.cn/Article/details/gpxlirnlv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/gimbpxyqn.sHtML

JS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gmfwcjmhg.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/ggteedvtq.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gfcgeqrhp.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gevkqytoq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fktsv.cn/Article/details/gqubtullg.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gscgjzmqe.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.yfazqb.com/Article/details/gpxutyoqw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.vehdjk.com/Article/details/gvmdonscj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.epnwcf.com/Article/details/ghvzxllgn.sHtML

JS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gqdokhymv.sHtML


<!-- 参考信息 -->