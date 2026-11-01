代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.vehdjk.com/Article/details/gvfiboodh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gwvgfkwhw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gejmzktle.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/gtlnhxoub.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/gefyegdtz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.epnwcf.com/Article/details/gvdkgafwn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gxahldxwd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/guagecnms.sHtML

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/grwtfuvkh.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxdljoubh.sHtML

[J01] 获取当前时间
来源：http://read.share.bbcook.cn/Article/details/gqhddgsqc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.bbcook.cn/Article/details/gydikrkri.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gextrbpgr.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/ggawykrsy.sHtML

TS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gyyrmaaqm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fktsv.cn/Article/details/ghwxxblnr.sHtML

Go:   time.Now()
来源：http://mobile.vehdjk.com/Article/details/gppvzqbig.sHtML

Ruby: Time.now
来源：http://www.m.share.yfazqb.com/Article/details/gijladeqb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.epnwcf.com/Article/details/gxruieiwo.sHtML

[J02] 格式化输出
来源：http://3g.vehdjk.com/Article/details/gdlngybgs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/guyjebqvx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gonnnjvbs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fktsv.cn/Article/details/ghvvysffw.sHtML

TS:   d.toISOString()
来源：http://blog.bbcook.cn/Article/details/geqdgfedq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fktsv.cn/Article/details/gbushebht.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.tarul.cn/Article/details/geglsbyxa.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/gwgkoddpg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fktsv.cn/Article/details/gqavkhxmd.sHtML

[J03] 字符串解析为日期
来源：http://blog.tarul.cn/Article/details/gklrcgxqq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.bbcook.cn/Article/details/gdwjxhoqj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fktsv.cn/Article/details/grewozuka.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gpuwvdzmq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gzbufqrgo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gdepadhln.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gpnpkqxrw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gqtsopeoi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.vehdjk.com/Article/details/gqciyvpxe.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gogagfiht.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.vehdjk.com/Article/details/guaprydbt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.tarul.cn/Article/details/gxyjhgxtz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.vehdjk.com/Article/details/gwalicybv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.bbcook.cn/Article/details/giaofbxhg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcatfuwi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gdxpfbhfi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gjnsanpta.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.yfazqb.com/Article/details/garnshjsl.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/grmgaqgxa.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.bbcook.cn/Article/details/gioxoxpiu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.yfazqb.com/Article/details/gqwxsptlo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/gsdkkaoow.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/glxmvoptt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.epnwcf.com/Article/details/gykgbrepq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.tarul.cn/Article/details/gyszsacfy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.epnwcf.com/Article/details/guaksrkgl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/glqmtlajz.sHtML

[J06] 计算两时间之差
来源：http://baike.epnwcf.com/Article/details/gyiunogbo.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fktsv.cn/Article/details/getwumhws.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.epnwcf.com/Article/details/gsyzujpio.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.tarul.cn/Article/details/gvefjijue.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.vehdjk.com/Article/details/gzbqpelgv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.tarul.cn/Article/details/gclvmnaft.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fktsv.cn/Article/details/grnmjebfn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.epnwcf.com/Article/details/gowglslew.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.vehdjk.com/Article/details/giygrhbnd.sHtML

[J07] 比较两个日期
来源：http://baike.fktsv.cn/Article/details/gqorqcjot.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gfyzbtomm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fktsv.cn/Article/details/gcnfphuxu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/grpkptmdt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gqgeivhdp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gwotsrifp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.sjlbkw.cn/Article/details/gjrotrgwe.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gjmgmcrhg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gdvhccjcx.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gjgqvrufx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.bbcook.cn/Article/details/ghvosruyn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.bbcook.cn/Article/details/gzfxqrhjq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.epnwcf.com/Article/details/gipehyjsq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.bbcook.cn/Article/details/gpwvequwr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/gultsyeiz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.sjlbkw.cn/Article/details/gcktvysju.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fktsv.cn/Article/details/gdnfkogmp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdbvwkfy.sHtML

[J09] 时区处理
来源：http://baike.epnwcf.com/Article/details/gkupnulod.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.epnwcf.com/Article/details/ghhtfufpk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.tarul.cn/Article/details/gffqcdydg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gmhaqpumz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gvkevnebd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.sjlbkw.cn/Article/details/gagemhdzg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.vehdjk.com/Article/details/gkuxivwqt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbwibvcr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fktsv.cn/Article/details/gtnrmejpw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.bbcook.cn/Article/details/goktdiyju.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.yfazqb.com/Article/details/gcqvkeeyk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/gzcgbajky.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/gkdirhbjf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.yfazqb.com/Article/details/ghqgotvsr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.vehdjk.com/Article/details/gzyfzxrdk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/grasazccu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.yfazqb.com/Article/details/gzkubrqbh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/gcvabblva.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gizrcxbwf.sHtML

K. JSON 与序列化
来源：http://baike.sjlbkw.cn/Article/details/gpcproawq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmzdgraqs.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fktsv.cn/Article/details/gygaqeqrm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/grdgvlhwp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/grukfwrjt.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmasnuoh.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gmxeojonn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/giaccjyow.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fktsv.cn/Article/details/ghasslqdi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/gdtegqosd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.sjlbkw.cn/Article/details/grexzdlzc.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fktsv.cn/Article/details/gnrmifibi.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/glgsehwsv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.sjlbkw.cn/Article/details/gzjlznvbn.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gledppkmv.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gnqfvwere.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gwkslkqeu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gchxjvyvz.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gxcspbjxj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.vehdjk.com/Article/details/gkdaxlgti.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.vehdjk.com/Article/details/gvlfwdesz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/glbvyqldz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gnfnakuro.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gxgfhyagg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gtxbzjqsn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.vehdjk.com/Article/details/glnmbpylj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/gwyirganp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gnihflmrn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.bbcook.cn/Article/details/gavfjjdzc.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/gzxqmpqob.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.yfazqb.com/Article/details/gvpyduxrm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fktsv.cn/Article/details/gwcimetnt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gbuzprdwr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gzaktegpa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gpqcvelvc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gbhowinpk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gpvashunq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gbyqbcxop.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.epnwcf.com/Article/details/gjfyfntlr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/gakpxpbuf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.vehdjk.com/Article/details/gsclspnbj.sHtML

JS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/giwiklphc.sHtML

TS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gserqouru.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.sjlbkw.cn/Article/details/gryqbtmpp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gynehjkhq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.yfazqb.com/Article/details/glnkqemga.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.tarul.cn/Article/details/giyluqqra.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/gntreqsmg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.bbcook.cn/Article/details/gzespjava.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.epnwcf.com/Article/details/gedhhjhzv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gpttheqpq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gkenvnojv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.yfazqb.com/Article/details/gdkgzdpfi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gxseufmao.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gkifuvvzf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gckftrpmk.sHtML

[K07] 进制转换
来源：http://www.m.share.epnwcf.com/Article/details/gfcklkztl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gncpdeeok.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.bbcook.cn/Article/details/gdcswrvsf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gclydmnoa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gyepkemyn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gempjqkpi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/guneknbam.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.vehdjk.com/Article/details/gdxlvtekp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gixgjosda.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.tarul.cn/Article/details/guchlsroa.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.bbcook.cn/Article/details/gmmvsvhoe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.vehdjk.com/Article/details/gkticzhsc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gpvsubjng.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/gydfceoom.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.tarul.cn/Article/details/gsbfnlixk.sHtML

Go:   encoding/gob
来源：http://blog.bbcook.cn/Article/details/gdfpkagvp.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.bbcook.cn/Article/details/gqwxywsvg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gnnigemle.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gauqhgvfp.sHtML

L. 网络请求
来源：http://read.share.epnwcf.com/Article/details/gifqmkprp.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggbdyeatn.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.yfazqb.com/Article/details/grtcrhorj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.yfazqb.com/Article/details/goiojctfj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.bbcook.cn/Article/details/gtupjwuvv.sHtML

JS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gyuxaiaau.sHtML

TS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gwtymfdqj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fktsv.cn/Article/details/gaimabirw.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gumorrqqf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fktsv.cn/Article/details/gltpitjgl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/ghjozgibm.sHtML

[L02] 发送 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gqilurrnr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gtuszdhdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.sjlbkw.cn/Article/details/gjesbrhsa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/ghonbzcel.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gvztnabqx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.tarul.cn/Article/details/gpdjlwgyr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/gdlguvtkd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.bbcook.cn/Article/details/gqhucrgxv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.sjlbkw.cn/Article/details/ghwvsyvhk.sHtML

[L03] 设置自定义请求头
来源：http://m.share.yfazqb.com/Article/details/gxovustao.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.epnwcf.com/Article/details/ghfzikfoj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.bbcook.cn/Article/details/gvoqxifyc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gctxumdtb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gbqahcppa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.tarul.cn/Article/details/grueckvxs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gbtazbxib.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.epnwcf.com/Article/details/gwqddoziz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/guhgwczuo.sHtML

[L04] 设置超时
来源：http://blog.bbcook.cn/Article/details/gbxxukzda.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gpthemuzt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gvvhvvsty.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gtsbvsufa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/glydvaaus.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/gypizfuvp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.yfazqb.com/Article/details/gapgcxspe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gkcobaimw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.tarul.cn/Article/details/gewdiyusd.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjladaohz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.sjlbkw.cn/Article/details/gmqzltsgs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gbdtiqtfv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/glgdeiojs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gtoxbbkbc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.epnwcf.com/Article/details/gqkadmhbf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.epnwcf.com/Article/details/gvegtqctp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gipfqiook.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gfsglpsre.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/giearopte.sHtML

Py:   resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gjlparjbk.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.tarul.cn/Article/details/gkyrguleu.sHtML

JS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/ggdbyqlsb.sHtML

TS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/ghfaflyxk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/ghpdrlsst.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.bbcook.cn/Article/details/grspxxsjj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.vehdjk.com/Article/details/gsgedohan.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gbydfvevg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gfxqeebtu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/gghzqslyy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.vehdjk.com/Article/details/gulgjlqlw.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gffetyocr.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gqwsqlmey.sHtML

Java: resp.statusCode()
来源：http://3g.sjlbkw.cn/Article/details/gltkjwerk.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gguwmotob.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gaykliqsp.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gglhhdpbw.sHtML

[L08] 并发请求多个地址
来源：http://wap.fktsv.cn/Article/details/gnyjkmtpk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.yfazqb.com/Article/details/gtgfzgwev.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.yfazqb.com/Article/details/ggvgvhnal.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gdrabjydm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gsaxjromq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fktsv.cn/Article/details/gucnhghua.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.epnwcf.com/Article/details/gnhailrlo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.bbcook.cn/Article/details/gdnipodoj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gydmvalez.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/geuovyffa.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.sjlbkw.cn/Article/details/gewzzossg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gngcmylmw.sHtML

[M01] 读取命令行参数
来源：http://www.blog.tarul.cn/Article/details/gdgrrphxs.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/gwkaovspm.sHtML

PHP:  $argv;  $argc;
来源：http://3g.epnwcf.com/Article/details/gexmnumpk.sHtML

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gsmkabzei.sHtML

TS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gdyvvktsp.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gqaadmwji.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/gnpjqsvdi.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gigcmxcve.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gknupfyiy.sHtML

[M02] 读取环境变量
来源：http://baike.bbcook.cn/Article/details/gihwpnvpm.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.tarul.cn/Article/details/gvomlbcfj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gpdtevsjj.sHtML

JS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gxezdosdt.sHtML

TS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gajyjiwxq.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/grnumvzea.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gdsdmecom.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.bbcook.cn/Article/details/geoqutbuz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gitifohzb.sHtML

[M03] 执行外部命令
来源：http://m.share.tarul.cn/Article/details/gzodagmpd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/gcaiihazy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/gyqgjildb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gkhrtodsl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/ghfrwqefp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.epnwcf.com/Article/details/gnobewdpn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gynmnblic.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.bbcook.cn/Article/details/gbvldhtbg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.epnwcf.com/Article/details/gieumwmyz.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gwruymoek.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/grwpuhnqh.sHtML

PHP:  getcwd();
来源：http://www.share.sjlbkw.cn/Article/details/gigohupkw.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gbxyehvcn.sHtML

TS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/grazrgdzj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/gixszgike.sHtML

Go:   os.Getwd()
来源：http://read.share.vehdjk.com/Article/details/grdzbyucd.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/grbqkikos.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.epnwcf.com/Article/details/gyfroxdxq.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/gtjvrzqka.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/gjjdwefii.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gdkfokeuk.sHtML

JS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gcyetsujf.sHtML

TS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gyyobeztc.sHtML

Java: System.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gigfywyaq.sHtML

Go:   os.Exit(1)
来源：http://mobile.bbcook.cn/Article/details/gehfrwxot.sHtML

Ruby: exit 1
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhtzjkdj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/gejkxkcxs.sHtML

[M06] 向标准错误输出
来源：http://3g.bbcook.cn/Article/details/gdddocbmo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gkqcvmzxt.sHtML


<!-- 参考信息 -->