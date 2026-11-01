代发 wailian999

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/gcnxvkcqa.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gvobpufal.sHtML

[J01] 获取当前时间
来源：http://www.share.tarul.cn/Article/details/gzxtswsso.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.sjlbkw.cn/Article/details/gbtzdgwpg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gdgcuebjt.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gzxulqizv.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gelmrnrvn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/gmsblolxx.sHtML

Go:   time.Now()
来源：http://read.share.tarul.cn/Article/details/gpetvoftq.sHtML

Ruby: Time.now
来源：http://www.share.vehdjk.com/Article/details/gbyavjmyw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/goybudgcl.sHtML

[J02] 格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gvbirdlst.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gmhttqpkk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/gbagzspve.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.tarul.cn/Article/details/gmjodvhgn.sHtML

TS:   d.toISOString()
来源：http://baike.tarul.cn/Article/details/gyinuicbm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fktsv.cn/Article/details/gigigjdvh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fktsv.cn/Article/details/gppwxotle.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/gkmiopsyp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.sjlbkw.cn/Article/details/gxgwziemc.sHtML

[J03] 字符串解析为日期
来源：http://read.share.sjlbkw.cn/Article/details/gqbmrphry.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fktsv.cn/Article/details/gnyvyffdb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwifvvsbr.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/glsohdamt.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gdpqpuunl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gmxkkogoh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gtrqjshmm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gdttmuizz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.tarul.cn/Article/details/gcxxxhzaa.sHtML

[J04] 时间戳与日期互转
来源：http://baike.yfazqb.com/Article/details/gofusifiw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.yfazqb.com/Article/details/gqtgemuut.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fktsv.cn/Article/details/grhuihhik.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gtwwftfbk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gxceilbmr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.vehdjk.com/Article/details/gcbdmkmcx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/gpwqcqtox.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.epnwcf.com/Article/details/gyxqidqhz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/gzylfxrkp.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.epnwcf.com/Article/details/grrjcxqmg.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.vehdjk.com/Article/details/gplxusrtp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.epnwcf.com/Article/details/gmmlsagko.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/gouwwhopf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gcvsavnpu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.tarul.cn/Article/details/gknqjishw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gwqykvbmh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.bbcook.cn/Article/details/gtlliwawm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.epnwcf.com/Article/details/gnegwxdof.sHtML

[J06] 计算两时间之差
来源：http://www.share.bbcook.cn/Article/details/gwgqppvnl.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.bbcook.cn/Article/details/gfohjscex.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/grdrklhke.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.tarul.cn/Article/details/glpmjxhyq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.yfazqb.com/Article/details/guprujwft.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.tarul.cn/Article/details/gcozghkpm.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.bbcook.cn/Article/details/ggdvqfmzy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.tarul.cn/Article/details/gnwgaajkr.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.tarul.cn/Article/details/gjiadivgx.sHtML

[J07] 比较两个日期
来源：http://mobile.sjlbkw.cn/Article/details/grdwqtklh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/ghkeobgko.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gouqtwryj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/grrjhbmon.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gxwfdtjlg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fktsv.cn/Article/details/gqkkagbqs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.tarul.cn/Article/details/gdjyqozvc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gblxvlqpk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gbnqxezdx.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/giitdjzau.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fktsv.cn/Article/details/ggxwqusqu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.tarul.cn/Article/details/gmgujhbvv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.bbcook.cn/Article/details/gvngjaitl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.tarul.cn/Article/details/grmxvjavj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.yfazqb.com/Article/details/gmxeqfrzn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/gypnbmqva.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fktsv.cn/Article/details/gwilmeadi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.yfazqb.com/Article/details/gogcwfbxu.sHtML

[J09] 时区处理
来源：http://baike.tarul.cn/Article/details/gudmopyxj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/gonsfrbay.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/gyshqebzk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gtjnyfrla.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gfetjazql.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.yfazqb.com/Article/details/gbxlldosf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.tarul.cn/Article/details/gfpeykslj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.vehdjk.com/Article/details/gyxhstams.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/geveekben.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.vehdjk.com/Article/details/gysuzstzq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fktsv.cn/Article/details/gqvbcwraa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/gkrrujque.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.tarul.cn/Article/details/gaypjixob.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gkzbrzcoe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.sjlbkw.cn/Article/details/gmwmdmykb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fktsv.cn/Article/details/gpiyajvsp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.yfazqb.com/Article/details/glhhymbgq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fktsv.cn/Article/details/gnvogmiow.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/guudltkgn.sHtML

K. JSON 与序列化
来源：http://read.share.epnwcf.com/Article/details/ggrwjwrcq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gphjvgxhr.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.bbcook.cn/Article/details/giotnxlpq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gelzjpwnh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/guiueehpl.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/ggnrxynia.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gzisdzhfg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.epnwcf.com/Article/details/goqfndxbz.sHtML

Go:   json.Marshal(obj)
来源：http://baike.bbcook.cn/Article/details/geflssrdk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.sjlbkw.cn/Article/details/gafbzlwbh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.epnwcf.com/Article/details/gvskezspf.sHtML

[K02] JSON 字符串转对象
来源：http://baike.sjlbkw.cn/Article/details/gboehsbmj.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/gwxradzmt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gllvisvyf.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gpdglhvgl.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/ggzctwgvp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gggsjptav.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/ghctxbfuh.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gtrpaaras.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.yfazqb.com/Article/details/gqgxcmrie.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/gbbwjybdm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gdcpedrzn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/grtflrdqj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/ghmoovgac.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gamfvlguq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gzqyevnfl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.bbcook.cn/Article/details/glclcjsuf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.epnwcf.com/Article/details/gqfxigalr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.yfazqb.com/Article/details/gdolapada.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoecydag.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fktsv.cn/Article/details/gskkfiyzb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fktsv.cn/Article/details/gadeworyl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gakkypfov.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gulbihgfy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gdqfvgpcm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gakosknam.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.bbcook.cn/Article/details/glgowgkdh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.epnwcf.com/Article/details/gydxxsxix.sHtML

[K05] 深拷贝对象
来源：http://3g.bbcook.cn/Article/details/gxhdwatca.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/gvwmdupbp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/gabqgvchn.sHtML

JS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/ghxkhpxur.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/giulrpiuw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.sjlbkw.cn/Article/details/gmajtpfvi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/gtagomwqo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.tarul.cn/Article/details/gnljjdwdy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.yfazqb.com/Article/details/goymoffix.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gpwwmemce.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.vehdjk.com/Article/details/gxigmyagk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.epnwcf.com/Article/details/gxxfyeryz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/glfcrreyu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gpfsjgjlf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.vehdjk.com/Article/details/gtzjsmfjb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gfoersvfe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gmbwwnwhv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gjasndbdu.sHtML

[K07] 进制转换
来源：http://read.share.sjlbkw.cn/Article/details/guowpemsz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gxswjqtwc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.sjlbkw.cn/Article/details/gpkpfugkw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gbfvwibih.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gnlyddgow.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gfqvemmer.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/gtqghxhnj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fktsv.cn/Article/details/gjswbiskj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gngqliert.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/gexsbcrlt.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.tarul.cn/Article/details/gwdglfjcr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fktsv.cn/Article/details/gvpwyiczj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gddehzfsl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gdgnultwk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.yfazqb.com/Article/details/gixolxzrh.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/gzjoekqqb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkngtiylx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gdjtogcqg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grxaawrkh.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/gdobdfumw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gplbsrpkz.sHtML

[L01] 发送 GET 请求
来源：http://www.share.vehdjk.com/Article/details/gebzkctmq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fktsv.cn/Article/details/gtrwlcwgr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.epnwcf.com/Article/details/gtvvhnxoy.sHtML

JS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gohvhqiuy.sHtML

TS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gughzxoyn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/guuvqpxkq.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fktsv.cn/Article/details/grvruniqc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/goiiayyml.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fktsv.cn/Article/details/ghxazibjh.sHtML

[L02] 发送 POST JSON
来源：http://m.share.epnwcf.com/Article/details/glajgxyrh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gjqniwydl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fktsv.cn/Article/details/ghqcqhjdm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gwcibveer.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.bbcook.cn/Article/details/gvpytrrco.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gdvzylvon.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/gwmslxpcs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.yfazqb.com/Article/details/gnebbnaue.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.vehdjk.com/Article/details/gnxzeuhap.sHtML

[L03] 设置自定义请求头
来源：http://wap.vehdjk.com/Article/details/giklplsxi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fktsv.cn/Article/details/gjedlvcav.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/giqprgbcl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gbasnfjev.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gozbjpvis.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.sjlbkw.cn/Article/details/gjkzjnate.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gnggnmqes.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.yfazqb.com/Article/details/gyqmxifgk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gocbdmndh.sHtML

[L04] 设置超时
来源：http://www.m.share.tarul.cn/Article/details/glnooknzc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.tarul.cn/Article/details/gkyzkxmid.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/goexaaesl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gyzsqhqfc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gdezphobn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.bbcook.cn/Article/details/gtnzrpvbn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gbqvwizee.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.epnwcf.com/Article/details/ggihwdyzm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/ghtyxsqcg.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/gkxwpebph.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fktsv.cn/Article/details/gjicuivnt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gilzzxjbl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gxilutrpu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gmhngtxfr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.sjlbkw.cn/Article/details/gldbdbeis.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.tarul.cn/Article/details/gbmpsjpel.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.sjlbkw.cn/Article/details/gpzpssohk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.epnwcf.com/Article/details/gvhxmjzms.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gwdrozbaj.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gpnwvlcwx.sHtML

PHP:  json_decode($body, true);
来源：http://wap.tarul.cn/Article/details/gawzaroxs.sHtML

JS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/geyqznlhd.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gqkobnvkt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.epnwcf.com/Article/details/gaeoxabuh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.bbcook.cn/Article/details/gumiplqqz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.tarul.cn/Article/details/gujpsgbnv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/gjhfxbdqf.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gwymwwkvb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/gmxudzuwi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.epnwcf.com/Article/details/grdsmhdek.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gpdfkcjoj.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gfnhbugny.sHtML

Java: resp.statusCode()
来源：http://mobile.bbcook.cn/Article/details/giswymyti.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/geceunxfa.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fktsv.cn/Article/details/gqkgifsiv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gmsjevbss.sHtML

[L08] 并发请求多个地址
来源：http://baike.sjlbkw.cn/Article/details/gurpdpdgr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gdogkzudn.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.yfazqb.com/Article/details/guddtjpij.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gxcyqpbds.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gikejzird.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.sjlbkw.cn/Article/details/gpspaszrh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/gyqfeutpq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gqiywpcxd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.vehdjk.com/Article/details/ghewkfyki.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsdulxqot.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.tarul.cn/Article/details/gltkftvgd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gswjqzdrr.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gxqiealsa.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/gpfuypgnr.sHtML

PHP:  $argv;  $argc;
来源：http://blog.epnwcf.com/Article/details/gdkekfdnk.sHtML

JS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/girpctoga.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gbdmmfwiv.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gqdohocuk.sHtML

Go:   os.Args[1:]
来源：http://blog.yfazqb.com/Article/details/gaauhetav.sHtML

Ruby: ARGV
来源：http://www.blog.bbcook.cn/Article/details/gldtpktrd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gwqkpzeqz.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/gcnqxzltj.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/gkbpvkxic.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gwsbxmyiq.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/giknovffq.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gemwfkyle.sHtML

Java: System.getenv("HOME")
来源：http://mobile.yfazqb.com/Article/details/gtpojknri.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/gwbljzuhj.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/gmmlpsrsa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/gjpouvjao.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gkvyphpzq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.tarul.cn/Article/details/gnapohjdf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gswhvdqzl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/ghdmdbkof.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gibcltute.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/gswkezown.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/gywyqgppr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/gbtxdfjmp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.sjlbkw.cn/Article/details/gwaxykesl.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gxtbajoqn.sHtML

Py:   os.getcwd()
来源：http://m.share.tarul.cn/Article/details/gbrboxipc.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gjtrunenc.sHtML

JS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gjrommxuf.sHtML

TS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gkcbjnykz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.bbcook.cn/Article/details/grpsudnhk.sHtML

Go:   os.Getwd()
来源：http://www.blog.yfazqb.com/Article/details/grommghrw.sHtML

Ruby: Dir.pwd
来源：http://m.share.yfazqb.com/Article/details/gzoddlkqt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.tarul.cn/Article/details/gmlrdbcph.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/gnnzvnwjz.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/gofvhazas.sHtML

PHP:  exit(1);
来源：http://www.m.share.vehdjk.com/Article/details/gpdozljyk.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gmlioiroh.sHtML

TS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gkgvzagrp.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gwgczvgqx.sHtML

Go:   os.Exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gjbohznof.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gpdykxgng.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.vehdjk.com/Article/details/gfdjjqtxj.sHtML

[M06] 向标准错误输出
来源：http://3g.sjlbkw.cn/Article/details/giqmmyirv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gxjlbgbxq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/ggfulexbf.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gkoiveoli.sHtML

TS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gdrhugpfe.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gdsamaapk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.yfazqb.com/Article/details/gtahdglkq.sHtML

Ruby: warn "err"
来源：http://read.share.vehdjk.com/Article/details/gbhqukrsk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.sjlbkw.cn/Article/details/gnrkshpiy.sHtML

[M07] 判断是否为主入口
来源：http://m.share.epnwcf.com/Article/details/gvbkwwgje.sHtML


<!-- 参考信息 -->