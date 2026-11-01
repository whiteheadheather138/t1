代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.epnwcf.com/Article/details/gcthxwfoc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gkbejeqjl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/ghgkvsgva.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.tarul.cn/Article/details/gxxaepycg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.sjlbkw.cn/Article/details/gkoqqjaeq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.epnwcf.com/Article/details/gorpoplof.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/guhqedtai.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqwtueaxb.sHtML

J. 日期与时间
来源：http://www.m.share.yfazqb.com/Article/details/gilzcmhlv.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdpmadyxh.sHtML

[J01] 获取当前时间
来源：http://read.share.fktsv.cn/Article/details/gmoprirxm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.yfazqb.com/Article/details/gqbzjgkvh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/gazljumfe.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/giaomgcyd.sHtML

TS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gaesnyrny.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.bbcook.cn/Article/details/gmljhevji.sHtML

Go:   time.Now()
来源：http://www.m.share.bbcook.cn/Article/details/gvxuudkkj.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/gfascyxbg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/gqgctmklz.sHtML

[J02] 格式化输出
来源：http://blog.bbcook.cn/Article/details/gaxoqnldt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.bbcook.cn/Article/details/gnnzfvymn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/ghtwuuddp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.tarul.cn/Article/details/ghgjxqjek.sHtML

TS:   d.toISOString()
来源：http://wap.yfazqb.com/Article/details/gkaafgeou.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fktsv.cn/Article/details/gkihsrzps.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/gblvzbtzq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gfaepksxc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.yfazqb.com/Article/details/gdfzecror.sHtML

[J03] 字符串解析为日期
来源：http://3g.vehdjk.com/Article/details/gxgklcdem.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/gzazisfpm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.tarul.cn/Article/details/gdmjtdojs.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gtwduotss.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gztaezxkk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gghhvcnwh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fktsv.cn/Article/details/ggrmnzenw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gnyklveyy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.sjlbkw.cn/Article/details/gqahssnad.sHtML

[J04] 时间戳与日期互转
来源：http://wap.tarul.cn/Article/details/gmieqthql.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.tarul.cn/Article/details/gmlbbbevf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.yfazqb.com/Article/details/gslatrgve.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gfvsavxul.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.epnwcf.com/Article/details/gstdtfkbl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gwgvfgxxt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fktsv.cn/Article/details/grpvoatnu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbanlrbi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.epnwcf.com/Article/details/golvokvow.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fktsv.cn/Article/details/gaeehfmby.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.sjlbkw.cn/Article/details/gisrleraz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/gpdlcmtxs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/gxngvtriy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gwnsycxto.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.vehdjk.com/Article/details/gyborvzvy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/grmwhliwf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.yfazqb.com/Article/details/gnnzptlhl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gzsaewgad.sHtML

[J06] 计算两时间之差
来源：http://blog.bbcook.cn/Article/details/gajvxqzpz.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.tarul.cn/Article/details/gpjrynvvx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.bbcook.cn/Article/details/gnlwkbbfw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.sjlbkw.cn/Article/details/glmpgforc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.vehdjk.com/Article/details/giculmvek.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/gzutehwsn.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.sjlbkw.cn/Article/details/gluiforgf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/giybzethm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.epnwcf.com/Article/details/gwtxexypu.sHtML

[J07] 比较两个日期
来源：http://3g.tarul.cn/Article/details/ghqsybvqf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gtuzwcdzq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.bbcook.cn/Article/details/gijwritui.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/gdgvclhis.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gkkymmfcv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.vehdjk.com/Article/details/gwpinjnry.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.epnwcf.com/Article/details/gdwaxcnlp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gryaloggh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gmqnjytao.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.yfazqb.com/Article/details/gnizwoplm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.vehdjk.com/Article/details/gtcwvliej.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.tarul.cn/Article/details/gebdpkqlu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.yfazqb.com/Article/details/gmdvamnla.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.epnwcf.com/Article/details/gegnzksbm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/ggcpqppzb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.epnwcf.com/Article/details/gosklditc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gncbsuxmp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.vehdjk.com/Article/details/gvzuhccfm.sHtML

[J09] 时区处理
来源：http://baike.bbcook.cn/Article/details/gxxaziuzk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.yfazqb.com/Article/details/ggyxazrmh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.epnwcf.com/Article/details/gattowncu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/gedhhmyow.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gobwgvnvn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.vehdjk.com/Article/details/gwurqohzc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.yfazqb.com/Article/details/glwgiwmga.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/gaifgvfkb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/gbafwlrxj.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/gydjyafod.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/gnsankzla.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/ghqcyurjn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.tarul.cn/Article/details/gipfyismi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fktsv.cn/Article/details/gralzxvom.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/giwvghldx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.epnwcf.com/Article/details/gotcswwec.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.sjlbkw.cn/Article/details/glpympfgf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.tarul.cn/Article/details/goayefxta.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gltejfong.sHtML

K. JSON 与序列化
来源：http://blog.yfazqb.com/Article/details/gkrytztgp.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfeoyatnz.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.vehdjk.com/Article/details/ghqgumklb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gvcowfdwb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/gyfaxuexz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/guamdocfr.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gzfhcsvwr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fktsv.cn/Article/details/gptgvvint.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gdvgrlxph.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.yfazqb.com/Article/details/ghmkvhzke.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.epnwcf.com/Article/details/gshxazxwv.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjotwfsj.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/gwqtfbgbs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fktsv.cn/Article/details/gitueyccj.sHtML

JS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gufyylymc.sHtML

TS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gqfbqpfse.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.yfazqb.com/Article/details/gksktwxfp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/gnfecodzu.sHtML

Ruby: JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gaimpnknz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fktsv.cn/Article/details/gmsoqfuhs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.tarul.cn/Article/details/gsaubwmhg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gpvdkpjce.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/grgyhshyk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/gaoqlyrht.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gxjzmmvpp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gioyuehbh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gggokjzkw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.vehdjk.com/Article/details/ggwkrstug.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.epnwcf.com/Article/details/gxvxatxxa.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/gknhizvow.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.vehdjk.com/Article/details/gamxunyuw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fktsv.cn/Article/details/gwjbrffod.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gnksgcvkn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gzitiwyij.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gmouwjnqo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gfzyapamt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.bbcook.cn/Article/details/glddgjjso.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gmtalmeee.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/gqxirmtuj.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.tarul.cn/Article/details/gqlqrkfsq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.sjlbkw.cn/Article/details/gpezcmlaz.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gyhglqnge.sHtML

TS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gbfeuywny.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/grhqfqssq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.epnwcf.com/Article/details/granxhjut.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.tarul.cn/Article/details/ggwfbdxyp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fktsv.cn/Article/details/ghrzvyohy.sHtML

[K06] 解析 URL 查询串
来源：http://wap.tarul.cn/Article/details/gffapkxzs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gkerznjxk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gsbgehayi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gfnapwyfu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/gznpaydeu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.bbcook.cn/Article/details/gifpxtcxw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/ggyjiyxfy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gzgcfnibj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gqrqqwxra.sHtML

[K07] 进制转换
来源：http://wap.tarul.cn/Article/details/gxikhnbtd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gigtyxqvx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/gsrpzqkoy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/galhosdeo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/glyxtxbao.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/glxutphmz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fktsv.cn/Article/details/gwyxpqyjg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gjdpqldee.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/glhicatff.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.bbcook.cn/Article/details/gcammlqit.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gvtqosmpq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fktsv.cn/Article/details/gkzcmpjnt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gpheusuog.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gtlzltyhx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.tarul.cn/Article/details/ggrbvlcss.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/gjrzwqbkh.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.sjlbkw.cn/Article/details/glntjvtet.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fktsv.cn/Article/details/gzlekyttz.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gbjajwmdu.sHtML

L. 网络请求
来源：http://wap.epnwcf.com/Article/details/gpafmjakr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzwpfkjsa.sHtML

[L01] 发送 GET 请求
来源：http://baike.bbcook.cn/Article/details/gkbayugiz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.bbcook.cn/Article/details/gxxobtgjw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.tarul.cn/Article/details/gzigpbtsq.sHtML

JS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/gxsefcrek.sHtML

TS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/gwphdowvw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/glnsjxagi.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/glqillsfb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/gdmcpncgq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.epnwcf.com/Article/details/gzxqduqya.sHtML

[L02] 发送 POST JSON
来源：http://baike.bbcook.cn/Article/details/gafqarlje.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gnytigfnq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.epnwcf.com/Article/details/gospkdexr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/geeukhicc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/gxiltszps.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gbsldtgqd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.epnwcf.com/Article/details/gmjzpobep.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fktsv.cn/Article/details/genaibezp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.sjlbkw.cn/Article/details/gifaamzug.sHtML

[L03] 设置自定义请求头
来源：http://mobile.vehdjk.com/Article/details/gkdujqckj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fktsv.cn/Article/details/gmsreqdrg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.epnwcf.com/Article/details/ghisrcnqt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gnkutcwfy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/gelntqqkz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/ghkvdyytq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gmmcekprp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.yfazqb.com/Article/details/gmfafauzq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gulvwckpx.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gzqzhimzk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.epnwcf.com/Article/details/gjdnnnphh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.bbcook.cn/Article/details/gqjcerjap.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gjwfyrkco.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/grkrwjvns.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.yfazqb.com/Article/details/guoboucpj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/gkjlrvcum.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.yfazqb.com/Article/details/gtzemlbic.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.tarul.cn/Article/details/gtvvpyyup.sHtML

[L05] 上传文件（multipart）
来源：http://blog.epnwcf.com/Article/details/gbbqnxgih.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.bbcook.cn/Article/details/gltgtqxjj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/gsrwtogzj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.tarul.cn/Article/details/gpwaovqwi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gpbdkqucy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.bbcook.cn/Article/details/gqeukozme.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.yfazqb.com/Article/details/gbfezqdec.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gzlmildrs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.vehdjk.com/Article/details/gfdxvnnij.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/gthvqzpzf.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/ggxmcsfpn.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gcwgfcvni.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gruxfmiwt.sHtML

TS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/grwfcfcdp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/grobqylcp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.epnwcf.com/Article/details/gmiujqknh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.yfazqb.com/Article/details/gkzhgjumg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/ghogshccw.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gngfpijkp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.yfazqb.com/Article/details/glqrilnky.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.tarul.cn/Article/details/gnkyitmqg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/glhpbvzgt.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gmxlguqsv.sHtML

Java: resp.statusCode()
来源：http://www.blog.tarul.cn/Article/details/gjqzllfyp.sHtML

Go:   resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/gtgfkuyaj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gdbqffwqg.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gymkirkdw.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.sjlbkw.cn/Article/details/gukazgeae.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.vehdjk.com/Article/details/gfgpnhhtl.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/gqgfvwcvm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gpvtboool.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gpsesnpfh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.tarul.cn/Article/details/grrcfbhqn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/gvrocekwj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gtmzjbhhw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/guzhreuty.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gztkcwyme.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gmemwrzoz.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/glmcpxwmn.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gctqfexdt.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gitnxpqww.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.tarul.cn/Article/details/ghaqcwdcr.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/glksmynyd.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gilgqcffs.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gjovckdyn.sHtML

Go:   os.Args[1:]
来源：http://read.share.vehdjk.com/Article/details/gsyncqaro.sHtML

Ruby: ARGV
来源：http://wap.fktsv.cn/Article/details/gtgbramsa.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gmeaiivgy.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gapyhkkrb.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/gqaxucent.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.yfazqb.com/Article/details/grrycwaze.sHtML

JS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gnnrhrfaf.sHtML

TS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gwjlhsyir.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/goxyfihsq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gplufyouz.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.yfazqb.com/Article/details/grilktivq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/goscyqdan.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/gwjbjcbqd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fktsv.cn/Article/details/gqpjhwygk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/gphfpgmfi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gxczhtoyw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gugndwmsk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.epnwcf.com/Article/details/gfogwprrl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.tarul.cn/Article/details/gkrsxckbb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.epnwcf.com/Article/details/gxnbxvqqk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.yfazqb.com/Article/details/gqdwjuelp.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.vehdjk.com/Article/details/guboxrelq.sHtML

Py:   os.getcwd()
来源：http://baike.vehdjk.com/Article/details/gzlrmnlvn.sHtML

PHP:  getcwd();
来源：http://www.blog.fktsv.cn/Article/details/gkhgkhnds.sHtML

JS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gejtkplmv.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gcevzotpg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fktsv.cn/Article/details/gdcxmannm.sHtML

Go:   os.Getwd()
来源：http://3g.tarul.cn/Article/details/gclrumhvp.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/gxxlbzhwu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.sjlbkw.cn/Article/details/gegqehmpy.sHtML

[M05] 设置退出码
来源：http://www.blog.yfazqb.com/Article/details/gxgamlnen.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gfgehztfn.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/gwyofydeb.sHtML

JS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gcsocpvfw.sHtML

TS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/grzwmvxnt.sHtML

Java: System.exit(1)
来源：http://3g.epnwcf.com/Article/details/gtafsehps.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/gqzcrasfa.sHtML

Ruby: exit 1
来源：http://mobile.sjlbkw.cn/Article/details/gpjxcjsoz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/guuekdamz.sHtML

[M06] 向标准错误输出
来源：http://mobile.bbcook.cn/Article/details/gpeijbtjl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gwjxwpijd.sHtML


<!-- 参考信息 -->