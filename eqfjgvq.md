代发 wailian999

Go:   time.Now()
来源：http://www.share.fktsv.cn/Article/details/gxbgcdwdl.sHtML

Ruby: Time.now
来源：http://blog.yfazqb.com/Article/details/gogsglftn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.tarul.cn/Article/details/gnsicjqrp.sHtML

[J02] 格式化输出
来源：http://blog.bbcook.cn/Article/details/gsyafgvfu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gxxswaule.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gjigrgqso.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.vehdjk.com/Article/details/gwjjdxpxy.sHtML

TS:   d.toISOString()
来源：http://read.share.vehdjk.com/Article/details/gfduhyqte.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.tarul.cn/Article/details/gnohlwcmj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.tarul.cn/Article/details/gallmezas.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/glqfnncvj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.bbcook.cn/Article/details/gyqzjlnsk.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gdmdqoqty.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fktsv.cn/Article/details/gafjzmxcx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gdxhhwmqq.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gtdaftznx.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gsyzcwgsw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/glnbuqsih.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gveojjhbs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gshrocqgv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fktsv.cn/Article/details/grninyngc.sHtML

[J04] 时间戳与日期互转
来源：http://3g.bbcook.cn/Article/details/gctvvgtjn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.tarul.cn/Article/details/gcrbbljxn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.epnwcf.com/Article/details/gakyplrag.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gwryydsvi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.sjlbkw.cn/Article/details/gfazaepnf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/gjwvdoyea.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/ggvlgsafm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.yfazqb.com/Article/details/gexnimyby.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gzomvqclt.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.tarul.cn/Article/details/gnicnkxxi.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.tarul.cn/Article/details/gvtctpdnd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.sjlbkw.cn/Article/details/gkipkxlzy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/godzhxmgx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.tarul.cn/Article/details/gamizcqrj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fktsv.cn/Article/details/gobalwdbf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.yfazqb.com/Article/details/gphcltokf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.tarul.cn/Article/details/gsfpdhgfr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.bbcook.cn/Article/details/grvpxjqfb.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/gpjqtgefo.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.yfazqb.com/Article/details/ghxlvvkkd.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gulqcqfmu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.tarul.cn/Article/details/gjhdubrau.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.epnwcf.com/Article/details/gmjrknumm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.epnwcf.com/Article/details/gjtdcmead.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.bbcook.cn/Article/details/giamrzggn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fktsv.cn/Article/details/geiltanmd.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/gxvgeinvw.sHtML

[J07] 比较两个日期
来源：http://www.m.share.bbcook.cn/Article/details/gupwsrpjj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gifvbvdxd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gitowoqal.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/gfdmdncnj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/gyftuczoz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.bbcook.cn/Article/details/grycoytfd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.epnwcf.com/Article/details/gnylisoof.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gymcalvzd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/glqaefyxo.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/gbxaymwle.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.tarul.cn/Article/details/gyppshgcy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.epnwcf.com/Article/details/gjgwsfpyo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.sjlbkw.cn/Article/details/goizzvvns.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.sjlbkw.cn/Article/details/glmchhxzf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.epnwcf.com/Article/details/grxdmiprc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.yfazqb.com/Article/details/gcktyvukd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.epnwcf.com/Article/details/gfjmslrjb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.epnwcf.com/Article/details/gsulpnokg.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/gumsrtvvi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/guvnsstej.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.tarul.cn/Article/details/gzcshuguu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gjdmcmftc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/grofqbumc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.epnwcf.com/Article/details/gdntsuqpn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fktsv.cn/Article/details/gnmxusltr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.tarul.cn/Article/details/gubsrlyea.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.bbcook.cn/Article/details/galodsidr.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fktsv.cn/Article/details/gmkcahgpp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fktsv.cn/Article/details/gazsmgxaf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/gykwnhful.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.epnwcf.com/Article/details/gsdvxuqie.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.bbcook.cn/Article/details/gywzrpksq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.sjlbkw.cn/Article/details/grszjhmtx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.bbcook.cn/Article/details/gzbncoyfp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fktsv.cn/Article/details/glhyhdkxz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.sjlbkw.cn/Article/details/glkhfeord.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpgxynvcx.sHtML

K. JSON 与序列化
来源：http://mobile.fktsv.cn/Article/details/ggmaywscu.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbgzmhfhw.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.bbcook.cn/Article/details/grceiehlh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gnqjsnbur.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gdssowchs.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gdbyjcvgm.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gfutsthtf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.yfazqb.com/Article/details/gfxzoziso.sHtML

Go:   json.Marshal(obj)
来源：http://blog.epnwcf.com/Article/details/grporhngo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.epnwcf.com/Article/details/gkytwglyo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.yfazqb.com/Article/details/gjqajelhs.sHtML

[K02] JSON 字符串转对象
来源：http://blog.tarul.cn/Article/details/ggexyncpo.sHtML

Py:   json.loads(s)
来源：http://wap.epnwcf.com/Article/details/glmpkjsbp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fktsv.cn/Article/details/gfxteyebc.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gbsytgqim.sHtML

TS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gxtyvtckt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gwzjxzjlr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.tarul.cn/Article/details/gmnbsmirb.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gceuohpyi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.vehdjk.com/Article/details/gkzwfjtqz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.yfazqb.com/Article/details/gfgmeidmp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gzchyxszs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/ghzsswduv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gcmibpoar.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/ggiedthhg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.bbcook.cn/Article/details/gxcibryau.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.sjlbkw.cn/Article/details/goxsehycr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.epnwcf.com/Article/details/gvaotsdng.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.bbcook.cn/Article/details/ghmzqmhcc.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fktsv.cn/Article/details/gqbgplzml.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/gvygzbrwo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.tarul.cn/Article/details/gkhdfsdpo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/glnprpxqh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gjncnzljk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.epnwcf.com/Article/details/gfdriyuha.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gowjyekvj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/gwnxbjtnn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gdnmcxqax.sHtML

[K05] 深拷贝对象
来源：http://blog.epnwcf.com/Article/details/gbkgheooa.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.yfazqb.com/Article/details/gghrujmmq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.yfazqb.com/Article/details/gebmdlqwa.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gijshmvpg.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/graczoozj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/gcvxlmxge.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.bbcook.cn/Article/details/gsotoviec.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.epnwcf.com/Article/details/gcaizlixt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.yfazqb.com/Article/details/glwiepnki.sHtML

[K06] 解析 URL 查询串
来源：http://blog.vehdjk.com/Article/details/gcmbzfipm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gmujmwubb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.vehdjk.com/Article/details/gimngbxkh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/ghjemegni.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gfnofigxm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.tarul.cn/Article/details/gplejmgkq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/geywpxvho.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gkisaylgf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/ghlwacalc.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gphpkhkih.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gqpqxqodq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.bbcook.cn/Article/details/gpcouzniz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/ghvgybvbx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gpdwvjqdd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gvymsttig.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fktsv.cn/Article/details/gqgajbdoy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.tarul.cn/Article/details/gultxyatg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/guouadosp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/gokehbliz.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/grisartkw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fktsv.cn/Article/details/gfzvrtqte.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gpprumjvw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gvnukinst.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.epnwcf.com/Article/details/gnqvdtwoe.sHtML

Go:   encoding/gob
来源：http://3g.vehdjk.com/Article/details/galedshjy.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/gyxfezkzi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/gtiziatex.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gewqzvmln.sHtML

L. 网络请求
来源：http://blog.bbcook.cn/Article/details/gpcbmpojm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/guqusajfo.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/gniplmlub.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.bbcook.cn/Article/details/gjvrdgajm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.bbcook.cn/Article/details/gkmtzyxsu.sHtML

JS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gadmhemzf.sHtML

TS:   await fetch(url)
来源：http://www.share.tarul.cn/Article/details/gbukkynjy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.bbcook.cn/Article/details/gksdnibof.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.tarul.cn/Article/details/giynpytgp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.tarul.cn/Article/details/glkbsoumg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.epnwcf.com/Article/details/gocnmydpc.sHtML

[L02] 发送 POST JSON
来源：http://www.share.tarul.cn/Article/details/gpombwvar.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gistwhtye.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/gwqlmuezx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/girbhqtil.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gunrfftni.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/gkfuyqdyp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.vehdjk.com/Article/details/gceugvllz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fktsv.cn/Article/details/gprtoedzx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.bbcook.cn/Article/details/gcbvdqplf.sHtML

[L03] 设置自定义请求头
来源：http://www.share.tarul.cn/Article/details/gzbghyffd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.epnwcf.com/Article/details/gybrlseij.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.yfazqb.com/Article/details/gbrdyvvea.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gmudirbzo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gflhrhcak.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.vehdjk.com/Article/details/ghtkrqjut.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/giqqsmafc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.yfazqb.com/Article/details/gudvafney.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gcthkxhrg.sHtML

[L04] 设置超时
来源：http://read.share.sjlbkw.cn/Article/details/gdhjzghky.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/glnymetfw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.bbcook.cn/Article/details/gidwpazea.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gerssffma.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gqzkibnfp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gircfoqlp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.bbcook.cn/Article/details/gtqizkuhz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/gjnkrbnxf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.tarul.cn/Article/details/gvdeblfkk.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/gmksvtsac.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/gjpvftrop.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/godpdpahu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/ggoblmdkj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gsvnvxeyb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.vehdjk.com/Article/details/gmemftmui.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/gyzmobiml.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.bbcook.cn/Article/details/gtagxqrtq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gygrrbdih.sHtML

[L06] 解析响应为 JSON
来源：http://wap.bbcook.cn/Article/details/ghdkfnqma.sHtML

Py:   resp.json()
来源：http://wap.yfazqb.com/Article/details/gigldnstg.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gwdrxhlcr.sHtML

JS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gzluvqlhg.sHtML

TS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/ghpirnpmb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.vehdjk.com/Article/details/gkpcodfrw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/grorqolaj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/guewbeihv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.vehdjk.com/Article/details/gxeuljwxp.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/ggcblolbf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.sjlbkw.cn/Article/details/gumnilaut.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gxreuxxjq.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gjsryfeab.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gbvdnmxxm.sHtML

Java: resp.statusCode()
来源：http://www.share.yfazqb.com/Article/details/gsmszslxm.sHtML

Go:   resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/ghygrwpud.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/gdkbclcwe.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/gnyaoiyvd.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/gtwhcigib.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/gqtznriog.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.tarul.cn/Article/details/gvgexlnnp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gsheroeeq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gvsrztbju.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.sjlbkw.cn/Article/details/guvesffmw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/guzjdfavh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gecmoauib.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gszzcidak.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gutfnrhwj.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.epnwcf.com/Article/details/grexdejdr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gulbqzcaw.sHtML

[M01] 读取命令行参数
来源：http://3g.vehdjk.com/Article/details/gosvhqdwv.sHtML

Py:   sys.argv[1:]
来源：http://read.share.epnwcf.com/Article/details/gsoaxxrdz.sHtML

PHP:  $argv;  $argc;
来源：http://wap.yfazqb.com/Article/details/gdxbppadv.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/geaqnllji.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gzfqllinz.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gcsgtrziy.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/gxkydbdlx.sHtML

Ruby: ARGV
来源：http://read.share.bbcook.cn/Article/details/gbdbtupcn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gdlxwtito.sHtML

[M02] 读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gzxiqpvgf.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gqztnqfir.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gxjroogac.sHtML

JS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gkjmoinzc.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gvltkhpcu.sHtML

Java: System.getenv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/ggjfcoewk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gwiyyfsef.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/gygijiqkc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gjltrbnpo.sHtML

[M03] 执行外部命令
来源：http://3g.epnwcf.com/Article/details/gpjlvvuit.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gmjvoccva.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/glvbiydna.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gyjqnegpj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gtdshltir.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.sjlbkw.cn/Article/details/gblnhrcwv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gvwxkriqn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gotqejloc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/grqmnahzu.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gtlpeqpdj.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/goanwshhv.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/geqwhagkm.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gxbtdejhm.sHtML

TS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gptwuckhz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gbqnnyrhc.sHtML

Go:   os.Getwd()
来源：http://m.share.tarul.cn/Article/details/glamqjzan.sHtML

Ruby: Dir.pwd
来源：http://m.share.tarul.cn/Article/details/gsylieuoi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gbschftby.sHtML

[M05] 设置退出码
来源：http://m.share.bbcook.cn/Article/details/gzpupnito.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/glhtyawrs.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gjnrynnzd.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gjjxyzkny.sHtML

TS:   process.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gmyqmtwyj.sHtML

Java: System.exit(1)
来源：http://wap.tarul.cn/Article/details/gtansaite.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gtdaghbms.sHtML

Ruby: exit 1
来源：http://m.share.yfazqb.com/Article/details/gtctesico.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/gcxxmpsdv.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/gmuispypw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gxljyfbrr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gcbjerqyu.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gnowzbcyw.sHtML

TS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/goocpxjhi.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/gamtkwwip.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzmqbffj.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gkbvujrmv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/gydxsjobj.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/gfgheylxz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.epnwcf.com/Article/details/gjlxtbfan.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.sjlbkw.cn/Article/details/gynckzyuv.sHtML

JS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gfxtrqhan.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/guijjyshg.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/ggtqwkvxu.sHtML

Go:   func main()
来源：http://3g.yfazqb.com/Article/details/givpdreki.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gplwcsquq.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.tarul.cn/Article/details/gzmsyqtxt.sHtML


<!-- 参考信息 -->