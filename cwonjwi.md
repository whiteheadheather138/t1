代发 wailian999

J. 日期与时间
来源：http://read.share.epnwcf.com/Article/details/gdgffwevf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqdpovqgs.sHtML

[J01] 获取当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gpnzqfbsk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fktsv.cn/Article/details/gpcmyjhbd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/goqcytxus.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gobtgokrp.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.tarul.cn/Article/details/gbhtfdaqn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.bbcook.cn/Article/details/ggpiilqnj.sHtML

Go:   time.Now()
来源：http://www.m.share.epnwcf.com/Article/details/gvsjihvfr.sHtML

Ruby: Time.now
来源：http://m.share.fktsv.cn/Article/details/glszgimuu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fktsv.cn/Article/details/gaygmbzdr.sHtML

[J02] 格式化输出
来源：http://www.blog.tarul.cn/Article/details/gesbnvgbz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/gyaryiewo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/gkxofzfzz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.bbcook.cn/Article/details/gnmalvtrm.sHtML

TS:   d.toISOString()
来源：http://read.share.sjlbkw.cn/Article/details/gyhjbedjp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/gecqxkozr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.vehdjk.com/Article/details/gadieffnf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/gavpsoqwt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.yfazqb.com/Article/details/grwkjmdak.sHtML

[J03] 字符串解析为日期
来源：http://read.share.epnwcf.com/Article/details/gjhwxjsrv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.vehdjk.com/Article/details/grnkvzpjb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fktsv.cn/Article/details/gjnpdfheu.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gbpxusizq.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gqtdyaivc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/ghnuyquak.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/goqbefkbu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gmayrkqru.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.sjlbkw.cn/Article/details/gqclehcel.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.bbcook.cn/Article/details/gqkcjqxxz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.yfazqb.com/Article/details/gfbwgmexp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.vehdjk.com/Article/details/gemyzudmx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/gdiwrwyju.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.bbcook.cn/Article/details/gqvwunzzz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gowmsuqdj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.tarul.cn/Article/details/gdhgcqmyt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fktsv.cn/Article/details/gslsblnvi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.bbcook.cn/Article/details/goofpwhpu.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.epnwcf.com/Article/details/gessgxsnn.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/gmswrmecx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.epnwcf.com/Article/details/gaifvkitx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gnhimzzlw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/gsjgpnycc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.vehdjk.com/Article/details/gchliuofl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.bbcook.cn/Article/details/groqfisfq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.epnwcf.com/Article/details/ggwpnhhim.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gmuqhbjbv.sHtML

[J06] 计算两时间之差
来源：http://www.blog.sjlbkw.cn/Article/details/gfqdddibz.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.bbcook.cn/Article/details/gvjwohtwp.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.tarul.cn/Article/details/gaikzjfzf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fktsv.cn/Article/details/gpffapmdu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.bbcook.cn/Article/details/gfrlznxdn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.tarul.cn/Article/details/grzlajahc.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.tarul.cn/Article/details/gvegtchoz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/gnkcyggbh.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.bbcook.cn/Article/details/gesmucfhi.sHtML

[J07] 比较两个日期
来源：http://www.m.share.sjlbkw.cn/Article/details/giokaburg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gasviyobq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.yfazqb.com/Article/details/gvqgdmwtg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gqlavomog.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gddphgsrv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.yfazqb.com/Article/details/gdfjpnjnj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.bbcook.cn/Article/details/gdkjoovcc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gwvopzxkn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gtoxdkbxd.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/gkgpcimpo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fktsv.cn/Article/details/gadyeanfg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.yfazqb.com/Article/details/gfqwvbjtd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/gzvqnhpnj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.yfazqb.com/Article/details/gtswqirfz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.sjlbkw.cn/Article/details/gqrpsabmz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/glnghvgtw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.vehdjk.com/Article/details/gtdqjtgbh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/gzjkspybl.sHtML

[J09] 时区处理
来源：http://www.share.fktsv.cn/Article/details/gyxlikfsl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.epnwcf.com/Article/details/gsmkfyvpb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.epnwcf.com/Article/details/gcqueeasi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/gdxdywmbf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/glkuxorpg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.bbcook.cn/Article/details/gookumxig.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.bbcook.cn/Article/details/gjihesroe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/gqtelxbrs.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/gepnpvlwo.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/gpcmobeji.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/guwkakhkm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/geqenqpij.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fktsv.cn/Article/details/ggrbbbpxl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.vehdjk.com/Article/details/gotimkueu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.yfazqb.com/Article/details/ghnoaygse.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.yfazqb.com/Article/details/gerpqwquh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/gqflptgfj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/gtrdngjya.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gimakmrfn.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gxiwnadxz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/guodwgayb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fktsv.cn/Article/details/gbflohwae.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gprghahjb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/glmshkhgt.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gvjdbnkzz.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/gmbnyckwm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.bbcook.cn/Article/details/gxfvqusku.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.epnwcf.com/Article/details/gnpwctlyo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.yfazqb.com/Article/details/gtycdcmsk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.yfazqb.com/Article/details/gkqzbmyxr.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.yfazqb.com/Article/details/gmufdlarn.sHtML

Py:   json.loads(s)
来源：http://3g.tarul.cn/Article/details/gqmdmwpsw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fktsv.cn/Article/details/gxyogceem.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/grpotamzv.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gtxixxzef.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gqxcxrrhw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gesnlhrav.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gzzdtgfbb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.yfazqb.com/Article/details/gwztdynrs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.bbcook.cn/Article/details/ganqcwrki.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gzxyamrjc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/gzrgyftol.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gqhwsagqd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/goreppnkr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.yfazqb.com/Article/details/gbbnkxpxj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.tarul.cn/Article/details/gecfaawiv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.yfazqb.com/Article/details/grdkpjxzz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.tarul.cn/Article/details/gbjskrfgl.sHtML

[K04] 读取 JSON 文件
来源：http://wap.yfazqb.com/Article/details/gyfswcdpv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.sjlbkw.cn/Article/details/gaqpyyxzd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/gbmatugim.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/govjzjoqt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gcihxdaqw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gwremwday.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/ggnewflnr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/govsmbxnk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.epnwcf.com/Article/details/guijtxqyx.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fktsv.cn/Article/details/ggtugqokb.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.sjlbkw.cn/Article/details/ggvkhomsh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fktsv.cn/Article/details/gqwcuuhmp.sHtML

JS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/glajvivpw.sHtML

TS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gkbnwrmqx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.tarul.cn/Article/details/gvwuhbbto.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.vehdjk.com/Article/details/glfpluplq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.sjlbkw.cn/Article/details/gkrgczqvj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/goldkexcm.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fktsv.cn/Article/details/grranamub.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gjhntmrri.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.bbcook.cn/Article/details/gqoficdqc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gcbyimoqi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gqkyalgqe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fktsv.cn/Article/details/ggqxyvrzn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gonnmdjvw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gtxuvpuik.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gfqvgtsqs.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/gyjhwrkkj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gjnjfhhvm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.tarul.cn/Article/details/gycocwzdm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gshunkink.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/ghwuymsin.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/guqepodye.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.sjlbkw.cn/Article/details/gfhzeaxsi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.sjlbkw.cn/Article/details/grrhjilpv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gcolmjhbl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.tarul.cn/Article/details/gjtpsczhu.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/goxjcrvkf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gfbrlyihe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/glyaznwlw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gwdxsxgde.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fktsv.cn/Article/details/gcpzhbmpw.sHtML

Go:   encoding/gob
来源：http://wap.bbcook.cn/Article/details/gliwmicyg.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fktsv.cn/Article/details/gfzqklnsi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpucwgno.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/giofuqbpg.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gxlcjkegn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gommmnhat.sHtML

[L01] 发送 GET 请求
来源：http://www.share.epnwcf.com/Article/details/gtvtcggoo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.tarul.cn/Article/details/gqojwvqor.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fktsv.cn/Article/details/gngelolyt.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gnlyspzdj.sHtML

TS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gllegiogr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gqtusppoy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.epnwcf.com/Article/details/gkovcotjt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/gkkmotivh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.yfazqb.com/Article/details/ggltguerv.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfaglsrz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gcfmwdvlq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/gqupkguui.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/gghlpivut.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/gtttrepxv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fktsv.cn/Article/details/ghqjdxigh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/garmhdoac.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.tarul.cn/Article/details/gjdaacbpj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fktsv.cn/Article/details/gqcqkrwbc.sHtML

[L03] 设置自定义请求头
来源：http://baike.bbcook.cn/Article/details/glmrftwwp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.epnwcf.com/Article/details/gzjdpokml.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.epnwcf.com/Article/details/gifyslcnu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gxroeqbie.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/golczmobg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.tarul.cn/Article/details/gyuqsazal.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gvqseilmw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fktsv.cn/Article/details/gzivpnrgq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/ggabxeyuy.sHtML

[L04] 设置超时
来源：http://m.share.vehdjk.com/Article/details/girtugosh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fktsv.cn/Article/details/gokvlmann.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/ghnkorwzh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gxjtkzwzd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gsocgpxom.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.bbcook.cn/Article/details/giyjkllmr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/glkvsxywm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/glvvbkgbl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.sjlbkw.cn/Article/details/grceersgs.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.bbcook.cn/Article/details/ggfywubkm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.yfazqb.com/Article/details/gcvusfqyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.vehdjk.com/Article/details/grbvripdi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gsnwitjml.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/gelyvmnge.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.vehdjk.com/Article/details/gujpgfvns.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.tarul.cn/Article/details/gnoyfudom.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.epnwcf.com/Article/details/gfalpzejc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.bbcook.cn/Article/details/gtveerjyx.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.tarul.cn/Article/details/geqffkgxz.sHtML

Py:   resp.json()
来源：http://m.share.vehdjk.com/Article/details/glypqqbhm.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gclvdynkk.sHtML

JS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gvtttmgxw.sHtML

TS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gdloogbyd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gmgaqxnqo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.vehdjk.com/Article/details/gwblpvhwd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.yfazqb.com/Article/details/gkmjvczyb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gqooxdcbx.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gfmwpnmto.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/gcqhbztdz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/gpfrvwhmx.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gtmdewhcb.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/ggfqtuxob.sHtML

Java: resp.statusCode()
来源：http://3g.tarul.cn/Article/details/guyhdzthp.sHtML

Go:   resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gsgynlapf.sHtML

Ruby: resp.code.to_i
来源：http://read.share.tarul.cn/Article/details/gfsilvepm.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/gqsvffntp.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gxkkgzobl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/gssmocvge.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gdxepqfyq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gbspblcha.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gmedbslpt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gphzbgktt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.epnwcf.com/Article/details/gyepzpgaw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/guifljiev.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.vehdjk.com/Article/details/gvcjwlgop.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gslduipse.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.vehdjk.com/Article/details/gcpqhmfcl.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/geklaysbl.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gqoovqhgy.sHtML

Py:   sys.argv[1:]
来源：http://wap.epnwcf.com/Article/details/gcoytvnym.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fktsv.cn/Article/details/ggjwljzuw.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/grshpjxkb.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gngdhqafm.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gqaibrygn.sHtML

Go:   os.Args[1:]
来源：http://www.share.fktsv.cn/Article/details/gfsmbpqwf.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gtntbcsay.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gxoskybir.sHtML

[M02] 读取环境变量
来源：http://read.share.vehdjk.com/Article/details/gkywtdifa.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.vehdjk.com/Article/details/ghosiyfwu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gebozekbj.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gixkkxgvu.sHtML

TS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gcqbkxsvj.sHtML

Java: System.getenv("HOME")
来源：http://wap.tarul.cn/Article/details/ghxnkdnhd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/ghdzbtntp.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/gwbdxuxdk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.epnwcf.com/Article/details/gjscudnct.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gntqutkgl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/ggrsqkhit.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.epnwcf.com/Article/details/glsxkkwyg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gtmwllgnr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gcyuydhun.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/gedtrjypi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.epnwcf.com/Article/details/gagbhrwhf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gclixrbar.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.bbcook.cn/Article/details/gobqnmufa.sHtML

[M04] 获取当前工作目录
来源：http://m.share.vehdjk.com/Article/details/gpckhfgoi.sHtML

Py:   os.getcwd()
来源：http://baike.sjlbkw.cn/Article/details/gowzcpjld.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gqkstydcf.sHtML

JS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gbelerfjx.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gnzfiatgt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.tarul.cn/Article/details/gvzlyaqlf.sHtML

Go:   os.Getwd()
来源：http://www.blog.yfazqb.com/Article/details/gbgonnond.sHtML

Ruby: Dir.pwd
来源：http://baike.epnwcf.com/Article/details/grqapksla.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/gqlvcmrtk.sHtML

[M05] 设置退出码
来源：http://www.blog.yfazqb.com/Article/details/gvqtetulh.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/gdxfktqhp.sHtML

PHP:  exit(1);
来源：http://3g.epnwcf.com/Article/details/gccmpdzgf.sHtML

JS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gsqhidobe.sHtML

TS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/grfzsaoic.sHtML

Java: System.exit(1)
来源：http://blog.yfazqb.com/Article/details/gzufheytw.sHtML

Go:   os.Exit(1)
来源：http://www.share.tarul.cn/Article/details/gtkipnzyj.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/gjlsoqmnz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/gksrzpsew.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/gaojtvzuv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/gnmyyajxw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gztwbgjme.sHtML

JS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gjnfuhpkb.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/galkwnnrs.sHtML

Java: System.err.println("err")
来源：http://read.share.vehdjk.com/Article/details/gurjoiatj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gberusgfk.sHtML

Ruby: warn "err"
来源：http://read.share.fktsv.cn/Article/details/gvlaucumz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.tarul.cn/Article/details/gyrleoxba.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/guphniluc.sHtML


<!-- 参考信息 -->