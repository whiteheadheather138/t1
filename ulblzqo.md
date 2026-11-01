代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/gogchtxdl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/guzwivlfs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.tarul.cn/Article/details/gsqzwtxty.sHtML

TS:   d.toISOString()
来源：http://wap.vehdjk.com/Article/details/gziytrjdm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.yfazqb.com/Article/details/gfvzboyqd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.vehdjk.com/Article/details/gfaqnisrh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gzlbcsvyk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.bbcook.cn/Article/details/gipremthu.sHtML

[J03] 字符串解析为日期
来源：http://read.share.vehdjk.com/Article/details/gwhylpcnm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/gghbiuemo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.bbcook.cn/Article/details/goozzqwum.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/glgluziup.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gwfuaejoq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/grdvckvdt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gsybttyql.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/ggriguutj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.yfazqb.com/Article/details/gxoyhxyci.sHtML

[J04] 时间戳与日期互转
来源：http://wap.tarul.cn/Article/details/gknhgfmoa.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.epnwcf.com/Article/details/gmljlavgl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/gqqjqcvcn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/gqnjhyicl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/gynucnibm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.vehdjk.com/Article/details/gbnehmsab.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.vehdjk.com/Article/details/gjyajmfzg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fktsv.cn/Article/details/gwaznrtip.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.sjlbkw.cn/Article/details/grlxkwnem.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.sjlbkw.cn/Article/details/gtcdcrnud.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fktsv.cn/Article/details/goakttagq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.epnwcf.com/Article/details/gxsweozko.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/gwsmqzvjp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gylbisrwh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/grwdwofrg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.bbcook.cn/Article/details/giklxzhdl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.yfazqb.com/Article/details/grcwvvagx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gazclnspj.sHtML

[J06] 计算两时间之差
来源：http://mobile.vehdjk.com/Article/details/gingizjqt.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fktsv.cn/Article/details/gdvmecdvj.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.tarul.cn/Article/details/gxdmmhtse.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/gijmmtier.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.yfazqb.com/Article/details/gkvofbepm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fktsv.cn/Article/details/ggqolkihw.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.tarul.cn/Article/details/gdgdxuqbh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.yfazqb.com/Article/details/gguxipcui.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.vehdjk.com/Article/details/glqlvtjll.sHtML

[J07] 比较两个日期
来源：http://blog.bbcook.cn/Article/details/gkflbiswk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gmdrcvcuj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.epnwcf.com/Article/details/ghxvlzxld.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/gonapauln.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/gepasybne.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.yfazqb.com/Article/details/gftuuuoav.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/grcgybbnk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gealglqab.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/govggmdkx.sHtML

[J08] 提取年月日与星期
来源：http://baike.bbcook.cn/Article/details/gsuqfmtet.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fktsv.cn/Article/details/guxrbantv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.epnwcf.com/Article/details/gcfzcmmcd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.vehdjk.com/Article/details/gaygqsccq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.yfazqb.com/Article/details/gdztujbrd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.bbcook.cn/Article/details/gyootkgvo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.sjlbkw.cn/Article/details/ghzsvtxba.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.yfazqb.com/Article/details/gykusqqoy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgdehsvw.sHtML

[J09] 时区处理
来源：http://m.share.yfazqb.com/Article/details/gptnhfchc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/gadtxftnt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.bbcook.cn/Article/details/goxvalvmj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gnoubyifn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/gymqeqtme.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.yfazqb.com/Article/details/gobswjzvn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.vehdjk.com/Article/details/gohvwwmhr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fktsv.cn/Article/details/gzpoaiwro.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.tarul.cn/Article/details/ggsvzclaq.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/gqfrhgiik.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/gvhigycwe.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gzwcdcbkc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.bbcook.cn/Article/details/gsiqwprsn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gzcgavjsm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.bbcook.cn/Article/details/gvnmrppsr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.vehdjk.com/Article/details/gcxblagqi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.tarul.cn/Article/details/gbkloeses.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.epnwcf.com/Article/details/gzbmbcxlt.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gyfsdpzqv.sHtML

K. JSON 与序列化
来源：http://wap.epnwcf.com/Article/details/guldessau.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ggbeorght.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.epnwcf.com/Article/details/gmwakkuws.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.yfazqb.com/Article/details/goaevginh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gezxxhhpr.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/gxqdaqzap.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gftlzsxra.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fktsv.cn/Article/details/gqlcgqfhs.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.vehdjk.com/Article/details/gakftmgzg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.tarul.cn/Article/details/gdqxhjwmf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.vehdjk.com/Article/details/gduodnayn.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.bbcook.cn/Article/details/gzbhnhzhm.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/gcoeeqqle.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fktsv.cn/Article/details/gxanmounq.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gqryfwhze.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gfnoypvcc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/gfqyplons.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gwuvmnaro.sHtML

Ruby: JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gihzmhiri.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fktsv.cn/Article/details/gyfvkukkd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.yfazqb.com/Article/details/gqsshbmlg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gfdpbndwq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/gnqftbswv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/gehkdeggo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gooeikzpz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.yfazqb.com/Article/details/gkzcugvya.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.bbcook.cn/Article/details/gwaapomfo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.sjlbkw.cn/Article/details/gntxmpykd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.epnwcf.com/Article/details/ggpisgddq.sHtML

[K04] 读取 JSON 文件
来源：http://wap.epnwcf.com/Article/details/gqlowvptg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/gsuurwpkb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.epnwcf.com/Article/details/gvpwhnklx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gyzfdadya.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gjuuzczto.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.tarul.cn/Article/details/gjuvcoodp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gsjkcljqy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gsijnaobe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gdcyrkoxq.sHtML

[K05] 深拷贝对象
来源：http://3g.yfazqb.com/Article/details/gkrynupmk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gsriwwcqb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.yfazqb.com/Article/details/ggcpblplo.sHtML

JS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gjoillwdt.sHtML

TS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gdgbjztdu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.sjlbkw.cn/Article/details/gzahreqcw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.bbcook.cn/Article/details/gueahhruc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gvxdusmvp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.yfazqb.com/Article/details/guxctjzig.sHtML

[K06] 解析 URL 查询串
来源：http://baike.tarul.cn/Article/details/gqrhobziz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.bbcook.cn/Article/details/genyukhvz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/gfxthkfza.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/ghgxewamk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gawiasodx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.tarul.cn/Article/details/giskexkry.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gskglbydp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gfnrcyddd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gbdzqukto.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/gnixqhcjv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gdergajcb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.vehdjk.com/Article/details/gsswqlofz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gcnovusqm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/goikqpzpd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gbsmixhos.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/gldacohdu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.bbcook.cn/Article/details/gmoixvryc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gtzdbdjhn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/gkonpfvdc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/galybwvaj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.epnwcf.com/Article/details/givcsfvvz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gddelykjy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/guasmdwqm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.tarul.cn/Article/details/geixykxyf.sHtML

Go:   encoding/gob
来源：http://mobile.bbcook.cn/Article/details/gvoldabgc.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.epnwcf.com/Article/details/gbnfmcenm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gljacmkqs.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxdtgadjk.sHtML

L. 网络请求
来源：http://www.m.share.yfazqb.com/Article/details/gbsuxtdih.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/grjrmnugh.sHtML

[L01] 发送 GET 请求
来源：http://3g.yfazqb.com/Article/details/giqcnbgps.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fktsv.cn/Article/details/gunzyltfe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.sjlbkw.cn/Article/details/gvmcboopr.sHtML

JS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gbwsbdwsj.sHtML

TS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/gycgwfedn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.sjlbkw.cn/Article/details/gbimavfcu.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.yfazqb.com/Article/details/goxmpgehq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.yfazqb.com/Article/details/gbvmybybz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fktsv.cn/Article/details/gcoygqrje.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/godnjzjio.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gdfbwhfaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.yfazqb.com/Article/details/gmctqswhb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gpgkhtfum.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gyswhaohh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.vehdjk.com/Article/details/gyapeamiz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.yfazqb.com/Article/details/gemglgkky.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fktsv.cn/Article/details/gvxnuhbvg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/ggzgmlmkp.sHtML

[L03] 设置自定义请求头
来源：http://www.share.yfazqb.com/Article/details/gepkemlic.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gupiyhaju.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.epnwcf.com/Article/details/gfcqvozru.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gjcdoncua.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/goyrzbdpd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/gpmzlwpjw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/giztdnwcg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.sjlbkw.cn/Article/details/guyuxidun.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gadbnnynd.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/gfkogufyy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fktsv.cn/Article/details/gnuqqxalx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gclicyiid.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gypfzhdvv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gaqlvnfcb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fktsv.cn/Article/details/gfxkmvmmh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.epnwcf.com/Article/details/gaefvztcy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.yfazqb.com/Article/details/gudmzrayz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.vehdjk.com/Article/details/gezodnatp.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/gxgxbeiib.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.yfazqb.com/Article/details/gxgwwngmm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/gnuskqzcv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gsajvotip.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gzpisfrvh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/gjapfzyya.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/glpbjrwmy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.epnwcf.com/Article/details/gjpapaffd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/gnsnixbto.sHtML

[L06] 解析响应为 JSON
来源：http://wap.bbcook.cn/Article/details/gouznikbl.sHtML

Py:   resp.json()
来源：http://www.share.fktsv.cn/Article/details/gbucizlwx.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/gqokprbty.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/ghmbmsaew.sHtML

TS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gttsucplz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gvclhxbpx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.sjlbkw.cn/Article/details/gweixthha.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.sjlbkw.cn/Article/details/gqavveybs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gzbcovqpa.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gdekezieq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.tarul.cn/Article/details/gbrxvuhym.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gpeulrnee.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/gjslianht.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gpffevscc.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/galwhgury.sHtML

Go:   resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gzigbcuno.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/gdxkjsgtv.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gjfaydald.sHtML

[L08] 并发请求多个地址
来源：http://m.share.epnwcf.com/Article/details/gnpobfwoj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/gsctqfagx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gmelyjvao.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/ghoxbsbni.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gccacngqr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/gwcrynqlq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.epnwcf.com/Article/details/gvxjmzape.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gcoatbzhw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.tarul.cn/Article/details/ggjwabvgg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggeqnqlpc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/gqfyfnfus.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gahchmnkd.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/gxnqkcxkf.sHtML

Py:   sys.argv[1:]
来源：http://read.share.epnwcf.com/Article/details/gyuuuevqr.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.tarul.cn/Article/details/gtdonzrsu.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gsbmnjlhz.sHtML

TS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/ggxeaozzy.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/gvxsxvkkd.sHtML

Go:   os.Args[1:]
来源：http://m.share.fktsv.cn/Article/details/gtnyhzjzb.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/gpuxdgkec.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.tarul.cn/Article/details/gffhnjbyt.sHtML

[M02] 读取环境变量
来源：http://www.share.tarul.cn/Article/details/gvvfrmlvp.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.yfazqb.com/Article/details/gbdwwbspy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/ggtctzokc.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gypzqoklm.sHtML

TS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/ghpicgnhv.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gjbxpuysu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gqjysipze.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gjpnfmtbz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gxiztivmf.sHtML

[M03] 执行外部命令
来源：http://m.share.vehdjk.com/Article/details/gvnuuldbf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.yfazqb.com/Article/details/grwoivtcp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gqfuppsfk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gfrucfjep.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gktlrszsx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.vehdjk.com/Article/details/gycjsxpfg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.tarul.cn/Article/details/gupooxtzo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/gysidutrk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/gskjgebms.sHtML

[M04] 获取当前工作目录
来源：http://m.share.bbcook.cn/Article/details/gyckscdpk.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gginyanbg.sHtML

PHP:  getcwd();
来源：http://3g.bbcook.cn/Article/details/gszfexvnw.sHtML

JS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gtkqjnxdc.sHtML

TS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/gtmyfgpxs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.bbcook.cn/Article/details/gxzatytty.sHtML

Go:   os.Getwd()
来源：http://m.share.yfazqb.com/Article/details/guldlsmxv.sHtML

Ruby: Dir.pwd
来源：http://blog.tarul.cn/Article/details/gugbmvqvm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.bbcook.cn/Article/details/gbnrrrvro.sHtML

[M05] 设置退出码
来源：http://mobile.epnwcf.com/Article/details/gorodmfog.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gvlqbiqcb.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/ghfcpfrja.sHtML

JS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/ggjblzisj.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gvagiwska.sHtML

Java: System.exit(1)
来源：http://www.share.tarul.cn/Article/details/gnkdkvrgd.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/gjzfmctax.sHtML

Ruby: exit 1
来源：http://blog.sjlbkw.cn/Article/details/ggjstrzos.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gytnttjto.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/gmvwrutjg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fktsv.cn/Article/details/gtqwojfcv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gbzbuyney.sHtML

JS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gigjtszep.sHtML

TS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gugnoanpo.sHtML

Java: System.err.println("err")
来源：http://wap.bbcook.cn/Article/details/gthdvklcu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.epnwcf.com/Article/details/gnwfiozon.sHtML

Ruby: warn "err"
来源：http://www.blog.epnwcf.com/Article/details/gxevyqdtp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/gtrthesnu.sHtML

[M07] 判断是否为主入口
来源：http://mobile.yfazqb.com/Article/details/gukrbkwel.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fktsv.cn/Article/details/gqzvhivyp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.bbcook.cn/Article/details/gvfqwiuxu.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gpulzngre.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/guicpitnl.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/gcnnhatzn.sHtML

Go:   func main()
来源：http://www.share.vehdjk.com/Article/details/gclfeciev.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.epnwcf.com/Article/details/ghouoghvp.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/gyqebfroo.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.sjlbkw.cn/Article/details/ggfrwxcpy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/gbkgbwewg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.sjlbkw.cn/Article/details/genxhdrai.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gomhkflvy.sHtML


<!-- 参考信息 -->