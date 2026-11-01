代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.yfazqb.com/Article/details/gcegnjfzq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.bbcook.cn/Article/details/gyqspjiru.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/guyetkwic.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.vehdjk.com/Article/details/gmovehyzp.sHtML

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/gxuozrmaa.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.vehdjk.com/Article/details/gosaefmdh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fktsv.cn/Article/details/gdasjhpsz.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gwdsxsndk.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gyhtyfjie.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gatlrxuml.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/grbkbslrv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/guriluakt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.tarul.cn/Article/details/glvbeuzbs.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/gzveqjobh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.yfazqb.com/Article/details/ggxdejpgt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.bbcook.cn/Article/details/gbbypeysd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.vehdjk.com/Article/details/gxhltvgzd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.vehdjk.com/Article/details/gytrfwtla.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.tarul.cn/Article/details/gsdhdjfjb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.yfazqb.com/Article/details/gkoejxbzt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.bbcook.cn/Article/details/gdwnfdvdh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.tarul.cn/Article/details/gbgfnyyvd.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.epnwcf.com/Article/details/gidpoymkp.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.sjlbkw.cn/Article/details/gjfofgzsv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.bbcook.cn/Article/details/gavbuprcw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gjibkphkq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gdwzwroor.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.epnwcf.com/Article/details/gpicxhpft.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/grromrzno.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.bbcook.cn/Article/details/gctvqswez.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/grdvtcddl.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/gisbzzlrd.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.epnwcf.com/Article/details/gnyezybzb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.bbcook.cn/Article/details/gbohvbyfc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.bbcook.cn/Article/details/ghbvvlfpy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/gihoipcjn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.sjlbkw.cn/Article/details/gppsrjuaq.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.vehdjk.com/Article/details/gswixnuoe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.tarul.cn/Article/details/gvhnsmdnq.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fktsv.cn/Article/details/gaccmceaf.sHtML

[J07] 比较两个日期
来源：http://www.share.fktsv.cn/Article/details/gvvuvacch.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gxfbcadfb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.vehdjk.com/Article/details/gssntkalg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/gytlywutk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/guurhzvpi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.epnwcf.com/Article/details/gqpplyuio.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.tarul.cn/Article/details/gnwfduilk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/ghpjftcag.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gnhaoplzl.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/ghufzagbw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.tarul.cn/Article/details/guuurlyqs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/guumsrepq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.tarul.cn/Article/details/gzlnlidwh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fktsv.cn/Article/details/gkvmxrega.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.tarul.cn/Article/details/gvyavtpbh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.vehdjk.com/Article/details/ghrcprlrz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.bbcook.cn/Article/details/gllwxwrks.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gacfczvmc.sHtML

[J09] 时区处理
来源：http://www.share.bbcook.cn/Article/details/gwikmlfwb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.vehdjk.com/Article/details/ggfgfcvyf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.bbcook.cn/Article/details/gjilwdrde.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gdgujtbpv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/gzcyzidxz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.epnwcf.com/Article/details/gsphjjmvy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fktsv.cn/Article/details/gmcjkwvaj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.yfazqb.com/Article/details/grnpdthnl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.tarul.cn/Article/details/glpdjsqtj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fktsv.cn/Article/details/gdtpdvhgf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/ghhbhgvzz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.epnwcf.com/Article/details/glvpgpqbz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.tarul.cn/Article/details/gektiizau.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/gwodzmxkz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.epnwcf.com/Article/details/gidqdosxo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gdjwpzjki.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.yfazqb.com/Article/details/gqmbhuhid.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.yfazqb.com/Article/details/gbdgvwtls.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkxizypzq.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/gkwahzqrf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gyebgcwtv.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.tarul.cn/Article/details/gspjghbyo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gazzakdco.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/ggoiziqat.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/gsexubibf.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gjociyrbs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.sjlbkw.cn/Article/details/gvwwrzito.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fktsv.cn/Article/details/grlcaqkia.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/gqpwzzgpp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.sjlbkw.cn/Article/details/giknknish.sHtML

[K02] JSON 字符串转对象
来源：http://3g.epnwcf.com/Article/details/gjqzpgrjm.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/gcligkiup.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.epnwcf.com/Article/details/gqqogmukx.sHtML

JS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gwpqaaoin.sHtML

TS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/grkncjpyp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.bbcook.cn/Article/details/gdkbxtkcd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gsyzsckuq.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gkxqpmapg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/gzkxzyrcc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gmoyzczjk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gvziefkrr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gwwldvizp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/glvtrycdm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/gonnzekeh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/ggscbbhug.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.tarul.cn/Article/details/gjiszzwcy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.sjlbkw.cn/Article/details/glukchbbl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.vehdjk.com/Article/details/gmgnzipee.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/gdldxawyz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.vehdjk.com/Article/details/gfjabwgfl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.vehdjk.com/Article/details/ghkfkwgjb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gudjoctgd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gjzimgtgq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/grxnkdybk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gnefgtvcv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gjditmvmb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/gtjrafnkz.sHtML

[K05] 深拷贝对象
来源：http://www.blog.bbcook.cn/Article/details/gndtxjjoy.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.tarul.cn/Article/details/gnyxlmwfy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.vehdjk.com/Article/details/gwsxcrcsw.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gqqfsboil.sHtML

TS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gjmdigban.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/gnfbdtorw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.tarul.cn/Article/details/gfcalnprg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.vehdjk.com/Article/details/grjkboecg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/gqrzgnwvm.sHtML

[K06] 解析 URL 查询串
来源：http://baike.vehdjk.com/Article/details/gfacmpmin.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/ghkzvdhig.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.bbcook.cn/Article/details/gqpzwufvq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gamatxizu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/grpekvute.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.bbcook.cn/Article/details/gqpmchefn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gwqhtykwe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gvghzdhok.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gvtbznbnh.sHtML

[K07] 进制转换
来源：http://blog.epnwcf.com/Article/details/gcgllgcmp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gzznekqju.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.tarul.cn/Article/details/ggeqfbluz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gtewygrgf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gjuticxlk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gbpomxesj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gzprvaopt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.vehdjk.com/Article/details/gmvcphzuy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gjhatmxuv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.tarul.cn/Article/details/ggplkrvgk.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.epnwcf.com/Article/details/gghwyfkir.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.sjlbkw.cn/Article/details/gbkcnzwwb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gkqhrgseg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gjhvnkmit.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.epnwcf.com/Article/details/gbhkerjll.sHtML

Go:   encoding/gob
来源：http://wap.sjlbkw.cn/Article/details/ggbktrafn.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.bbcook.cn/Article/details/gghmatxdx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/gzldwumzf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmawmjxgp.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/gnmiwgohm.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gofcsgxvs.sHtML

[L01] 发送 GET 请求
来源：http://wap.tarul.cn/Article/details/gpnahtnij.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/ggoyhwjba.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.yfazqb.com/Article/details/gxxikfbny.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gavmwqmbd.sHtML

TS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/grooiakft.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fktsv.cn/Article/details/gfoilcocl.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/gvbcoxysa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gdtfpkjfo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.bbcook.cn/Article/details/giietzbag.sHtML

[L02] 发送 POST JSON
来源：http://wap.yfazqb.com/Article/details/gzdosuppf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.bbcook.cn/Article/details/grbtehcik.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.yfazqb.com/Article/details/gvedmgcki.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gyrnhkfyg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gapyibypq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fktsv.cn/Article/details/ghhdhdvgf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.sjlbkw.cn/Article/details/gxztbacwv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.vehdjk.com/Article/details/gmagqocjt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gzbkdfthe.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.bbcook.cn/Article/details/gppuocqpg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fktsv.cn/Article/details/gnvckukyt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fktsv.cn/Article/details/geicdbhfb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gvpzzfgev.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gqojoivgo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.sjlbkw.cn/Article/details/gwdsixhec.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/gbkwxxnfv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/gtiyortld.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkmkolor.sHtML

[L04] 设置超时
来源：http://www.m.share.tarul.cn/Article/details/gghtzrxkw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.tarul.cn/Article/details/gvjqcmgiu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/gbuyefufp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gimiemtej.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/grqhlpfbu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.tarul.cn/Article/details/gqnhvrtcq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fktsv.cn/Article/details/goxeecmmg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.epnwcf.com/Article/details/geczudrtk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/gqsojykcm.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.sjlbkw.cn/Article/details/gbswtsycl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/giarzayhg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.epnwcf.com/Article/details/ghtqjkkwe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gwuakofiu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/giyunaffh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fktsv.cn/Article/details/gfqxtduon.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/gwdvyovlo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmtbjwzm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gdympboaa.sHtML

[L06] 解析响应为 JSON
来源：http://3g.sjlbkw.cn/Article/details/gpehuxdgq.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/ggxedwqnk.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gcttanurh.sHtML

JS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gueawxowg.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/genamzptt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.vehdjk.com/Article/details/ggfjeriwn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.epnwcf.com/Article/details/gzzfdgxuo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gkgunjfcn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.yfazqb.com/Article/details/gxdkgyvdr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gmsfesdud.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.yfazqb.com/Article/details/ghmtvupvi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.sjlbkw.cn/Article/details/gkavnuwck.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/ghztntasd.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/ghuvsninl.sHtML

Java: resp.statusCode()
来源：http://3g.epnwcf.com/Article/details/gripubejx.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gutapnzhj.sHtML

Ruby: resp.code.to_i
来源：http://baike.tarul.cn/Article/details/gvimiwukj.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gxdauoxyb.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gdjwgoptm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.bbcook.cn/Article/details/gwsogvfzo.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.bbcook.cn/Article/details/gpuftgzjt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gmilaueuw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gqcartsmp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fktsv.cn/Article/details/gqlclhokp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fktsv.cn/Article/details/gloolnasf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gpbhuclwx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.bbcook.cn/Article/details/gcdednsde.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gciwkqiho.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.yfazqb.com/Article/details/ggktfnctn.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzesnunhs.sHtML

[M01] 读取命令行参数
来源：http://3g.fktsv.cn/Article/details/gjvtynmjh.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fktsv.cn/Article/details/gbioqfvjz.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/ghdznqewk.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gazkxnper.sHtML

TS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gwwouhnnj.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.tarul.cn/Article/details/groszwehh.sHtML

Go:   os.Args[1:]
来源：http://www.share.fktsv.cn/Article/details/gwsqwmpqa.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gofznhnpk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gvjpfxeif.sHtML

[M02] 读取环境变量
来源：http://mobile.bbcook.cn/Article/details/ghwzeheiz.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.vehdjk.com/Article/details/gtdxrmvjo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gzxdilgnd.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gewoxddzq.sHtML

TS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gpqctlkfd.sHtML

Java: System.getenv("HOME")
来源：http://wap.bbcook.cn/Article/details/gmecbhdkf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gxqyiejzz.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gssjksgkt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gmksjbxuq.sHtML

[M03] 执行外部命令
来源：http://baike.epnwcf.com/Article/details/gczqaoqdm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.vehdjk.com/Article/details/gpwivzlqp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.vehdjk.com/Article/details/gcndtytuw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gsrhvnfia.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gcocabxzb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gvczqrduz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.sjlbkw.cn/Article/details/goxhtydrr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.vehdjk.com/Article/details/grfarhaxh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fktsv.cn/Article/details/gextdndpm.sHtML

[M04] 获取当前工作目录
来源：http://3g.epnwcf.com/Article/details/gmoajetge.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/goywzywld.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gcfqxjxxk.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gcydtopge.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gbjurinut.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/gpkbvthxa.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gcshbpxze.sHtML

Ruby: Dir.pwd
来源：http://m.share.tarul.cn/Article/details/gswjysloe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/glipnejfe.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/gvyqqezad.sHtML

Py:   sys.exit(1)
来源：http://blog.vehdjk.com/Article/details/gzeqskljl.sHtML

PHP:  exit(1);
来源：http://www.share.epnwcf.com/Article/details/giczitmfj.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gvtdehann.sHtML

TS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gfmhxqaka.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/glgbwjili.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/gihwnnuou.sHtML

Ruby: exit 1
来源：http://mobile.tarul.cn/Article/details/gmodyeapf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/ggmtzjzbk.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gljqfoyis.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gvpruldnx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gdtdexcla.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gwboaoupe.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gfzvrbqar.sHtML

Java: System.err.println("err")
来源：http://www.share.bbcook.cn/Article/details/guwvnwjmb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gighgzuqs.sHtML

Ruby: warn "err"
来源：http://read.share.vehdjk.com/Article/details/ghuymmadp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/gjzategoo.sHtML

[M07] 判断是否为主入口
来源：http://mobile.tarul.cn/Article/details/gyaznrcwa.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fktsv.cn/Article/details/gqrgscbvy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.bbcook.cn/Article/details/giswojfgi.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gqvlsdjbz.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gkmddityn.sHtML

Java: public static void main(String[] args)
来源：http://wap.sjlbkw.cn/Article/details/gqaqynrlx.sHtML

Go:   func main()
来源：http://www.share.fktsv.cn/Article/details/gvgrmjduq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.vehdjk.com/Article/details/gqmnicvyb.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gfkkuetzz.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.epnwcf.com/Article/details/gpzdvtljz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/gmorwofgh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fktsv.cn/Article/details/ggpngkbzc.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/govpecrbk.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gtkvfddgf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.yfazqb.com/Article/details/gjagfgkps.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gprnsjhst.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.tarul.cn/Article/details/gicdrdprb.sHtML


<!-- 参考信息 -->