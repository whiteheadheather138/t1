代发 wailian999

J. 日期与时间
来源：http://3g.sjlbkw.cn/Article/details/guvinjgvh.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gupgbxjih.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/gxuciwumb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.sjlbkw.cn/Article/details/gbqqhskvv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.yfazqb.com/Article/details/glndojjxu.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/gkhonhjdc.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gukjfxbkk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.tarul.cn/Article/details/gbdpknuwd.sHtML

Go:   time.Now()
来源：http://baike.sjlbkw.cn/Article/details/gwhtqebnx.sHtML

Ruby: Time.now
来源：http://wap.vehdjk.com/Article/details/gfaksynuw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.sjlbkw.cn/Article/details/gcqgvyiko.sHtML

[J02] 格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/ghunaiecb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/glqdrhrgy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/ghxzjkqvt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.sjlbkw.cn/Article/details/gyaufbcrg.sHtML

TS:   d.toISOString()
来源：http://baike.fktsv.cn/Article/details/gienjofpw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fktsv.cn/Article/details/gumsejzbi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fktsv.cn/Article/details/goehamrmd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gzutthduo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/gdlxefwpi.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.bbcook.cn/Article/details/geecwikeh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.epnwcf.com/Article/details/gzmbrzyos.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.bbcook.cn/Article/details/gdnmrouta.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/ggjaferai.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gnvajlivx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gvtpgfqet.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gthxnkrmm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gikkcjvqr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.bbcook.cn/Article/details/gjepngeqb.sHtML

[J04] 时间戳与日期互转
来源：http://baike.vehdjk.com/Article/details/gmclofabs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.epnwcf.com/Article/details/gxjogkpzg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fktsv.cn/Article/details/ggrwftiyc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.bbcook.cn/Article/details/giwqdqpaf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fktsv.cn/Article/details/gswobhwfc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.yfazqb.com/Article/details/gxkaomyux.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.yfazqb.com/Article/details/gsanthscb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.tarul.cn/Article/details/gwwhspisp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fktsv.cn/Article/details/geqfsjbil.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.yfazqb.com/Article/details/gwylhvvsf.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.vehdjk.com/Article/details/gonwrecpm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.bbcook.cn/Article/details/gljnfibap.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/gtbmkwcxv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gjykrzgkz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.yfazqb.com/Article/details/gdgggdtgl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.yfazqb.com/Article/details/gveupicfv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/gkbejvpsv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/gphhpoapo.sHtML

[J06] 计算两时间之差
来源：http://baike.tarul.cn/Article/details/gjynranqp.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/gzdoxhgkw.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fktsv.cn/Article/details/gmwihyyoo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.bbcook.cn/Article/details/ggzbaftgu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.vehdjk.com/Article/details/gedrojymu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gilewdhnb.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gphwondmo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.yfazqb.com/Article/details/gquzpnzai.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fktsv.cn/Article/details/gmhhjrdkn.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/gntmckfnr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gjavolevw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/goeauvuua.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gytshoaou.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/glkdyypnv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.yfazqb.com/Article/details/gjbnlxasd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.sjlbkw.cn/Article/details/gszjduyqv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gcxqyqqsy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gmxvftutc.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gjkufkrjv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.sjlbkw.cn/Article/details/giyilhdcq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.sjlbkw.cn/Article/details/gtjxhhwxn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.epnwcf.com/Article/details/gibomuudh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fktsv.cn/Article/details/gaoradqym.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.tarul.cn/Article/details/gbtfsnmzt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.tarul.cn/Article/details/gpdpryzah.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.sjlbkw.cn/Article/details/gydptlsuh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.epnwcf.com/Article/details/gcnulixbm.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/gnzlandqp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/ghsdmnpid.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.yfazqb.com/Article/details/glktafdoo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gtmniuxoo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/ggfuhlbvo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.epnwcf.com/Article/details/gqtgvxtjm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fktsv.cn/Article/details/gvxciulhj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gtxqazpfd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.bbcook.cn/Article/details/gnjwreqpq.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.sjlbkw.cn/Article/details/gzsxyhkyi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/gqkyzdhed.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/gscsnsaow.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gioslbmdk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.yfazqb.com/Article/details/gtnoinuod.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.epnwcf.com/Article/details/guepkuvbe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.bbcook.cn/Article/details/gdmtacosw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.epnwcf.com/Article/details/gpvvlufzg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.epnwcf.com/Article/details/gexjunaov.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkzugyeib.sHtML

K. JSON 与序列化
来源：http://blog.yfazqb.com/Article/details/ggohqsyic.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gywxduvvp.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.vehdjk.com/Article/details/gdjfazsqs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gkbhqfekt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gcpkiuazx.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gsfpablmu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gevzptvri.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.sjlbkw.cn/Article/details/guuhtsacu.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.vehdjk.com/Article/details/gnvpyvkvh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.bbcook.cn/Article/details/gdwqtdiwc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.bbcook.cn/Article/details/ggyiztwij.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.sjlbkw.cn/Article/details/gohtveorf.sHtML

Py:   json.loads(s)
来源：http://www.share.vehdjk.com/Article/details/gspwrwuih.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.sjlbkw.cn/Article/details/gbwmvfszp.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/givximnyk.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gvyujjlbg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fktsv.cn/Article/details/ghdqmvbss.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gfjlyhovk.sHtML

Ruby: JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gsbxjvlxa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/gqbexdwqj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fktsv.cn/Article/details/gsfixspdu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/gwjlrzqlo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/ghikoqgwn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gptplojtv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gqwttanam.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.sjlbkw.cn/Article/details/gzukchsbi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/gdulkutps.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fktsv.cn/Article/details/ghqdteifw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.epnwcf.com/Article/details/gsicgsfoc.sHtML

[K04] 读取 JSON 文件
来源：http://baike.tarul.cn/Article/details/gewsxhsrt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.sjlbkw.cn/Article/details/gbrhimrnx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.vehdjk.com/Article/details/grgnvhoua.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gbitugili.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gxsuylsbb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fktsv.cn/Article/details/geehbhjkm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/gddxnzfbn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.vehdjk.com/Article/details/gfgrczmaf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/grjxvtkam.sHtML

[K05] 深拷贝对象
来源：http://mobile.sjlbkw.cn/Article/details/grngsdgfo.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.tarul.cn/Article/details/gsvpioepv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.bbcook.cn/Article/details/gwejjnvht.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gybpfqneq.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/glhxctetq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.epnwcf.com/Article/details/gtjoitcms.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/gosppdyrl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.epnwcf.com/Article/details/gdqzgiukx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.bbcook.cn/Article/details/gqvyvrtiv.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.vehdjk.com/Article/details/gfgbetzat.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/grjrhcfgu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.yfazqb.com/Article/details/gvdddqoio.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gttzklvxm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/ggeowrpkx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gvdmvmdot.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gyyydrtgr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/grqhnrmne.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gxebovejk.sHtML

[K07] 进制转换
来源：http://blog.tarul.cn/Article/details/grmqfgaxw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/giuzxijda.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.tarul.cn/Article/details/gbsizrgao.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gxxaogxbx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/ghhcdnddp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gjkyuccna.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/grnvmxetb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.yfazqb.com/Article/details/gesexwocp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gclhjwfpd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.yfazqb.com/Article/details/gsuwsdhft.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.yfazqb.com/Article/details/gnimdifqn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.bbcook.cn/Article/details/gtqzbhehb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gcpznmenr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gwznimsjo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.vehdjk.com/Article/details/gfjbrvmml.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gencyghvh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gkjqtkwxi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gccpvatup.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghwaakkxm.sHtML

L. 网络请求
来源：http://mobile.epnwcf.com/Article/details/gozahzsqj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggbrzlyjd.sHtML

[L01] 发送 GET 请求
来源：http://www.share.epnwcf.com/Article/details/gcmowkshr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fktsv.cn/Article/details/gtycwhohy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fktsv.cn/Article/details/gmyjxgocc.sHtML

JS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/goczcqftu.sHtML

TS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gmbyfosaj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.vehdjk.com/Article/details/grtcjwbmg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.bbcook.cn/Article/details/grtwnwvsj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/gldwxqjmg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/gsujjzwwc.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gtotudckp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gjldtfawz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.yfazqb.com/Article/details/gbeukbrwk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gbkttdigz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gmhprjakl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gntbihfay.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fktsv.cn/Article/details/gpbpfmdpb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/gliabvnmm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.vehdjk.com/Article/details/gkdosvjse.sHtML

[L03] 设置自定义请求头
来源：http://3g.vehdjk.com/Article/details/grmdhnwur.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.vehdjk.com/Article/details/gskjkmrif.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.vehdjk.com/Article/details/giiwaqwna.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gjfmisxgu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gfayzlanh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.yfazqb.com/Article/details/gqbqcyspn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gyqlwpdkg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.bbcook.cn/Article/details/gbxtdbtxv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/gszouriwd.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gspwomtwy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/ghjovdhna.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.yfazqb.com/Article/details/gtypwtzhp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/gjmqytftz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gzvtsbsto.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gqssrhdfu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gdetdmcat.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.vehdjk.com/Article/details/gwocermel.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.epnwcf.com/Article/details/gddxffxnb.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.sjlbkw.cn/Article/details/gtxqsskdb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.tarul.cn/Article/details/glkfgurxk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gdupadlwq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/giagenywn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gplnvaslf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/gfqamyekc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fktsv.cn/Article/details/giuvkptpd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.vehdjk.com/Article/details/gsfzuwjuy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.vehdjk.com/Article/details/gxzkqoywg.sHtML

[L06] 解析响应为 JSON
来源：http://baike.sjlbkw.cn/Article/details/gjdwzkilq.sHtML

Py:   resp.json()
来源：http://m.share.tarul.cn/Article/details/gjbksppog.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.bbcook.cn/Article/details/gggmfqsqq.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gjurjhmlo.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gnooxeluh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.bbcook.cn/Article/details/gdooljdlf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.sjlbkw.cn/Article/details/gzcubbhxp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.vehdjk.com/Article/details/ghlfcxety.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.sjlbkw.cn/Article/details/gsseazfha.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gdjteobht.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/gzighnvrv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/gfhikgajb.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gvkgzfdlo.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/gkdkrqaiq.sHtML

Java: resp.statusCode()
来源：http://blog.vehdjk.com/Article/details/gnzrciojs.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gqredgbjk.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gctkcqxjt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/glrvossdj.sHtML

[L08] 并发请求多个地址
来源：http://www.share.tarul.cn/Article/details/gcxqdbqas.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.yfazqb.com/Article/details/gosrraksx.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/giptdrxhh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/glsbwdvjz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gxhyejtjc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fktsv.cn/Article/details/gwoikfmod.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.yfazqb.com/Article/details/gxkstowhu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gkadvqmyz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.sjlbkw.cn/Article/details/ghtjcawrp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzhhdhudp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.sjlbkw.cn/Article/details/gngrfslzn.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gyungtzns.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gjwqeurdg.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/gajbezlyk.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fktsv.cn/Article/details/giswxkmvp.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gsabgjqel.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gidvfqmua.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gtthkoeyo.sHtML

Go:   os.Args[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gkpnzpftf.sHtML

Ruby: ARGV
来源：http://wap.epnwcf.com/Article/details/gnokfkdqc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/guhvlgmkt.sHtML

[M02] 读取环境变量
来源：http://baike.epnwcf.com/Article/details/gqbjztqkx.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.vehdjk.com/Article/details/gazrcvaoq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/gcexmqpbv.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gildoaxhf.sHtML

TS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gmiwsnhzz.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/glvvvggzi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gfbiztabq.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fktsv.cn/Article/details/gjsthxblo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/glbqtuzrb.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fktsv.cn/Article/details/gfgyjubny.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.epnwcf.com/Article/details/gqurswmzw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.epnwcf.com/Article/details/gtwntyqyw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gtceeqpym.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gpairrmfw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.vehdjk.com/Article/details/gpvgqpcob.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfmmkmdj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.tarul.cn/Article/details/gxkkdqppr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.epnwcf.com/Article/details/goszmctxr.sHtML

[M04] 获取当前工作目录
来源：http://baike.bbcook.cn/Article/details/gdjendghy.sHtML

Py:   os.getcwd()
来源：http://read.share.epnwcf.com/Article/details/gghgfqyvu.sHtML

PHP:  getcwd();
来源：http://www.blog.fktsv.cn/Article/details/gffqmzmkr.sHtML

JS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gxtmbkptq.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gokupfyef.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/gpuxcaofl.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gwbbyufat.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/gwdouuifq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.tarul.cn/Article/details/gcixgncfh.sHtML

[M05] 设置退出码
来源：http://3g.vehdjk.com/Article/details/gaailtqcm.sHtML

Py:   sys.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gcyxnpcjg.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/ggdjwlcib.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gwjerusri.sHtML

TS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gfhnrrxut.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gbmnlysnv.sHtML

Go:   os.Exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gyubbhmwj.sHtML

Ruby: exit 1
来源：http://read.share.tarul.cn/Article/details/gcfxlpfic.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.yfazqb.com/Article/details/gvyeecmzk.sHtML

[M06] 向标准错误输出
来源：http://m.share.bbcook.cn/Article/details/gbmxtiblc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gaieorgom.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.yfazqb.com/Article/details/gbkupeepz.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gcqvoymhr.sHtML

TS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/geqiksznk.sHtML

Java: System.err.println("err")
来源：http://mobile.fktsv.cn/Article/details/gzwwillpv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/gruwakrjv.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gqbuorpzw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/gvfyspqdk.sHtML

[M07] 判断是否为主入口
来源：http://wap.fktsv.cn/Article/details/gmybtvalh.sHtML


<!-- 参考信息 -->