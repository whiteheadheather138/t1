代发 wailian999

J. 日期与时间
来源：http://blog.yfazqb.com/Article/details/gijslucyy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gaqlkojfm.sHtML

[J01] 获取当前时间
来源：http://read.share.epnwcf.com/Article/details/glvszbhzt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.bbcook.cn/Article/details/ggprdohdm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gbfuwwqpo.sHtML

JS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gagrykjug.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gypyzaoqw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.bbcook.cn/Article/details/gyknolnuk.sHtML

Go:   time.Now()
来源：http://www.blog.fktsv.cn/Article/details/gwejbluqg.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/gqihvbcds.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.bbcook.cn/Article/details/grygjiwgl.sHtML

[J02] 格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gfhureufp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/gubnpiobo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gpdcsgegy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fktsv.cn/Article/details/gnzyiidqv.sHtML

TS:   d.toISOString()
来源：http://www.blog.sjlbkw.cn/Article/details/gkalzvigd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gvuqqmkuk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fktsv.cn/Article/details/grnbqggxz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/glevhmlcb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/gstsqrcio.sHtML

[J03] 字符串解析为日期
来源：http://blog.sjlbkw.cn/Article/details/gidqjbddy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.bbcook.cn/Article/details/ghyoifxbj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.vehdjk.com/Article/details/gxwhkjtlv.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/ggamzgufp.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gttogubzs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/glhrdtpqk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/guhhmsfbx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/goyeojlud.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/gxlxvheye.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.vehdjk.com/Article/details/gavuopnuv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/grwgpvuak.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.vehdjk.com/Article/details/gsounbdea.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/grnmmesos.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.tarul.cn/Article/details/gffsxgyyw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.tarul.cn/Article/details/gjzmxbrqh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.epnwcf.com/Article/details/gvztxfsum.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/ggsmmofdo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/gydfqjzbp.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.bbcook.cn/Article/details/gfuhaqqhh.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.sjlbkw.cn/Article/details/gtmuvwuea.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.tarul.cn/Article/details/gopwevtad.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/glaivrxko.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/guobovuni.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/gibohsewi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.vehdjk.com/Article/details/gknvaclwg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fktsv.cn/Article/details/ginivcjmc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gmzgfhbkj.sHtML

[J06] 计算两时间之差
来源：http://m.share.yfazqb.com/Article/details/gxhjayide.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.bbcook.cn/Article/details/gekuaddfa.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.sjlbkw.cn/Article/details/gpbruiqwb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.tarul.cn/Article/details/govtjdile.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.epnwcf.com/Article/details/gnjkqihti.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.yfazqb.com/Article/details/gvdsackct.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.epnwcf.com/Article/details/ghfkfgwju.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.epnwcf.com/Article/details/gxxqccpzl.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.sjlbkw.cn/Article/details/gcxdtggdl.sHtML

[J07] 比较两个日期
来源：http://www.m.share.yfazqb.com/Article/details/gxitfwhqk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gikmosyeo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.vehdjk.com/Article/details/gliwmexgb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gaiwznkxo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gntlxkkth.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.sjlbkw.cn/Article/details/ggglwupaj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.tarul.cn/Article/details/ggzsgnuxy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/ggyajkyhe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gcdwvmfmc.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gtqwksucr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fktsv.cn/Article/details/gzhxqrjyz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gmgpuawqo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.vehdjk.com/Article/details/grsddjyub.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.vehdjk.com/Article/details/gtcjqiaml.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.yfazqb.com/Article/details/gavlkazzu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.vehdjk.com/Article/details/gnlnmvdhh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.vehdjk.com/Article/details/gaxefledo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.bbcook.cn/Article/details/gzsogbhnr.sHtML

[J09] 时区处理
来源：http://www.share.vehdjk.com/Article/details/gesvlzjqb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.sjlbkw.cn/Article/details/gupnxwekk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fktsv.cn/Article/details/gxoxirxdt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gwjavzrav.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/grnhiueiu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.bbcook.cn/Article/details/grwdjkmud.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fktsv.cn/Article/details/gabfmmvfe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.epnwcf.com/Article/details/giyrwrsrd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.vehdjk.com/Article/details/giewbmdxb.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/gfokosorh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.sjlbkw.cn/Article/details/gclhxcnmo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gwtcukbce.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gggbnsnyb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.bbcook.cn/Article/details/gswqyxnsx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.tarul.cn/Article/details/gvlrxalcl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.vehdjk.com/Article/details/gcpbojock.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.vehdjk.com/Article/details/ghzmvspqh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fktsv.cn/Article/details/gljpvubjp.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ghaxxhleu.sHtML

K. JSON 与序列化
来源：http://baike.bbcook.cn/Article/details/ghuxheisy.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gkhggnyns.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.yfazqb.com/Article/details/gpyzdynjn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gcxzxyieo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gzhheyufe.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/ghnvpmxuo.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gpsgjsddf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.vehdjk.com/Article/details/gbxpsrajd.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/gioudxkrm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.epnwcf.com/Article/details/gfudkhdco.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gocrimajh.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fktsv.cn/Article/details/gxhyelcov.sHtML

Py:   json.loads(s)
来源：http://3g.tarul.cn/Article/details/gextdalrj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.tarul.cn/Article/details/goibrnvvi.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/guwdtmmwz.sHtML

TS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gtylzxwiy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gtrcslrpj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/gmppymhpb.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gpfwdlzzw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.bbcook.cn/Article/details/getrfqqza.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gcvunrelm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/gsuwrmkya.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gxyysurqd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/grfhuxncv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gdptnvuoi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.sjlbkw.cn/Article/details/glbetwoyo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gsfywbhgk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.epnwcf.com/Article/details/ghunwqcpa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.yfazqb.com/Article/details/ggisvfraa.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/grvxludfu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.vehdjk.com/Article/details/gdfugzpqn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fktsv.cn/Article/details/gyoefomzs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/gwikzljmp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gxnamcmtv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.vehdjk.com/Article/details/gtwgvrhoa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/gtmqvwzut.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.epnwcf.com/Article/details/gmlefqvcl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.vehdjk.com/Article/details/gazvbbtyu.sHtML

[K05] 深拷贝对象
来源：http://baike.vehdjk.com/Article/details/gvkmyuqnf.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.yfazqb.com/Article/details/gxsrbubee.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/gwobqockp.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gcgkmjssc.sHtML

TS:   structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/gnhffilhg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/grhjepcah.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fktsv.cn/Article/details/gfqfaudoq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fktsv.cn/Article/details/gdfnjcfpz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/gbpgeiqkr.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/gguhdtbbo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gxjuutngf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/ghyerkdmt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gjvgybywx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gjkuciarx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/gumwjljas.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gcjnuiqqv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gjtyiuomf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/ggmhutjvp.sHtML

[K07] 进制转换
来源：http://m.share.fktsv.cn/Article/details/gcttnjevw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gtgugxuwz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/gmaxlzerb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gkkngehcp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gyzzdlsxx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gwwtobdds.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fktsv.cn/Article/details/gyfvixymk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.yfazqb.com/Article/details/gsakxtejw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gbgtchcxl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.yfazqb.com/Article/details/gqdtwizqw.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/gbstsvvar.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.vehdjk.com/Article/details/gnzeoxcpo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/ggncnrqku.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gsorqsvwe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/gmxbhklef.sHtML

Go:   encoding/gob
来源：http://mobile.sjlbkw.cn/Article/details/gpwxgpfql.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.bbcook.cn/Article/details/gpdnpfujv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gixeimzol.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqjozprvw.sHtML

L. 网络请求
来源：http://www.m.share.tarul.cn/Article/details/gkeuhemib.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gdfmetesm.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gualrtctv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gsjulzuvf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.vehdjk.com/Article/details/ghvhusbaj.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gjptdphrb.sHtML

TS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gwckkbccw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.yfazqb.com/Article/details/gcefhetaf.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/grwbkpqkg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/gkkzmzyjt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.sjlbkw.cn/Article/details/guaxjoehx.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gvydfyhvr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gopwqpqyw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fktsv.cn/Article/details/gefkmlwyd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gkvhhzksj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gmpzzisjr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/gowddrrwn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.vehdjk.com/Article/details/gukcdronn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/gepdighdl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/ggaaqxwfe.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/gdutvuvbg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.epnwcf.com/Article/details/gtrvisltw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.vehdjk.com/Article/details/gjghwsqte.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gomqregqw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gpaokuuax.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.tarul.cn/Article/details/gzmmgoosq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gxwkcczxs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.tarul.cn/Article/details/gnxrwxvou.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gykicebrq.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/gectrdnyw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.sjlbkw.cn/Article/details/gztkxjwbh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.yfazqb.com/Article/details/glapatcns.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gazclzfwd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/geupsokwg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gfkusazge.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gtxdhrwmq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.epnwcf.com/Article/details/gpuzsgmxt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.tarul.cn/Article/details/gxlleqhbx.sHtML

[L05] 上传文件（multipart）
来源：http://blog.bbcook.cn/Article/details/guokgurgt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gmrkxuxga.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/gjgoedmfu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gkelasbis.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gijjjbgkz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.vehdjk.com/Article/details/gwksqomfu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/gnjtzbcpb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.tarul.cn/Article/details/gdiiduhdg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.vehdjk.com/Article/details/gpbicalwr.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.bbcook.cn/Article/details/gxgkkbppr.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/gmquzrkyo.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gtbvyhscc.sHtML

JS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/goxhzgjbo.sHtML

TS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gdslgbfdw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.tarul.cn/Article/details/gemvdouwn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/gzoravpwq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/gbsulngtk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.bbcook.cn/Article/details/ggmjghrtf.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gfuvkpizz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fktsv.cn/Article/details/gmthsarzy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnegydym.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gtgriptpj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/goabfkson.sHtML

Java: resp.statusCode()
来源：http://m.share.fktsv.cn/Article/details/gxlwztqyv.sHtML

Go:   resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/ghzfaapqk.sHtML

Ruby: resp.code.to_i
来源：http://3g.sjlbkw.cn/Article/details/gihkhjvai.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gncwcoxux.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.bbcook.cn/Article/details/gwnivoiep.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.vehdjk.com/Article/details/ghzzxomsu.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.epnwcf.com/Article/details/gqnilebij.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gaxgwytff.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/ganprhemt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.bbcook.cn/Article/details/ghmncxfyx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.yfazqb.com/Article/details/gqjokmuqi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/glnznmmvx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.tarul.cn/Article/details/gysgevpet.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfatfveis.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gvonrrszm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjryyjmnr.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.tarul.cn/Article/details/grzzkdryw.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/gsoxhivuh.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.vehdjk.com/Article/details/gmnumvxxf.sHtML

JS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gskvgibia.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gbklrvusm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gkgwhcttf.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fktsv.cn/Article/details/ghmcjogej.sHtML

Ruby: ARGV
来源：http://blog.epnwcf.com/Article/details/ggeesrtjo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.tarul.cn/Article/details/gwefhzrgw.sHtML

[M02] 读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gwoemflbe.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.bbcook.cn/Article/details/gvngmiqtc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gyroerkdo.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gzshxsrtx.sHtML

TS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gfjbqisfe.sHtML

Java: System.getenv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gjhieuugq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.yfazqb.com/Article/details/gxcjsihrk.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.bbcook.cn/Article/details/grqzirqmp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.epnwcf.com/Article/details/gqbqnlukk.sHtML

[M03] 执行外部命令
来源：http://mobile.vehdjk.com/Article/details/gggdggxye.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.yfazqb.com/Article/details/gfwsktgiv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fktsv.cn/Article/details/gxpupacpa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gnsblzlyb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gcphnhqln.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.epnwcf.com/Article/details/geekehkyq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.sjlbkw.cn/Article/details/gtupvntep.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.epnwcf.com/Article/details/gifzceqgy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/gomgjmvon.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/gejvqutii.sHtML

Py:   os.getcwd()
来源：http://blog.fktsv.cn/Article/details/gbqdglgyr.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gldmibvww.sHtML

JS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/ghttvqeyc.sHtML

TS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/glvgiqwwv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.yfazqb.com/Article/details/giletvicd.sHtML

Go:   os.Getwd()
来源：http://read.share.yfazqb.com/Article/details/ghgvfigdu.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/ghjwdwwtp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gppaobbor.sHtML

[M05] 设置退出码
来源：http://3g.vehdjk.com/Article/details/gzfxxqaqe.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gjndjouyw.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gicbtysba.sHtML

JS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gpiwtptqw.sHtML

TS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gkiqdlstk.sHtML

Java: System.exit(1)
来源：http://baike.epnwcf.com/Article/details/gnulxeaou.sHtML

Go:   os.Exit(1)
来源：http://read.share.bbcook.cn/Article/details/gcsyhndtp.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/gdpkrallp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.tarul.cn/Article/details/gfmjfwjln.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/gtabqvjzo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gcgkrtvch.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/gbvakgonk.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gtvejaxhp.sHtML

TS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gzpjillvo.sHtML

Java: System.err.println("err")
来源：http://mobile.tarul.cn/Article/details/gktsgwwrt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/gzlguqnll.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gntlfiuzb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.bbcook.cn/Article/details/ghhzzgpse.sHtML

[M07] 判断是否为主入口
来源：http://read.share.bbcook.cn/Article/details/goxxhxysa.sHtML


<!-- 参考信息 -->