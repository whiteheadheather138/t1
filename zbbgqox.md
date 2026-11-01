代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.epnwcf.com/Article/details/gclyyonjc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.epnwcf.com/Article/details/gqiwgoatt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/glybwxcxf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkzwclyct.sHtML

J. 日期与时间
来源：http://www.blog.epnwcf.com/Article/details/gwzogclaf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/guidphkgr.sHtML

[J01] 获取当前时间
来源：http://blog.epnwcf.com/Article/details/gfoxjvhil.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.bbcook.cn/Article/details/gxcebwtwr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/gkirzlzry.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gjdbgfdyn.sHtML

TS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gwldxulrj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.epnwcf.com/Article/details/gkqxqycth.sHtML

Go:   time.Now()
来源：http://wap.vehdjk.com/Article/details/ghlisovrg.sHtML

Ruby: Time.now
来源：http://wap.bbcook.cn/Article/details/gmwkkifke.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.yfazqb.com/Article/details/ggfqqedyn.sHtML

[J02] 格式化输出
来源：http://m.share.bbcook.cn/Article/details/gqhutrqvz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gupvwlors.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gtiunisid.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.bbcook.cn/Article/details/gdnqaebce.sHtML

TS:   d.toISOString()
来源：http://blog.sjlbkw.cn/Article/details/gdgwfjegh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.epnwcf.com/Article/details/gdkydmwaj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.epnwcf.com/Article/details/gnjktlfyj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/gqbnyvfgh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqygdyzqc.sHtML

[J03] 字符串解析为日期
来源：http://read.share.epnwcf.com/Article/details/gssljxfmu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.epnwcf.com/Article/details/gsjqwqpmc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.epnwcf.com/Article/details/gcewqmogy.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gtoomzkei.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gvvdpiqev.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gzkpcwjeq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/gmkpdyjjl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gsesvzlxv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.bbcook.cn/Article/details/gidrgwwev.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.vehdjk.com/Article/details/gyhchwrrr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.tarul.cn/Article/details/gorliyifh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.bbcook.cn/Article/details/gvbotfmgk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.tarul.cn/Article/details/gqynjjhxl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.tarul.cn/Article/details/gpcxlqzhs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/gumvhmqkp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fktsv.cn/Article/details/gstysfdxs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.epnwcf.com/Article/details/ghakahazm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.yfazqb.com/Article/details/ghpwvlqmr.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fktsv.cn/Article/details/graulfabf.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.bbcook.cn/Article/details/grucwouuj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.epnwcf.com/Article/details/gndxhkykt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/gipgkufkb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gfjhnidpr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/ggcawdvkk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.tarul.cn/Article/details/grvhogecn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/guiqsecfv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.bbcook.cn/Article/details/ginqsdnwh.sHtML

[J06] 计算两时间之差
来源：http://blog.yfazqb.com/Article/details/gajearchk.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.epnwcf.com/Article/details/ghgivwwxb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.tarul.cn/Article/details/gdbubhsmg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.epnwcf.com/Article/details/gaxiozemm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.epnwcf.com/Article/details/ghrjxjqnx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.sjlbkw.cn/Article/details/gdvdgkneh.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.bbcook.cn/Article/details/gncrhuyqh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.bbcook.cn/Article/details/gkmiepaue.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.bbcook.cn/Article/details/geumsokpz.sHtML

[J07] 比较两个日期
来源：http://www.share.vehdjk.com/Article/details/gijmmiktp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gsrnykncg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fktsv.cn/Article/details/gyemapwuk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gtoxwwwtl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gvxsdoapg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gnbuxqrom.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/ggvvzyupi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gtloiaiol.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrtomuyx.sHtML

[J08] 提取年月日与星期
来源：http://www.share.sjlbkw.cn/Article/details/gqbupprsx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.bbcook.cn/Article/details/guzfvzrft.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fktsv.cn/Article/details/gwvfmqgez.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.vehdjk.com/Article/details/gcrsrfmfd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnhdxmwk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/gnvimlgzk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.yfazqb.com/Article/details/gsbbpjhco.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/gzonjnhtt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.sjlbkw.cn/Article/details/gtcojphnc.sHtML

[J09] 时区处理
来源：http://www.share.bbcook.cn/Article/details/gymbjnntt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fktsv.cn/Article/details/gnmgcwbvw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.sjlbkw.cn/Article/details/gomaxjsbr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.vehdjk.com/Article/details/gtvlcelkp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/geetyjndl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.epnwcf.com/Article/details/gmzchnxre.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fktsv.cn/Article/details/gavcayhsm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.tarul.cn/Article/details/ghwodmeml.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fktsv.cn/Article/details/grbiaduud.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.vehdjk.com/Article/details/gobbclljk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.sjlbkw.cn/Article/details/goxwuaziv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fktsv.cn/Article/details/glfklxzrd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.sjlbkw.cn/Article/details/gywrtomni.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.yfazqb.com/Article/details/gnapkoxpu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fktsv.cn/Article/details/gwekoivmj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fktsv.cn/Article/details/gyeixyogr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.yfazqb.com/Article/details/goxrzdjkc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.bbcook.cn/Article/details/gjxivedmf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzhssxmwu.sHtML

K. JSON 与序列化
来源：http://read.share.epnwcf.com/Article/details/gqjyndlid.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/grpntcarh.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.tarul.cn/Article/details/gvqvopxnu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gfkfdgkqp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gshthbjul.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/goyarfkly.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/gfrdobzro.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/gtcmnhrpd.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.vehdjk.com/Article/details/guyodpknr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fktsv.cn/Article/details/gqacwmedk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gmiudvtul.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fktsv.cn/Article/details/gyhyrrafj.sHtML

Py:   json.loads(s)
来源：http://mobile.bbcook.cn/Article/details/griyqwkxr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.bbcook.cn/Article/details/gvjehrylc.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gwgvdmhyi.sHtML

TS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gyrlrabco.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.bbcook.cn/Article/details/gejelhbdp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gwnxypldz.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gpultaawj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gjvmlcidc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/ghlepibjw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gsqgfrvkc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gktqhcsup.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gsdfbkqkp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/gsoflojmq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gzgsvcait.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.sjlbkw.cn/Article/details/glvproptu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.epnwcf.com/Article/details/gubmbtwqp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.bbcook.cn/Article/details/gqcmccbnk.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fktsv.cn/Article/details/grngjioca.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.epnwcf.com/Article/details/gwcokfynq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.bbcook.cn/Article/details/gbusyzczi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gukwegrkl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gqghyfife.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gtkzfgaeq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gemvlpeqe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.bbcook.cn/Article/details/glaiazamb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gonfgrbcc.sHtML

[K05] 深拷贝对象
来源：http://baike.tarul.cn/Article/details/gjoyuofnp.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.epnwcf.com/Article/details/gobvupezd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/glsavbuww.sHtML

JS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gdahpyucp.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gghnacucc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.yfazqb.com/Article/details/gwzhuehyi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/gcrmqvwva.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.sjlbkw.cn/Article/details/glirqvjml.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.tarul.cn/Article/details/ggepadgzd.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gxypfdkhm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gubqvavwo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.sjlbkw.cn/Article/details/gelxlejpw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/goldiwofh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gveqhoqvy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gogkjswfr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gokwiuuxu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gvojfnssq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gjzjijqai.sHtML

[K07] 进制转换
来源：http://baike.bbcook.cn/Article/details/gjaecsvyy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gvnhnlcbm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/ggexqkjgv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gjsqofccz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gzbetjsdq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gvmvemzto.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.bbcook.cn/Article/details/gqwgoptjs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/gqqpsszqu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gznapviiw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/gejkdshem.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/gbmrxcajx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.sjlbkw.cn/Article/details/gvodgbcae.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gwitohdus.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gjphrmdvg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/gljhacsxc.sHtML

Go:   encoding/gob
来源：http://3g.epnwcf.com/Article/details/gpcwdptvc.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhjhbrnz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/gtrsomilu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkvqbbszd.sHtML

L. 网络请求
来源：http://mobile.bbcook.cn/Article/details/gtmeyoawz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gokxotkma.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fktsv.cn/Article/details/gphsdggci.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.epnwcf.com/Article/details/gelvaygyd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.bbcook.cn/Article/details/gwyprgids.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/ggpqryevq.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/ggifbbqgm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fktsv.cn/Article/details/gfslzuawb.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.yfazqb.com/Article/details/gcflikklz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/gmiyvonhh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.tarul.cn/Article/details/gmgbhjkvq.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/gdimajibr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gehwvrycb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.epnwcf.com/Article/details/gaekouvbd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gyijbpdrv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gohjmblev.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/gjbpibwxe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gnncjsxgu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/gyzdnsbja.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/ghcpbubin.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fktsv.cn/Article/details/gvwhsdbkc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gkpfkrwrt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtshsmokc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gcighxfqg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gpvkiaapw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.vehdjk.com/Article/details/gdgiqeynb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/grdwftucs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.tarul.cn/Article/details/gmtbodtup.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gccgtouea.sHtML

[L04] 设置超时
来源：http://www.blog.tarul.cn/Article/details/gqmakcxgr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhxjkkzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.vehdjk.com/Article/details/gtincqwjk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gjacpcdth.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gelhqjche.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fktsv.cn/Article/details/gmgmxhdtu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gcgbwpfdj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.vehdjk.com/Article/details/gklkbfaiq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.vehdjk.com/Article/details/gbufvwyul.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/gvhxnevzx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.vehdjk.com/Article/details/gvhrbabfw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/ggmfdpvbh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gfondzofp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gjvbyfdzg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.bbcook.cn/Article/details/gvhokhvij.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.sjlbkw.cn/Article/details/gthlturvi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fktsv.cn/Article/details/gqucvovny.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.bbcook.cn/Article/details/gteaumqlk.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/gpbdbwgqr.sHtML

Py:   resp.json()
来源：http://wap.epnwcf.com/Article/details/groxgfroa.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/gghfcrsxt.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gvuomtdlv.sHtML

TS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gzmliovbb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gvhpzeuju.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.vehdjk.com/Article/details/gwfyqmfxf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.bbcook.cn/Article/details/gzvlrhflw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.sjlbkw.cn/Article/details/gsnljreta.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gjyuqlsqs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/gcafykdmx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.bbcook.cn/Article/details/gyfctfxan.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/gmacjfixq.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gysosjxnz.sHtML

Java: resp.statusCode()
来源：http://mobile.fktsv.cn/Article/details/gtenumxru.sHtML

Go:   resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gvhrfdyrv.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gjkjbaxvk.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gcfetaasp.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gzbyxgbpk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gztxqkngm.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.vehdjk.com/Article/details/gunmneimh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/ggilkjzul.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gmjfzdixi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.epnwcf.com/Article/details/ggfgasvgq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.epnwcf.com/Article/details/gtoyfqtfe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.bbcook.cn/Article/details/gtkrnqebf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.epnwcf.com/Article/details/gyazrijol.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrjtbzok.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.tarul.cn/Article/details/gkrrxsjny.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/guouoxnah.sHtML

[M01] 读取命令行参数
来源：http://blog.bbcook.cn/Article/details/ggccghugk.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/gtflipccp.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fktsv.cn/Article/details/gshrghuwk.sHtML

JS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gbimhzzfv.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gwsomhjox.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gkeisddjh.sHtML

Go:   os.Args[1:]
来源：http://blog.bbcook.cn/Article/details/gtyxjcsnb.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/gdqocanzl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gcpxanzho.sHtML

[M02] 读取环境变量
来源：http://www.share.tarul.cn/Article/details/gyximhnon.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.epnwcf.com/Article/details/gdlzatxqu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gxxpfqjrl.sHtML

JS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gwjdglzbp.sHtML

TS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gssafpztu.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/geknfuovg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gpmvkyjyd.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/gsvtrimfr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/gvbpadpzw.sHtML

[M03] 执行外部命令
来源：http://www.share.fktsv.cn/Article/details/gmnfliffq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/gpktenytr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/gsneopgse.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gizxgrjlr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/ggqoybomh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gnakpkzdd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.vehdjk.com/Article/details/gnjprlttp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/gywrnlnab.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/goxgwantw.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwlgfbws.sHtML

Py:   os.getcwd()
来源：http://read.share.yfazqb.com/Article/details/gmuuzjhrj.sHtML

PHP:  getcwd();
来源：http://read.share.fktsv.cn/Article/details/gjuzsbveu.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gjieopdco.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gqbbpvrqp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gjztonzfq.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gcvrhlnpu.sHtML

Ruby: Dir.pwd
来源：http://blog.tarul.cn/Article/details/grvdqskho.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.bbcook.cn/Article/details/gkiyhwolk.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/glndljaoh.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gxfkqzhva.sHtML

PHP:  exit(1);
来源：http://mobile.bbcook.cn/Article/details/guoziqdyy.sHtML

JS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gyaalpmsv.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gdvmlaqrk.sHtML

Java: System.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gjntjyopp.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/ggthkqhli.sHtML

Ruby: exit 1
来源：http://www.share.fktsv.cn/Article/details/gyywfkfuj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gmncniwyk.sHtML

[M06] 向标准错误输出
来源：http://mobile.vehdjk.com/Article/details/goaqarvyf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/godojgxba.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.sjlbkw.cn/Article/details/gwdccvpph.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gcbphxjqr.sHtML

TS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/glntlqktp.sHtML

Java: System.err.println("err")
来源：http://read.share.vehdjk.com/Article/details/gundbgxns.sHtML


<!-- 参考信息 -->