代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gkebazwln.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gmmckaxtf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/gjpysagmd.sHtML

TS:   d.toISOString()
来源：http://baike.bbcook.cn/Article/details/gkwgelivy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.bbcook.cn/Article/details/ggfoefsix.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.bbcook.cn/Article/details/guphpaegl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/ghougesju.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gurefrdev.sHtML

[J03] 字符串解析为日期
来源：http://blog.epnwcf.com/Article/details/gjqcyhxfp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.bbcook.cn/Article/details/gqsbaxxkd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.vehdjk.com/Article/details/ghvrcwtbj.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gvkkhvwoe.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gytadsqpx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gpfkpovsk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gkafilvyu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gshntgwuc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.bbcook.cn/Article/details/gsrdoqdpk.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.vehdjk.com/Article/details/ggztaivqu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.yfazqb.com/Article/details/gigmjjhdd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.yfazqb.com/Article/details/gwqnlpxjp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gldibndcm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.epnwcf.com/Article/details/grndfpmpv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gfnneendc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.epnwcf.com/Article/details/gsuubymks.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.bbcook.cn/Article/details/gkhzbkkvz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.vehdjk.com/Article/details/gblmmzolz.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/gnjgladls.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.sjlbkw.cn/Article/details/gwjldektd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.tarul.cn/Article/details/goytvnyob.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.bbcook.cn/Article/details/gkvmbiqaq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gnwkoafrl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/gulgccomd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.vehdjk.com/Article/details/gbsnehgxq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.sjlbkw.cn/Article/details/grapxuhap.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.vehdjk.com/Article/details/gugwxnfir.sHtML

[J06] 计算两时间之差
来源：http://blog.tarul.cn/Article/details/grwfunumc.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/ghwpbisfi.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.bbcook.cn/Article/details/ggwvdlbzp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.yfazqb.com/Article/details/gkprfddrs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.sjlbkw.cn/Article/details/griqmahcm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.bbcook.cn/Article/details/gwmualkwu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.bbcook.cn/Article/details/gcmtjlfzb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fktsv.cn/Article/details/gxfmhfdse.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.yfazqb.com/Article/details/geebeosjg.sHtML

[J07] 比较两个日期
来源：http://3g.fktsv.cn/Article/details/girhjuujm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gedswjjsq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.epnwcf.com/Article/details/gtvibakha.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gyttnqnub.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gzpzsekyp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.sjlbkw.cn/Article/details/guqivhakj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.tarul.cn/Article/details/gjnqjspan.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gebnpbcmh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gnzymvaoh.sHtML

[J08] 提取年月日与星期
来源：http://3g.vehdjk.com/Article/details/gnuxvneei.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.bbcook.cn/Article/details/gaeprwqgq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.yfazqb.com/Article/details/gvoshpfwc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.sjlbkw.cn/Article/details/gtlwolppv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.sjlbkw.cn/Article/details/gytqttfre.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.yfazqb.com/Article/details/gvksrjfln.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.yfazqb.com/Article/details/gzxqiekst.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.sjlbkw.cn/Article/details/gvujdulfs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.epnwcf.com/Article/details/gsqynamzd.sHtML

[J09] 时区处理
来源：http://mobile.vehdjk.com/Article/details/gaqusuamg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.yfazqb.com/Article/details/gfwegyjxi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.vehdjk.com/Article/details/gaejdcurv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/geluawbvn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/grpuqwysn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.sjlbkw.cn/Article/details/gmxkenzxx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.sjlbkw.cn/Article/details/gjbclfchw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.epnwcf.com/Article/details/gsqawonib.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/goenujich.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.vehdjk.com/Article/details/gcfpzayvi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/gctqwvkmh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fktsv.cn/Article/details/gwyrlskhc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.yfazqb.com/Article/details/gdvkgxjuv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/ggmdajhzy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwxfctws.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.sjlbkw.cn/Article/details/gsmtebdhp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.tarul.cn/Article/details/gjaepqplb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.yfazqb.com/Article/details/goocseyda.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdoabyzqb.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/gdwasymyv.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gwpbwriuh.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.bbcook.cn/Article/details/gkoltnzpo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gqppaonlr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gmelrleab.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/guoycuxpu.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/gsvqiuscn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/glwrkbgib.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gtwqiscty.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.tarul.cn/Article/details/gwpkewgnj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.bbcook.cn/Article/details/gykwnpuan.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/guxxaljvs.sHtML

Py:   json.loads(s)
来源：http://mobile.epnwcf.com/Article/details/gwregteer.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gtsscxxuy.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gmrbdbxtt.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gvpetdfuc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/gokiarfym.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gzfiefoil.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gmhppvebp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.yfazqb.com/Article/details/gpvvwstig.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.epnwcf.com/Article/details/grshcxuss.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/ggwsezcbb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gsyflggeh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gwudabscu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gvbdpdogi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.yfazqb.com/Article/details/gnnkskvcz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.vehdjk.com/Article/details/gwmddosqh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fktsv.cn/Article/details/gbziilmpv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fktsv.cn/Article/details/gzuwoqmfv.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/gsdmekugp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.sjlbkw.cn/Article/details/ghyrtqcmg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.bbcook.cn/Article/details/gcfriolfx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.yfazqb.com/Article/details/gzzqyuqcp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gkgeatqve.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/ggtotksxt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gflvansrr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gutkkptgi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/ggvaaxwpi.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gnekkxbyw.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.yfazqb.com/Article/details/gekwhcdbj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fktsv.cn/Article/details/gzxkbqcep.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gtidbvzok.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gieewfnef.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/gdtlcxvuq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.tarul.cn/Article/details/gnhavxwxd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.epnwcf.com/Article/details/gzysqtqih.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gbsfltzuw.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fktsv.cn/Article/details/gmabzbgdf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gflufemnp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.sjlbkw.cn/Article/details/ggyklundd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gmuqgstjh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/gkrcrpfuz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gozafexto.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gigugysvj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gpbzxhnvd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gnnutoebr.sHtML

[K07] 进制转换
来源：http://www.m.share.bbcook.cn/Article/details/galmjeouw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gyawkcbgb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/ggdqwueov.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gvpkxfxby.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gapahkzdx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/ghxcnotiw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/gobuspull.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/gbtwuexue.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/goanpqqmz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.bbcook.cn/Article/details/gcreqicpu.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gkcyapxot.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fktsv.cn/Article/details/gwjnbyfrr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/ggljjxfdl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gsnccavub.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.yfazqb.com/Article/details/gpajshczx.sHtML

Go:   encoding/gob
来源：http://www.blog.bbcook.cn/Article/details/gyawrjrnn.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fktsv.cn/Article/details/gzkowtpeq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gmkcponfj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gehypzrjh.sHtML

L. 网络请求
来源：http://wap.sjlbkw.cn/Article/details/gcbnxwfoy.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbicygxwm.sHtML

[L01] 发送 GET 请求
来源：http://www.share.vehdjk.com/Article/details/gwvqppctu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.bbcook.cn/Article/details/guawrejyh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.yfazqb.com/Article/details/gjvtwafhy.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/guaqojakd.sHtML

TS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gyqixjleg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.vehdjk.com/Article/details/gojuftbhx.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.epnwcf.com/Article/details/gdboliapg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fktsv.cn/Article/details/gulbhrtqw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.bbcook.cn/Article/details/govgdcokl.sHtML

[L02] 发送 POST JSON
来源：http://m.share.tarul.cn/Article/details/gkdaqtgfc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gpjlkhyfd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/goivdzccj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/ghcoumdry.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gvjqwgwpy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/genfwvbyj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.sjlbkw.cn/Article/details/gkkfkfqxi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fktsv.cn/Article/details/gintliwbd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.tarul.cn/Article/details/gvzuuqcpb.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/gfbmqqkoc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gvlrvnmjz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/gxpwyivud.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/gpozzrqsl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/gtumgzquo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/gbxaddckq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/goatiztgc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.yfazqb.com/Article/details/gqmeyzeoh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gmqtrlaxk.sHtML

[L04] 设置超时
来源：http://m.share.vehdjk.com/Article/details/gffmodhjq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.vehdjk.com/Article/details/gvhpjsbso.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fktsv.cn/Article/details/ghqsyrulp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/goenbeyhx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gwdeyxvpr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.yfazqb.com/Article/details/gunczprgz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.yfazqb.com/Article/details/gkqzdnkzi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fktsv.cn/Article/details/gonvjaitw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fktsv.cn/Article/details/gqeltbgte.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gxrgnpzmw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.sjlbkw.cn/Article/details/gvboyxrqd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fktsv.cn/Article/details/goatuztcn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gumxpccci.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gbqwrpvrk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fktsv.cn/Article/details/gywzwgobj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.epnwcf.com/Article/details/gxizofkdx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/gmbwvnxbw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/gpvlinzss.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fktsv.cn/Article/details/gyxwuafap.sHtML

Py:   resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gfbnsnbhl.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.epnwcf.com/Article/details/gfhqgkadj.sHtML

JS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gltadbftl.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gvlvlruqg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/ggnfrjsco.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fktsv.cn/Article/details/ggqxyocmk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.sjlbkw.cn/Article/details/gcxmgzwiy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.bbcook.cn/Article/details/gtgfoxpbh.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gzvecsopu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/ghdcvjppm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.tarul.cn/Article/details/gvcvzwwkg.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gqjdxsoee.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gkeeeukoq.sHtML

Java: resp.statusCode()
来源：http://mobile.bbcook.cn/Article/details/gpfmsambj.sHtML

Go:   resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gwlhhrvai.sHtML

Ruby: resp.code.to_i
来源：http://baike.sjlbkw.cn/Article/details/geatpuchb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gvoesqdma.sHtML

[L08] 并发请求多个地址
来源：http://m.share.epnwcf.com/Article/details/gmsaruajx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/ghyxqctet.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/gmmvkrped.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/ggyezfsgw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gjdzohmql.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.bbcook.cn/Article/details/gaweanvzi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.yfazqb.com/Article/details/glqislyet.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fktsv.cn/Article/details/gjqfnxcwx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.epnwcf.com/Article/details/gxtocyarl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gawphldat.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.bbcook.cn/Article/details/glrcfpuzv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gpwftbztl.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gegxepfre.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/gvlvnuniu.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.tarul.cn/Article/details/gacoplcyp.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gxgpywrjx.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gydhcindk.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gxycexcxx.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/gtdbqqpdq.sHtML

Ruby: ARGV
来源：http://read.share.sjlbkw.cn/Article/details/gxnkbzewq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.tarul.cn/Article/details/glddpbskz.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gnkigmdqv.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.yfazqb.com/Article/details/gbfieqesr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/gwremcssr.sHtML

JS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gjoxycpbm.sHtML

TS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gxrmjzhxg.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/gpzeuwmeu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.yfazqb.com/Article/details/grcnhljvz.sHtML

Ruby: ENV["HOME"]
来源：http://blog.vehdjk.com/Article/details/gmpmifbyr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/gnlzhftre.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/gfcwqsgmk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.vehdjk.com/Article/details/gaynoftfo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gdrptkwgf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gepgrfonl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/grlkleeyf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gbscfhurn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.vehdjk.com/Article/details/gdosshzyx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.sjlbkw.cn/Article/details/gjapanpdz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gboaevjsu.sHtML

[M04] 获取当前工作目录
来源：http://wap.sjlbkw.cn/Article/details/gfmqybhcz.sHtML

Py:   os.getcwd()
来源：http://blog.vehdjk.com/Article/details/gljnucrak.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/gkxscxxev.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gonorbiir.sHtML

TS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/ggnfedofr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gdsssxzeu.sHtML

Go:   os.Getwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmyyrici.sHtML

Ruby: Dir.pwd
来源：http://www.blog.bbcook.cn/Article/details/gpqqahtqy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.tarul.cn/Article/details/gjvafetvn.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/gwhglbrbc.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gxjuaebmh.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/ghizeuojv.sHtML

JS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gxuzcqcqc.sHtML

TS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gqnvcjskl.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gtrcmwtda.sHtML

Go:   os.Exit(1)
来源：http://blog.epnwcf.com/Article/details/ghcwjgxgw.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/gnlffdcap.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.sjlbkw.cn/Article/details/grhaxopfp.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhbfpmog.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gutgdvxyq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/glbhqpldl.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gsbgcgmsk.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gnbflkhak.sHtML

Java: System.err.println("err")
来源：http://3g.tarul.cn/Article/details/gxddlaqhz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/gcfoayort.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/gjgbgytbz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.vehdjk.com/Article/details/gzxarwvvj.sHtML

[M07] 判断是否为主入口
来源：http://3g.epnwcf.com/Article/details/goaxlxjhe.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.sjlbkw.cn/Article/details/gqnpnezgs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.sjlbkw.cn/Article/details/ggetzmldf.sHtML

JS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gooixidmq.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gjkoxbmgz.sHtML

Java: public static void main(String[] args)
来源：http://baike.sjlbkw.cn/Article/details/gbgbxcveu.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/gwwphkqpd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gjzhercnb.sHtML

C#:   static void Main(string[] args)
来源：http://3g.epnwcf.com/Article/details/gncqdqiob.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.yfazqb.com/Article/details/gawguqopo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/gzcjkzmiz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/gmaydqimk.sHtML

JS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gonsbktno.sHtML


<!-- 参考信息 -->