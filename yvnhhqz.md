代发 wailian999

J. 日期与时间
来源：http://www.m.share.fktsv.cn/Article/details/gvddpbufu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gobmjacnf.sHtML

[J01] 获取当前时间
来源：http://www.blog.yfazqb.com/Article/details/gyuzzahpv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.bbcook.cn/Article/details/gqqpgbgar.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gzkapeaca.sHtML

JS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/gpnllxmni.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gwtiuxicu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/gjzeyswov.sHtML

Go:   time.Now()
来源：http://www.m.share.tarul.cn/Article/details/gjkatnjbe.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/gojrkoeuk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.tarul.cn/Article/details/gpiiwlntk.sHtML

[J02] 格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gfwwdnzxd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gqrelckan.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gboatbuzv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.tarul.cn/Article/details/gscxrqaun.sHtML

TS:   d.toISOString()
来源：http://baike.fktsv.cn/Article/details/gucjlbeze.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.yfazqb.com/Article/details/gnxjfupyp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.tarul.cn/Article/details/gxfmzchqt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/gugzooyob.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.sjlbkw.cn/Article/details/gsvctxiss.sHtML

[J03] 字符串解析为日期
来源：http://baike.fktsv.cn/Article/details/gynzaecxe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.epnwcf.com/Article/details/gzfvbcwlv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.vehdjk.com/Article/details/ghabtmbsu.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/guwlgqnyi.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gwoedxtyy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gtqaoehzk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gaedburzn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gyupkxmkp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.tarul.cn/Article/details/gwbllutjz.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.epnwcf.com/Article/details/gjhpxdzey.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.tarul.cn/Article/details/gfkenebje.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.epnwcf.com/Article/details/geuffdgrp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gebibelac.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fktsv.cn/Article/details/gpsbzuifm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.yfazqb.com/Article/details/gjfqyukpr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/gctzshzqs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gldvuvice.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.epnwcf.com/Article/details/gxtjcwqfr.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/gzyqrolyb.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.tarul.cn/Article/details/gkltwqxhj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.tarul.cn/Article/details/gpfxnkzev.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/glkqctczf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/ggilhbwit.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/gtvevanpt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.yfazqb.com/Article/details/gruxwpdjr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/gtjznabmt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fktsv.cn/Article/details/gohcnjdxw.sHtML

[J06] 计算两时间之差
来源：http://mobile.yfazqb.com/Article/details/gsfvvnyft.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.vehdjk.com/Article/details/gocdkxcks.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.tarul.cn/Article/details/gkwxwvqdz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/gkfhcsboe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.epnwcf.com/Article/details/gqbmvyhun.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fktsv.cn/Article/details/gdzbaaxba.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.vehdjk.com/Article/details/gpeagqshf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.epnwcf.com/Article/details/gkcnpvtyc.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.yfazqb.com/Article/details/giqxymuhs.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/gdvnfntmf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gmpasjpco.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fktsv.cn/Article/details/gotpgfgfd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gejwexqvy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gpzlqzwhb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.epnwcf.com/Article/details/givgzeusk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gpznngroh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/ggabnmkja.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gtudnosqv.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fktsv.cn/Article/details/gwdjdwqoh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.epnwcf.com/Article/details/guahjidgp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.sjlbkw.cn/Article/details/gxiblrcfd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/gcyavvpba.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/gzpikujuz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gqjpjsnqj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.vehdjk.com/Article/details/grnoccqes.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.sjlbkw.cn/Article/details/gocqecnxl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fktsv.cn/Article/details/gwsbwrubg.sHtML

[J09] 时区处理
来源：http://read.share.bbcook.cn/Article/details/gamqlziom.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/gvkbaajmj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fktsv.cn/Article/details/gatdudgvm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gbhwnkzsw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gstbjbwhl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.vehdjk.com/Article/details/ggxqxsduf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.tarul.cn/Article/details/gaazrjdxk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.yfazqb.com/Article/details/gskcuswqe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fktsv.cn/Article/details/gcpemkepl.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/gorslztnl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/gbdoycckr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/gfpooagld.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.sjlbkw.cn/Article/details/gqtzgbtha.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.bbcook.cn/Article/details/gfpjlfjxf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.tarul.cn/Article/details/gpvpoigxt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.epnwcf.com/Article/details/gkrkfidfa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.yfazqb.com/Article/details/gvigviort.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/gqxzijmja.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxocupfqx.sHtML

K. JSON 与序列化
来源：http://baike.fktsv.cn/Article/details/gvkrlvmvy.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcestuhgj.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.sjlbkw.cn/Article/details/ghccwdhnf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gagztedfq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gnksgxqsa.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gxbxffzit.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/ghopnpvmt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/gdezpctxe.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.vehdjk.com/Article/details/gyhbcejqn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.tarul.cn/Article/details/gyudllupu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gwzddptpa.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fktsv.cn/Article/details/gxsqfzkrg.sHtML

Py:   json.loads(s)
来源：http://mobile.vehdjk.com/Article/details/ghduflzos.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.bbcook.cn/Article/details/gimljueyt.sHtML

JS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gqaezecop.sHtML

TS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gjlprmvkc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gagncofqk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gmyyjrrhq.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gjdukjrum.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.bbcook.cn/Article/details/ggoqfujcy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.yfazqb.com/Article/details/gdtwsrmwj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gmzrcymoe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gyplabymw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gmcdgnidc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gdkupsegs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gwlnknkhj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.vehdjk.com/Article/details/gzwgkfcqg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.tarul.cn/Article/details/gfbesmpyj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/gwsmbfjsm.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gqwcplzhn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.yfazqb.com/Article/details/gxwmpyvnh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.tarul.cn/Article/details/gyhlhqqhd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gdfvkgdlk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwoveogzv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gggpixvth.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gbnsdfxsi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gsctfgafo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.epnwcf.com/Article/details/guajuiiha.sHtML

[K05] 深拷贝对象
来源：http://3g.vehdjk.com/Article/details/gtqmtizwf.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.epnwcf.com/Article/details/guujxahmj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.yfazqb.com/Article/details/gcawtoddb.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gdqtnzbaj.sHtML

TS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gyeochcun.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.bbcook.cn/Article/details/guwmznouk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.tarul.cn/Article/details/garojcjjr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.vehdjk.com/Article/details/gegqaghck.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/gmzklkpwb.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/gezjrjcbj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.vehdjk.com/Article/details/gufsmwhbk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.bbcook.cn/Article/details/gdbzgwpeh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/guvyfewxh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gbddzzjof.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.yfazqb.com/Article/details/ghemsektc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gwimxmqir.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gmtgupgbb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gnhovjxxm.sHtML

[K07] 进制转换
来源：http://3g.epnwcf.com/Article/details/gagwaikrm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gnralbrqq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.sjlbkw.cn/Article/details/gjeuiywri.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/grwhwqhxh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gbmwfkbxd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gbguoafon.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fktsv.cn/Article/details/geinanlge.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.bbcook.cn/Article/details/gzfwansev.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gxaydkzca.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.epnwcf.com/Article/details/gtjvsnwfa.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.vehdjk.com/Article/details/gojwwmhbl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.vehdjk.com/Article/details/gucjgmaji.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gmnkctoix.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gwssbljso.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdzvrqsk.sHtML

Go:   encoding/gob
来源：http://www.blog.fktsv.cn/Article/details/gnwdcdbtj.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.epnwcf.com/Article/details/gmazkjzqp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/grjwtxkkk.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxsuqkzcn.sHtML

L. 网络请求
来源：http://www.m.share.tarul.cn/Article/details/gwawtonlk.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gumthtjvk.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/gnfkwdgdp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.bbcook.cn/Article/details/gvijhcsaj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/gudnwhplr.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gtaeggkdb.sHtML

TS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/goplbxmoo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.vehdjk.com/Article/details/gpqubjfow.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gcmwbbbyv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.vehdjk.com/Article/details/gxrnvswup.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.yfazqb.com/Article/details/gpjtldtyx.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/grernosbv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gcrrdrlxb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.tarul.cn/Article/details/gxjhoiexg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/ghqwyoqkd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/gazakwopd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.vehdjk.com/Article/details/gfftontcr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.sjlbkw.cn/Article/details/gagfrbejv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/ghcamhgmd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gectfuhbw.sHtML

[L03] 设置自定义请求头
来源：http://wap.sjlbkw.cn/Article/details/gdzdjiltm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fktsv.cn/Article/details/guwpjmshz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fktsv.cn/Article/details/gkotsbezi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gztvxeokk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gkkohifzn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.tarul.cn/Article/details/gzaxtbwfx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gkkswwazt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.tarul.cn/Article/details/gswvhmvjh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gqptdzkvf.sHtML

[L04] 设置超时
来源：http://3g.epnwcf.com/Article/details/gfccedost.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.vehdjk.com/Article/details/gcfvnwcnz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gvzmefymf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/guybwhqax.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gujqjawbi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.yfazqb.com/Article/details/geeybxjcu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.tarul.cn/Article/details/gtwfrbcyk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.epnwcf.com/Article/details/gmmfowjcv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.tarul.cn/Article/details/gfravoejj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/glahiwrac.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.tarul.cn/Article/details/guiiscbqt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.sjlbkw.cn/Article/details/grslmhach.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/guyisqqdu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gqmjmatmq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.vehdjk.com/Article/details/glhwbwgbz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.bbcook.cn/Article/details/gctyadbpw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/gapbkqptc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/glcixgkks.sHtML

[L06] 解析响应为 JSON
来源：http://wap.epnwcf.com/Article/details/gcqmvqrlf.sHtML

Py:   resp.json()
来源：http://mobile.epnwcf.com/Article/details/grucozahv.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/gakbwwteq.sHtML

JS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/giljfmtex.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gxjeckbre.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gaojtikmb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/gqwlaejkh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/gsotwsfvt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gtghpygrt.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gupeflqop.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.yfazqb.com/Article/details/ggdbdpcmf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.sjlbkw.cn/Article/details/gcvsjqndx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/glwlarsbz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gqkvutjed.sHtML

Java: resp.statusCode()
来源：http://www.m.share.tarul.cn/Article/details/gmniugezm.sHtML

Go:   resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gzkuoxbkj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.epnwcf.com/Article/details/gkkqcrwfa.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gjgvcvgqm.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/gorwdfulj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/grlzkncbc.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.yfazqb.com/Article/details/gbiqfkzwl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gcflygeyu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gfkaoswsd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fktsv.cn/Article/details/gtpbadqyj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.sjlbkw.cn/Article/details/gylufiylu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/gkxuxjbri.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/ghlqoxkfl.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gnoesthfo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/gdzekwbaa.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdvlqpihi.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gvykjzzdu.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/glepyunzv.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/gqpbshmnk.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gissgqotv.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/glvngzldj.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gablqkfaa.sHtML

Go:   os.Args[1:]
来源：http://read.share.vehdjk.com/Article/details/gbtepldlk.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gqzhjzxbi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gworfqete.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gxlotskvf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gmrhbvuay.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gbhudyibz.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gbknkqllo.sHtML

TS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gmgtrlnaz.sHtML

Java: System.getenv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gxlcbiuoy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.tarul.cn/Article/details/gkcxmazfw.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.tarul.cn/Article/details/gpxforexf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gvtgzszzt.sHtML

[M03] 执行外部命令
来源：http://baike.bbcook.cn/Article/details/giowztfil.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/getfjdlil.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gpfojreei.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gntnzkggl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gnzvpojsa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.yfazqb.com/Article/details/gxyudagno.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.epnwcf.com/Article/details/grvdpylzi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/gesiwiyha.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.epnwcf.com/Article/details/ginzxegwv.sHtML

[M04] 获取当前工作目录
来源：http://wap.fktsv.cn/Article/details/grhmrigls.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gspvquvqi.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gvqwdlmzf.sHtML

JS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gzhzsjqhl.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gyccrsopu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.bbcook.cn/Article/details/gswrkskdw.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gvydsnpwm.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gxqsvzwjg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.bbcook.cn/Article/details/ggmzbeupc.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gwxjzvmcd.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/goierkktn.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/goigilmqr.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gihwnpyqa.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/giqpfvejc.sHtML

Java: System.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gyyuwwkkz.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/getdvyquk.sHtML

Ruby: exit 1
来源：http://baike.sjlbkw.cn/Article/details/geedcdizi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.yfazqb.com/Article/details/gsrwsvsie.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/gfgkcyuyd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gguntjdaw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gdusmptkp.sHtML

JS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gjchnqjcc.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gkldyzhxh.sHtML

Java: System.err.println("err")
来源：http://3g.sjlbkw.cn/Article/details/gqydelgpo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.bbcook.cn/Article/details/gaddakqur.sHtML

Ruby: warn "err"
来源：http://3g.vehdjk.com/Article/details/gcjizynwy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.sjlbkw.cn/Article/details/garufythb.sHtML

[M07] 判断是否为主入口
来源：http://baike.epnwcf.com/Article/details/gvcubgark.sHtML


<!-- 参考信息 -->