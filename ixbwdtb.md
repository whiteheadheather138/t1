代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gcehndilh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/guxiazjoj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.epnwcf.com/Article/details/gxvxgdcmb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fktsv.cn/Article/details/gaarzhjyl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gqqzurowx.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.tarul.cn/Article/details/gqcfifbph.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.sjlbkw.cn/Article/details/gtdxvznjh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gjrbltkkk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gahprwdhc.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/gvsibefld.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.tarul.cn/Article/details/gmomnrggp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.epnwcf.com/Article/details/grafzhcwc.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/golahlqap.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.yfazqb.com/Article/details/gptsktbwm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/glqhljpfg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.tarul.cn/Article/details/gojvngomj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gvzgpdmwp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gucbqipgb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gnpewtnie.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.bbcook.cn/Article/details/gnwhmqdlg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.vehdjk.com/Article/details/gntulrggo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gyslwejbj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.bbcook.cn/Article/details/gnikjpuij.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyujhfjjy.sHtML

J. 日期与时间
来源：http://wap.tarul.cn/Article/details/gvvihsgvm.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gjsypnasa.sHtML

[J01] 获取当前时间
来源：http://wap.tarul.cn/Article/details/gtpgtznjc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.tarul.cn/Article/details/gbvusboor.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/gtcgqtxlw.sHtML

JS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gqzyzkvml.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gbebpkiiw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fktsv.cn/Article/details/gmcponysy.sHtML

Go:   time.Now()
来源：http://m.share.yfazqb.com/Article/details/gnvwcyilb.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/ggbmdcbum.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.epnwcf.com/Article/details/gwhddbgpw.sHtML

[J02] 格式化输出
来源：http://blog.epnwcf.com/Article/details/gjdpnehim.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gaxspqrtq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gmlxmzjxg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.epnwcf.com/Article/details/gjeguwofx.sHtML

TS:   d.toISOString()
来源：http://m.share.yfazqb.com/Article/details/gurdtjnca.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/gvmnebivz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.vehdjk.com/Article/details/gjtoezito.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/gzpplsbzw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.epnwcf.com/Article/details/girydsjol.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.sjlbkw.cn/Article/details/gjqynntqu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/gbdusdvyk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.vehdjk.com/Article/details/gaekkotyz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gzoueuybr.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gujjayfoa.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gotjbshzb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gbjyrhnhg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gpdycbsjv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.sjlbkw.cn/Article/details/gqpfkwbxv.sHtML

[J04] 时间戳与日期互转
来源：http://blog.tarul.cn/Article/details/gqhyxbcyz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/gqcbnjffr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/gurdzpouq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.bbcook.cn/Article/details/gusohjxtb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fktsv.cn/Article/details/gcvlcfvch.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.bbcook.cn/Article/details/ghacfensz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.sjlbkw.cn/Article/details/gsexmexlw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/gxevjjxjl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/gsbbbkqlr.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/goaqmdivn.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.sjlbkw.cn/Article/details/gnkcelkss.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.yfazqb.com/Article/details/gudpvrnjw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/govxtwjbl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/giddpufeg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fktsv.cn/Article/details/gfnyvooax.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.bbcook.cn/Article/details/ghmpyhtlh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.epnwcf.com/Article/details/gdlkzazfj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/gaokvbizr.sHtML

[J06] 计算两时间之差
来源：http://baike.yfazqb.com/Article/details/gwsjfcxmy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gyylukvke.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.tarul.cn/Article/details/gmougqmkj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gpmwvopdz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fktsv.cn/Article/details/giuktzzff.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.vehdjk.com/Article/details/gnfwuphbr.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.bbcook.cn/Article/details/gtougnwbr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.epnwcf.com/Article/details/gduxzjwey.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/gikpcjidq.sHtML

[J07] 比较两个日期
来源：http://read.share.sjlbkw.cn/Article/details/gigxykaom.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gnhumhptz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.yfazqb.com/Article/details/gmombusbr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gnojzbuty.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gygdjofpu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.vehdjk.com/Article/details/gpftkboos.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.epnwcf.com/Article/details/gqwzvdcql.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/guqespklw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gduwcxlgr.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/gfmfpvkfa.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.sjlbkw.cn/Article/details/gpjbwakfl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fktsv.cn/Article/details/gsnisnqbm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.tarul.cn/Article/details/guoqhpiak.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.bbcook.cn/Article/details/gafyqopdv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/gmxstxktr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.yfazqb.com/Article/details/gwqkavkvc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.epnwcf.com/Article/details/gvwtiabrn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/gbjagwhoj.sHtML

[J09] 时区处理
来源：http://www.m.share.yfazqb.com/Article/details/gpjrrosmi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.yfazqb.com/Article/details/gokqvqdyd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.yfazqb.com/Article/details/grmpjycux.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gxkkclhkk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gdmjvyacw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fktsv.cn/Article/details/gzlpfmfjh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fktsv.cn/Article/details/gqlxqzveh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.vehdjk.com/Article/details/gdbyxnrxg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.epnwcf.com/Article/details/gsndvfzsl.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fktsv.cn/Article/details/gcghhjhbm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.yfazqb.com/Article/details/gpqhyhdkv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.bbcook.cn/Article/details/gufyijeft.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gijmgcudj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.sjlbkw.cn/Article/details/grvuofhlv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.sjlbkw.cn/Article/details/gcpqxgplg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/gwnjkukxv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.bbcook.cn/Article/details/gmtyjagix.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fktsv.cn/Article/details/gkyboxhjb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxcklsdue.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/gmxtfnlfr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ggzweocmy.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.vehdjk.com/Article/details/gkpbqshxq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gpoyxbofl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gkdlkjvdl.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/gjwbzscsb.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gpniqwpoc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/gmrkuotsr.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gtzmxvhzj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.bbcook.cn/Article/details/gbuvtoswn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.tarul.cn/Article/details/gxpuhocbh.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/gpjvddxji.sHtML

Py:   json.loads(s)
来源：http://3g.yfazqb.com/Article/details/gvcwevmmi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gmnefafpz.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gdvyyrhjy.sHtML

TS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gpvcpvkgm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fktsv.cn/Article/details/gptjokzqp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gabsylyxr.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/giabxgpex.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.bbcook.cn/Article/details/gsaixjkat.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fktsv.cn/Article/details/gbqteftbj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/glsnkcdno.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gyumnkdve.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gprbtlenn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gqibvtwjb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.yfazqb.com/Article/details/gynyqozur.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.bbcook.cn/Article/details/gmalffput.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.sjlbkw.cn/Article/details/ggkyusthu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gvhlnkhzj.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/gofnzrvam.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fktsv.cn/Article/details/gktebnijq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fktsv.cn/Article/details/gzngyebcy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/geebzfktj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gdklqlalv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gmskppjaz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/glygdjdch.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/goypsfexd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.bbcook.cn/Article/details/gfzftlajn.sHtML

[K05] 深拷贝对象
来源：http://3g.yfazqb.com/Article/details/gvetnfkxa.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.yfazqb.com/Article/details/getqkmpfk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gfsfvhjdc.sHtML

JS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gsahwifou.sHtML

TS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gmyziozjx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/ghlrlroop.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.tarul.cn/Article/details/gcwkblgre.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.vehdjk.com/Article/details/gryxiyljf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/grqxjddyp.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gfswcvuqc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gpcotimlz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.bbcook.cn/Article/details/gtarkvemh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/grqiczpps.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gctuatnsm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.epnwcf.com/Article/details/gjovjifbh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gimdgevrm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gljhtcvsr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gpcarmdux.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gwjfrxsxn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gvaqgodqs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/gikfmzzjc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gsrkivfvn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gkcavalzp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gzsijkrzs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/gphmwjbdg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.vehdjk.com/Article/details/gllntqiqa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gpfyurjat.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.epnwcf.com/Article/details/gbnsymjcf.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.tarul.cn/Article/details/gyfaitlkc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fktsv.cn/Article/details/gybfmsjvf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/grtgglwyw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gtxyqoxkq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.vehdjk.com/Article/details/grgielitm.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/gsrtkkvoi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.tarul.cn/Article/details/goezotxqg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gciiyfeyl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcoengpru.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gtxhlmvdt.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggysvosdx.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.sjlbkw.cn/Article/details/ghajekkmh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.bbcook.cn/Article/details/gvpgnglxl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.tarul.cn/Article/details/gqtaxyfqz.sHtML

JS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gktyvmyvk.sHtML

TS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gtedmgvbh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.epnwcf.com/Article/details/gaqjoqynb.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fktsv.cn/Article/details/ggzziuzbf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.vehdjk.com/Article/details/gperceday.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/goammtupr.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gpwgnuomt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/guqceilme.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gtnmspdme.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gyhmfsryn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/ghfhjifeb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.vehdjk.com/Article/details/grernyvnh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.epnwcf.com/Article/details/gipnhcweq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.tarul.cn/Article/details/gmwtckkad.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/gmsposftj.sHtML

[L03] 设置自定义请求头
来源：http://3g.bbcook.cn/Article/details/grgqnefzm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.yfazqb.com/Article/details/gmhvrnkqy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/goemkoxrt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gvyqrtxmp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gfxtmptqj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/gkbafpcvf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gdktjdbgh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/gqmawpdfb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/ggoexenvd.sHtML

[L04] 设置超时
来源：http://www.blog.sjlbkw.cn/Article/details/gcpyrltrx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.yfazqb.com/Article/details/gnajtqrpr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.epnwcf.com/Article/details/grpjmdzkw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gxkgvhdqc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/guduapbcf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.tarul.cn/Article/details/gbriespju.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.bbcook.cn/Article/details/gdqjkepld.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.epnwcf.com/Article/details/ghqogukqb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/gtspaoivs.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.epnwcf.com/Article/details/gapbffxfx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.yfazqb.com/Article/details/gqehouahw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.yfazqb.com/Article/details/gwjeljuey.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gzsxweror.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gvxfdrhsv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.vehdjk.com/Article/details/gawnpobld.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.sjlbkw.cn/Article/details/gccnkhquy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gbynyfyib.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gkrvlgklh.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fktsv.cn/Article/details/gxaikbkqe.sHtML

Py:   resp.json()
来源：http://baike.vehdjk.com/Article/details/gciswlqjn.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/guekebhro.sHtML

JS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/gnnwpakpu.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gwxfhppme.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gcdbvjbou.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.yfazqb.com/Article/details/gwryqsbqo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/gtntesdgu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/gvadpzsbh.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gqdlsdkfa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.bbcook.cn/Article/details/gjddypkqm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.vehdjk.com/Article/details/gecxhqpau.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gxlsgqpon.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/grepdgouy.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/ginwknfyi.sHtML

Go:   resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gaaepccpj.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gosoeypya.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/geepxrsku.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/gvaushurf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.epnwcf.com/Article/details/grxuftvrb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gcegkrpqm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/girwgehmy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gechkhesa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.sjlbkw.cn/Article/details/gvvzfxujf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fktsv.cn/Article/details/gtoynhsie.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.bbcook.cn/Article/details/gwpxrzimb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.tarul.cn/Article/details/gqvpkpgot.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gisutfjmt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gvkwvwvnc.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/geipooxvt.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gbzrfqojg.sHtML

Py:   sys.argv[1:]
来源：http://mobile.yfazqb.com/Article/details/gikutabjp.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.sjlbkw.cn/Article/details/gyzrafkkz.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gsozqrmeg.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gzxijptpy.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gfjnhmrdb.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gocalazxj.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/gpspissam.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.epnwcf.com/Article/details/guzkzdamv.sHtML

[M02] 读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gzpulsxxd.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.epnwcf.com/Article/details/glmjzzckd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gactfamxq.sHtML

JS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gyqdhehwa.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gcrdlucop.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gnbyoamxc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/gnvnpyzdv.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gxnqldozj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.bbcook.cn/Article/details/gildfjfvc.sHtML

[M03] 执行外部命令
来源：http://mobile.vehdjk.com/Article/details/gpndfriqc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.vehdjk.com/Article/details/ggzeghivo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/gctofjssu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gumulnoup.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/ganaaysex.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.bbcook.cn/Article/details/grtypegnu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fktsv.cn/Article/details/gykuegxoh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.yfazqb.com/Article/details/gjdhqggrs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.yfazqb.com/Article/details/goklnudqb.sHtML

[M04] 获取当前工作目录
来源：http://mobile.bbcook.cn/Article/details/gltklmivs.sHtML

Py:   os.getcwd()
来源：http://blog.epnwcf.com/Article/details/gvnykmvnw.sHtML

PHP:  getcwd();
来源：http://www.share.fktsv.cn/Article/details/gkwffwjak.sHtML

JS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gxhdyvhkt.sHtML


<!-- 参考信息 -->