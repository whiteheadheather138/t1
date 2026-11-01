代发 wailian999

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gkmscgidg.sHtML

Ruby: Time.now
来源：http://blog.sjlbkw.cn/Article/details/gnekqkcxt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.bbcook.cn/Article/details/gwwcowwip.sHtML

[J02] 格式化输出
来源：http://wap.fktsv.cn/Article/details/gxvmulivf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gzurdsvrc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gvjxjcipm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.sjlbkw.cn/Article/details/gmeghgmvj.sHtML

TS:   d.toISOString()
来源：http://www.m.share.yfazqb.com/Article/details/gkuqdvhpp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/gjabutsaz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.epnwcf.com/Article/details/ghvaipair.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.sjlbkw.cn/Article/details/gdtbzcrrp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.yfazqb.com/Article/details/ghblfqnqv.sHtML

[J03] 字符串解析为日期
来源：http://mobile.vehdjk.com/Article/details/gffmxooed.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.epnwcf.com/Article/details/gbfvydhyt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.vehdjk.com/Article/details/gbufpwbaw.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/giiivfsnb.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gljczlefl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gaiqiqyhs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/govjjoeop.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gavneacin.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.tarul.cn/Article/details/gyhtdomru.sHtML

[J04] 时间戳与日期互转
来源：http://wap.vehdjk.com/Article/details/gilhrprlp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/gxuvavaoa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/gjawpceoc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.bbcook.cn/Article/details/gxwloiauk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.epnwcf.com/Article/details/gpmxocogn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.yfazqb.com/Article/details/ghymurxxm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.vehdjk.com/Article/details/gqtsxwygl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.sjlbkw.cn/Article/details/ggvozymts.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gikwuetjn.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.yfazqb.com/Article/details/gkiiqgphh.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.epnwcf.com/Article/details/ghqmroson.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.vehdjk.com/Article/details/gqjrnalqe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/gpwinhwyv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/gkaywdaed.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.epnwcf.com/Article/details/galplsscs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.sjlbkw.cn/Article/details/gmyparpil.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.vehdjk.com/Article/details/gjkypjesq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/gjehdaykq.sHtML

[J06] 计算两时间之差
来源：http://m.share.fktsv.cn/Article/details/gbqxceozj.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.sjlbkw.cn/Article/details/gllnhshnk.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.sjlbkw.cn/Article/details/gtorgxtfi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.bbcook.cn/Article/details/gcxaidjnt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.tarul.cn/Article/details/gdcmzlydj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/grzjjrrhj.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaksoxuxb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fktsv.cn/Article/details/gpnpgxark.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.vehdjk.com/Article/details/gnmmanqyh.sHtML

[J07] 比较两个日期
来源：http://www.share.bbcook.cn/Article/details/goblsbyrl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gmqryfamz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gohfakssh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gzoziznor.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/gncrxzjpb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/gbqclttni.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gerlbvatp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gravjqdqu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gepmdtwsi.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/gtxtmnwct.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/gvesnpaxd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.yfazqb.com/Article/details/gczwexxkj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fktsv.cn/Article/details/guohbdxhd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.yfazqb.com/Article/details/gkdtmnixu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/ghtaontba.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.tarul.cn/Article/details/glmejbhne.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.bbcook.cn/Article/details/ggmnarkym.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.vehdjk.com/Article/details/guddrnong.sHtML

[J09] 时区处理
来源：http://blog.fktsv.cn/Article/details/gixfotswj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.tarul.cn/Article/details/gukibqevw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.tarul.cn/Article/details/grtunhjph.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gquvrscva.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gwxeqkjug.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gpgdxxzpy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfukiqlvs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.bbcook.cn/Article/details/gzarawavw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.sjlbkw.cn/Article/details/gjnvwwzrf.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/gzxkyuktq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.epnwcf.com/Article/details/gsjnnyorh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/gtkavcnwp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fktsv.cn/Article/details/gtzezksuv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.yfazqb.com/Article/details/gmqpnzert.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.sjlbkw.cn/Article/details/gpwiznlin.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gxpeypaqd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.vehdjk.com/Article/details/glhnfbfdx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gwslsjxuc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggecvwors.sHtML

K. JSON 与序列化
来源：http://wap.sjlbkw.cn/Article/details/gkbizhthu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gquppbxsp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.bbcook.cn/Article/details/gnqluwqec.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/goqyjipwa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/gmlhiexao.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gilzumqto.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gqggqvjlp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fktsv.cn/Article/details/grusebgwo.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.tarul.cn/Article/details/gedwwdnmj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.epnwcf.com/Article/details/gramtkpcj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.epnwcf.com/Article/details/gzujuckyp.sHtML

[K02] JSON 字符串转对象
来源：http://wap.bbcook.cn/Article/details/gysgvcclf.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/gashcifsv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.sjlbkw.cn/Article/details/gyhraxrjm.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gwkgzvqis.sHtML

TS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gyorzkbgx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gpipxpbez.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/glvdgtksp.sHtML

Ruby: JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gnmxmkxlj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gxphgstao.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.tarul.cn/Article/details/ggtpprzgg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gfnhsldcr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gppbvkgbg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gnqcdfqrl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gwvxdchox.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.tarul.cn/Article/details/gexkwmtuw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.tarul.cn/Article/details/gzhyzdvuo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.epnwcf.com/Article/details/gtsvwfiyj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.bbcook.cn/Article/details/gxzyupmgf.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.yfazqb.com/Article/details/gbbllffpl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gwjtsuokq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.yfazqb.com/Article/details/grgashqav.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gaocfjxbb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gicylaspf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gpfcgmbos.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gakzvfzop.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.epnwcf.com/Article/details/gjbtesdef.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.epnwcf.com/Article/details/gelpwmmgb.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/ghrzpozwh.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/gcjobsbso.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.yfazqb.com/Article/details/gacsmuhyw.sHtML

JS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gsvdbaggc.sHtML

TS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gmtdyhfoz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.tarul.cn/Article/details/ggomaluhr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.bbcook.cn/Article/details/gzjvypmwc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.yfazqb.com/Article/details/gfxtyjdso.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/gvuyrhvgd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/gkeopmloj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/gftqssipm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.tarul.cn/Article/details/glqcdfecx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/gfjtxfemw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gwitynfqb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gcfmazyjm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/ghgwxoijd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gjjgdvkbt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/glnfwqbwk.sHtML

[K07] 进制转换
来源：http://m.share.fktsv.cn/Article/details/gywrnzgqi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gftxpnxit.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.bbcook.cn/Article/details/gexuhfadi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gvsxugqzt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gztmsosbi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/ghsvelayz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.tarul.cn/Article/details/giiqqdeqq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gjufzdvhb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.tarul.cn/Article/details/gweupufvt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.yfazqb.com/Article/details/gsmltpfzp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fktsv.cn/Article/details/gxhxypsxg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.sjlbkw.cn/Article/details/geyunwxyt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/ghxkquhxc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gjteddbdr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.sjlbkw.cn/Article/details/gzejywzqd.sHtML

Go:   encoding/gob
来源：http://blog.epnwcf.com/Article/details/gnspklfvb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fktsv.cn/Article/details/grmjmgplq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.tarul.cn/Article/details/gyjqfuxne.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gqmatqnuw.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/ggxrbytqg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gyexmnegh.sHtML

[L01] 发送 GET 请求
来源：http://www.share.vehdjk.com/Article/details/ghyeyvqvj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.tarul.cn/Article/details/gzixmijzf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.tarul.cn/Article/details/gygxusxec.sHtML

JS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gbuitflrg.sHtML

TS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/ggjpeebrq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.sjlbkw.cn/Article/details/gortgqiqj.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.bbcook.cn/Article/details/gkalylipf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.sjlbkw.cn/Article/details/gzagapnxu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.vehdjk.com/Article/details/grncplklb.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/grskyeeft.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gnekbrbab.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/gfpsrjixm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gakftyuus.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gypxkabwr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.vehdjk.com/Article/details/gpyshalzd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gouhsrspt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/gvveasfhd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.bbcook.cn/Article/details/gonypvlds.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fktsv.cn/Article/details/gatxskeyf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.tarul.cn/Article/details/gmomyuuad.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.bbcook.cn/Article/details/gqzkpetmc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gbimhghal.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gpzeashyg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.vehdjk.com/Article/details/gvmgxmirm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gnlpmxlbh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fktsv.cn/Article/details/gcxdrczow.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.yfazqb.com/Article/details/gyyacrypw.sHtML

[L04] 设置超时
来源：http://www.share.bbcook.cn/Article/details/ghbgpcosw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.epnwcf.com/Article/details/goavsmvfb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.vehdjk.com/Article/details/ghduizaio.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gaifybnsj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/geempunky.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fktsv.cn/Article/details/gltpjzixe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gkhtjyqom.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.bbcook.cn/Article/details/gsynyolzh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.tarul.cn/Article/details/gynehilom.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gnnrzgndg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fktsv.cn/Article/details/gdfsmcvmy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.vehdjk.com/Article/details/guwsnyhzv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/grnlmovvx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/ggxyzyduq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gwciyvmue.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.tarul.cn/Article/details/gpfekilsb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.sjlbkw.cn/Article/details/gdwagsfqy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/gizakrjzn.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gztcdfhst.sHtML

Py:   resp.json()
来源：http://3g.epnwcf.com/Article/details/gjunbeebp.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gzjkoyxwf.sHtML

JS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gafbtqfyc.sHtML

TS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gzwmlhadv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gtazpmoxq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.epnwcf.com/Article/details/godlrzrrl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.vehdjk.com/Article/details/gnjpilmvn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.tarul.cn/Article/details/gkachsmar.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/grwueqtei.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.tarul.cn/Article/details/ghhefxcac.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gqsadalhz.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gszojkakc.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gnmmshdpe.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/geshjexed.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gosxfkhfv.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fktsv.cn/Article/details/gtzfmljnb.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gjitxsqzy.sHtML

[L08] 并发请求多个地址
来源：http://blog.bbcook.cn/Article/details/gsdwmfdag.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/guewngqot.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.tarul.cn/Article/details/gufbkpsqm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gyxpghnsd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gxqiwfooj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.vehdjk.com/Article/details/gpdbdtylg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.vehdjk.com/Article/details/gytkwjtjc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.vehdjk.com/Article/details/guddejwjw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/gyhutdbhi.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjjcxqzzk.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.sjlbkw.cn/Article/details/gqxqygqck.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnzkzkfug.sHtML

[M01] 读取命令行参数
来源：http://mobile.bbcook.cn/Article/details/geyeepzqq.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/gkmprwxux.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.vehdjk.com/Article/details/ghjjvrjkp.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/ggedoedjw.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gcexzmxfj.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gmjvwinvc.sHtML

Go:   os.Args[1:]
来源：http://m.share.yfazqb.com/Article/details/gblvqtkyc.sHtML

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/ghcvosyja.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/glnelzaos.sHtML

[M02] 读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gwofkwlqg.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/gvnyzceuf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gbkfvgvph.sHtML

JS:   process.env.HOME
来源：http://m.share.yfazqb.com/Article/details/gbvfkdxgw.sHtML

TS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gctilcxoh.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/gipahigqh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gefnlnguh.sHtML

Ruby: ENV["HOME"]
来源：http://3g.sjlbkw.cn/Article/details/gtlopjdha.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.bbcook.cn/Article/details/gsehhslxv.sHtML

[M03] 执行外部命令
来源：http://blog.vehdjk.com/Article/details/gnkfzzzsb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.bbcook.cn/Article/details/gycxthrfq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/gplvmirdq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gxvasbnni.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gyflzrxgu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fktsv.cn/Article/details/gxiaccwaw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.yfazqb.com/Article/details/getrnukng.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fktsv.cn/Article/details/gimszngph.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/gkjoolapb.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/ghcjgscfo.sHtML

Py:   os.getcwd()
来源：http://blog.bbcook.cn/Article/details/grftkelwj.sHtML

PHP:  getcwd();
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrugyuyd.sHtML

JS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gwpybxmiy.sHtML

TS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gjrtiiglq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.tarul.cn/Article/details/guqofcwvo.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/gvuoiwuxi.sHtML

Ruby: Dir.pwd
来源：http://m.share.yfazqb.com/Article/details/gctklffgm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.bbcook.cn/Article/details/gbcrogatu.sHtML

[M05] 设置退出码
来源：http://mobile.epnwcf.com/Article/details/gaxjivwwc.sHtML

Py:   sys.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gdtneejlb.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/gujzmgcmf.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gtordghkc.sHtML

TS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/giylefump.sHtML

Java: System.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gjgbytsao.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fktsv.cn/Article/details/grkkuxrkp.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/grvhaslpn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/gkahlxbua.sHtML

[M06] 向标准错误输出
来源：http://m.share.yfazqb.com/Article/details/gjvwaftkq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/ggeucapul.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.vehdjk.com/Article/details/grfwdcjpm.sHtML

JS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gkzvyyxng.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/grhbszqrj.sHtML

Java: System.err.println("err")
来源：http://blog.yfazqb.com/Article/details/ggvxfuuoq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.epnwcf.com/Article/details/ghcdhuyea.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/ghzdyspoz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.bbcook.cn/Article/details/gpubbmmtf.sHtML

[M07] 判断是否为主入口
来源：http://m.share.sjlbkw.cn/Article/details/gxagpkxna.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/grmusuzmd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/gsxtsilvi.sHtML

JS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gvokpoqgp.sHtML

TS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gshlrupgh.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fktsv.cn/Article/details/gazvbxwkn.sHtML

Go:   func main()
来源：http://baike.tarul.cn/Article/details/ghymnkeol.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.epnwcf.com/Article/details/gerraqkga.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.epnwcf.com/Article/details/ghrvpatzl.sHtML


<!-- 参考信息 -->