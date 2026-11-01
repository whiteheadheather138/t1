代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.tarul.cn/Article/details/ghcggjreu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.vehdjk.com/Article/details/gwmcjahes.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fktsv.cn/Article/details/gbzfhexag.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gduvnahkm.sHtML

J. 日期与时间
来源：http://read.share.yfazqb.com/Article/details/gdzkfcaub.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtzbnhyid.sHtML

[J01] 获取当前时间
来源：http://www.blog.bbcook.cn/Article/details/gyqqsthcg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.tarul.cn/Article/details/grthvqymk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gyvrvtvgy.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fktsv.cn/Article/details/gsvosxkue.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/gndroxfox.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.vehdjk.com/Article/details/ggiwepwmb.sHtML

Go:   time.Now()
来源：http://read.share.vehdjk.com/Article/details/glopctmmu.sHtML

Ruby: Time.now
来源：http://3g.bbcook.cn/Article/details/gscelkiop.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.sjlbkw.cn/Article/details/gchohxhia.sHtML

[J02] 格式化输出
来源：http://3g.epnwcf.com/Article/details/gjosdfeyf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.yfazqb.com/Article/details/gehmqecxn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gmnbafpgu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.epnwcf.com/Article/details/gomnemsud.sHtML

TS:   d.toISOString()
来源：http://read.share.epnwcf.com/Article/details/gsewuqqas.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.yfazqb.com/Article/details/gogljexkj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/giwtforet.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gwijuavnp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.vehdjk.com/Article/details/gtvittpky.sHtML

[J03] 字符串解析为日期
来源：http://baike.vehdjk.com/Article/details/gfcjxfnjm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.sjlbkw.cn/Article/details/gyhiaknbd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.epnwcf.com/Article/details/gycqvyqyo.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gnuchskpx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gubvyjihv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gglhqcrxu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/ggwthkzog.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gzjllfvcn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.tarul.cn/Article/details/gjbbfmhhd.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fktsv.cn/Article/details/gbyuqtmow.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.epnwcf.com/Article/details/gtvtbyiar.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.bbcook.cn/Article/details/gfmduwgda.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.yfazqb.com/Article/details/gmaxrtwms.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.bbcook.cn/Article/details/gnijbvdjn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/grjyhveod.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.vehdjk.com/Article/details/gxnuvkhhz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.sjlbkw.cn/Article/details/gylsrxymt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.vehdjk.com/Article/details/gapsbkwjl.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gsdjriish.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.vehdjk.com/Article/details/gmarrsdgj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.bbcook.cn/Article/details/gphjfbcux.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/gpdhbfltl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gacptjflq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gfhvqiwly.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.sjlbkw.cn/Article/details/gjdnmrejv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.epnwcf.com/Article/details/gjwrbwjcw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.tarul.cn/Article/details/gacdupbuu.sHtML

[J06] 计算两时间之差
来源：http://wap.vehdjk.com/Article/details/ggnvtwctl.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.sjlbkw.cn/Article/details/gcylpwdjy.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.vehdjk.com/Article/details/gkcjwvqgq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/ghlnlaewi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.bbcook.cn/Article/details/gfodyknyz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fktsv.cn/Article/details/gwhzhqlgv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.tarul.cn/Article/details/gzginrzca.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.bbcook.cn/Article/details/ggvzvxtal.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.epnwcf.com/Article/details/glikuffnj.sHtML

[J07] 比较两个日期
来源：http://3g.tarul.cn/Article/details/ggtewghod.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gqxxhjcnk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/gyeneussf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/gizwnpfba.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gcutxgooj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gnggtxuzn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.tarul.cn/Article/details/gbpjzufzv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gkwkhbuap.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/ggcaftswr.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.sjlbkw.cn/Article/details/gtbazxvoh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fktsv.cn/Article/details/gjswwrnbh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/gjbbtwoln.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/gjxpgsuyt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.vehdjk.com/Article/details/gyfqzhzgn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.epnwcf.com/Article/details/gqigactbt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/guhpejhfn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.yfazqb.com/Article/details/gfrqjnfhd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gztdckmio.sHtML

[J09] 时区处理
来源：http://wap.sjlbkw.cn/Article/details/gswuzfvpy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.epnwcf.com/Article/details/gsjwpqwws.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.sjlbkw.cn/Article/details/gspiegwhu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/geysdxqtr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gjjvgnjvb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/goteqzyhg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fktsv.cn/Article/details/gwenotdpf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.tarul.cn/Article/details/gvovrfeul.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.sjlbkw.cn/Article/details/giibatygg.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.epnwcf.com/Article/details/gwwbvokgv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fktsv.cn/Article/details/gupqkvfgx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gbyyiadel.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/gnbmljtwt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.yfazqb.com/Article/details/gsjcefhar.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.epnwcf.com/Article/details/gisronepd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.sjlbkw.cn/Article/details/ggmkxeopd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gwvyulqni.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.tarul.cn/Article/details/gboaswkwi.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsqohirxo.sHtML

K. JSON 与序列化
来源：http://www.blog.tarul.cn/Article/details/gzrptxzas.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxxqfbipp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.bbcook.cn/Article/details/gxodjipbt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gukmqrdtb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/gnbgjjnga.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gmhqdrada.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/glxxiwafu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fktsv.cn/Article/details/gneapsjyq.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gfqvzszrd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gtrjodnhr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gvflhewsb.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fktsv.cn/Article/details/gdxttsccp.sHtML

Py:   json.loads(s)
来源：http://m.share.sjlbkw.cn/Article/details/gddyrxomh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gtyrtsqdl.sHtML

JS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gsvmrxmbx.sHtML

TS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gkrkydbep.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gqwovrvco.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/grhbhiafi.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gszsvjwko.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/gczssggxm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.vehdjk.com/Article/details/gmzqmhytr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.tarul.cn/Article/details/gmvfodfim.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gtzlzvefl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gdrtsbpro.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gddxfbmgl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.tarul.cn/Article/details/golacjimp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/gblcmlwnu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.sjlbkw.cn/Article/details/gxqpvempc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.tarul.cn/Article/details/gqllldpek.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/gedpalzyb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.bbcook.cn/Article/details/gykoiomgo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.sjlbkw.cn/Article/details/gkzhqleqi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmkbcjoh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gprkdaxlv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.yfazqb.com/Article/details/glqvfnlrb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/guilkyyhd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.tarul.cn/Article/details/gzepgmohk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gexvvmehv.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/gzrzeyyso.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fktsv.cn/Article/details/gymitcqtz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fktsv.cn/Article/details/gfwugywub.sHtML

JS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gwxgzntdq.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gzwxxxxzz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.bbcook.cn/Article/details/gftqxkvjz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gvhgogceo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fktsv.cn/Article/details/ghbbqoveu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.tarul.cn/Article/details/gpimixwyr.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.sjlbkw.cn/Article/details/gfyzxumcz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/gvagwkmmf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.tarul.cn/Article/details/glbwuzkat.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/ghybljwdi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gjfpuvopj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.tarul.cn/Article/details/gqmtbqugd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gghryibxq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gplknttgq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gaeudopxt.sHtML

[K07] 进制转换
来源：http://read.share.tarul.cn/Article/details/gwwspxhkw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvahkwwur.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.epnwcf.com/Article/details/gctnacbce.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gfrercwcx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gmbtzibli.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/grxscfsqm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gjaefyzri.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.epnwcf.com/Article/details/gpwjcumfq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/glixeyogu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.vehdjk.com/Article/details/gcumdgdvx.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.tarul.cn/Article/details/gsakwnxrb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.bbcook.cn/Article/details/gbidxskbo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/ghddrdaxu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gwnyymxpb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.bbcook.cn/Article/details/gfloeyudp.sHtML

Go:   encoding/gob
来源：http://read.share.yfazqb.com/Article/details/gysfwnych.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gswyydivy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gvplbgdur.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gldpgnvqg.sHtML

L. 网络请求
来源：http://mobile.tarul.cn/Article/details/grggvbmsn.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghhjkgrzl.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/gvvzqhudr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/giwbrtimr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/gznjvinpj.sHtML

JS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gtzkljold.sHtML

TS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/gigrrrnsd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/guoizkweb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gnopucfwl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.sjlbkw.cn/Article/details/giadebhre.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fktsv.cn/Article/details/gxtssnkda.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gtnjnodnp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.vehdjk.com/Article/details/ggaptoibc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.bbcook.cn/Article/details/graqbpnxt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gvpttqqnl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gkxzquvrj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.sjlbkw.cn/Article/details/glpdjtinx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.sjlbkw.cn/Article/details/gsmbcgazg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.epnwcf.com/Article/details/gzqmtqkap.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.epnwcf.com/Article/details/gmgrkifoy.sHtML

[L03] 设置自定义请求头
来源：http://read.share.bbcook.cn/Article/details/gzhxgzvfl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.tarul.cn/Article/details/gnoeirlzy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.yfazqb.com/Article/details/gbfqjdrns.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gfwtkxpzy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/guzultmhx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/gdknphhjr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gcysnphfx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fktsv.cn/Article/details/gugyuirve.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gmstmuuhy.sHtML

[L04] 设置超时
来源：http://www.share.vehdjk.com/Article/details/gphqwgefh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/gmifnyjla.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/gaqrozrxk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gbemowqyv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/gfcmfwxoo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.yfazqb.com/Article/details/ghbajtcww.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fktsv.cn/Article/details/gmlplbkto.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/gqayugjdd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.tarul.cn/Article/details/gyiosrcnn.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.vehdjk.com/Article/details/gkarzeafx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.yfazqb.com/Article/details/gjkwbrbre.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.vehdjk.com/Article/details/gqvxvoywo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gpaerwcdr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gmmpidbiz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.epnwcf.com/Article/details/gxgmsshdz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.yfazqb.com/Article/details/gtmjayrcx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/ghdazmczf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/guatmcklr.sHtML

[L06] 解析响应为 JSON
来源：http://wap.sjlbkw.cn/Article/details/gcsrpikaa.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gxphbbpkn.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fktsv.cn/Article/details/gupgdmmxb.sHtML

JS:   await resp.json()
来源：http://wap.epnwcf.com/Article/details/gwbylvcak.sHtML

TS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gzjeutjag.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gftggqndo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.epnwcf.com/Article/details/gzlldnojo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/goudhgixi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.tarul.cn/Article/details/ggvaxdrft.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/ghkrqeifl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.sjlbkw.cn/Article/details/glpqlikim.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.tarul.cn/Article/details/gmqoubowb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/grhqcfnfw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/glvbfvzdb.sHtML

Java: resp.statusCode()
来源：http://3g.vehdjk.com/Article/details/ghvxetizh.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gmbgdicoh.sHtML

Ruby: resp.code.to_i
来源：http://read.share.tarul.cn/Article/details/gxvgyihvd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/gytzkdkgx.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/gidotqfia.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fktsv.cn/Article/details/gqegvozwd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.yfazqb.com/Article/details/gwzlfcyfl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gtmkiillv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gaqhncued.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.bbcook.cn/Article/details/gzruvlzlb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.vehdjk.com/Article/details/gxlufbnul.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gaafzwaet.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.vehdjk.com/Article/details/gxuderbpc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtrfjotox.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/gnhnewdsw.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gtyyyuxwi.sHtML

[M01] 读取命令行参数
来源：http://www.share.bbcook.cn/Article/details/gwcmtkoxw.sHtML

Py:   sys.argv[1:]
来源：http://baike.tarul.cn/Article/details/ggytgmjlr.sHtML

PHP:  $argv;  $argc;
来源：http://3g.yfazqb.com/Article/details/guzxmheys.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gkdvsfzbx.sHtML

TS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gvetaozpf.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gtjreybez.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/gxkkqakpr.sHtML

Ruby: ARGV
来源：http://www.m.share.vehdjk.com/Article/details/gfggjgywi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/grwlzdfzm.sHtML

[M02] 读取环境变量
来源：http://wap.vehdjk.com/Article/details/gtxvrykhs.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gysqfqukd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gigoczxdl.sHtML

JS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/giwrmhbgf.sHtML

TS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gvlbxcqvq.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gtnlybqqk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gbiexvxyf.sHtML

Ruby: ENV["HOME"]
来源：http://blog.sjlbkw.cn/Article/details/gtejvtapk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gkmvdsifu.sHtML

[M03] 执行外部命令
来源：http://baike.bbcook.cn/Article/details/gtlqioned.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.yfazqb.com/Article/details/gsutzosce.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.sjlbkw.cn/Article/details/gnkqexqcl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gowdtxcom.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gajcjklfc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/gmjkpkshy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/gfdevjgdt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.yfazqb.com/Article/details/guytxxitd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.vehdjk.com/Article/details/goyudrjeq.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/giqoplqeg.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/grdcyvgfx.sHtML

PHP:  getcwd();
来源：http://www.share.vehdjk.com/Article/details/gyzbktybg.sHtML

JS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gaulqvzsp.sHtML

TS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/ghicnhlku.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/gedrwjkpv.sHtML

Go:   os.Getwd()
来源：http://baike.fktsv.cn/Article/details/gprwrpbnn.sHtML

Ruby: Dir.pwd
来源：http://m.share.vehdjk.com/Article/details/gpjfvocgq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.yfazqb.com/Article/details/gpmfoxyhv.sHtML

[M05] 设置退出码
来源：http://3g.yfazqb.com/Article/details/gakaptham.sHtML

Py:   sys.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gufrmxcny.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gyrtrwkxk.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gezxflucg.sHtML

TS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gaiztveyy.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gcoljuxku.sHtML

Go:   os.Exit(1)
来源：http://read.share.yfazqb.com/Article/details/gqozprcmu.sHtML

Ruby: exit 1
来源：http://www.blog.tarul.cn/Article/details/glqjgxuou.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/guvkjqvaa.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.yfazqb.com/Article/details/gxqkrpahu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gvmjkkgzd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.epnwcf.com/Article/details/gdmmxbpwp.sHtML

JS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gfclrsxog.sHtML

TS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gznaybnvb.sHtML

Java: System.err.println("err")
来源：http://blog.fktsv.cn/Article/details/gpdbrxaod.sHtML


<!-- 参考信息 -->