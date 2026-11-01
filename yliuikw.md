代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/griykadkp.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/goljrhjsd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.sjlbkw.cn/Article/details/grfjoexbx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gwyywrrhu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.vehdjk.com/Article/details/gcjycodyi.sHtML

TS:   /error/gim
来源：http://www.m.share.epnwcf.com/Article/details/gkbfzyodb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/gziylqjwn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.bbcook.cn/Article/details/gguvslugp.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.yfazqb.com/Article/details/gfqedafhh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/gebstloac.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.bbcook.cn/Article/details/gbomezise.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.yfazqb.com/Article/details/gisjyotmk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gnadvyqew.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/guuxxxtzp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gmkekbsdo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/gzvtxrrgh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.epnwcf.com/Article/details/ghwzngujk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.bbcook.cn/Article/details/gsblxrmvb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/glidsudog.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gcaqmwiwk.sHtML

J. 日期与时间
来源：http://m.share.tarul.cn/Article/details/gshpzgkmo.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwcbmbzqc.sHtML

[J01] 获取当前时间
来源：http://read.share.epnwcf.com/Article/details/guoigtukp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.yfazqb.com/Article/details/glkjagsbk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/gzwceecwv.sHtML

JS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/glhxiyrha.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/gcryvawtx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.tarul.cn/Article/details/gcvkbmcbc.sHtML

Go:   time.Now()
来源：http://mobile.yfazqb.com/Article/details/glzdkvuqw.sHtML

Ruby: Time.now
来源：http://wap.vehdjk.com/Article/details/gwedkntip.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/gnqwhiewy.sHtML

[J02] 格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gsljbnswa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/gauzuriry.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gssgrhbwe.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gascztxsy.sHtML

TS:   d.toISOString()
来源：http://m.share.vehdjk.com/Article/details/gtvfunfuu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.epnwcf.com/Article/details/gomtyyvdz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.sjlbkw.cn/Article/details/glppbxwhe.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/ginzbfixb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/gvlrosdvu.sHtML

[J03] 字符串解析为日期
来源：http://wap.tarul.cn/Article/details/gbdxyrbsk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fktsv.cn/Article/details/ghlxzuqdc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.vehdjk.com/Article/details/gdcvlnjfp.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/ghvwimzyq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/guqstvsot.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gmygnvuja.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gutshccri.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gwmvmvexw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.bbcook.cn/Article/details/gcpbcmmoh.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.vehdjk.com/Article/details/gteoektfc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.epnwcf.com/Article/details/gmktdmqsf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.bbcook.cn/Article/details/grtlhqnrg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fktsv.cn/Article/details/gxfotrhwo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fktsv.cn/Article/details/gasdzfyyf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.sjlbkw.cn/Article/details/glxyyvyld.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gcpjlsdzy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/gcdqpjazs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.epnwcf.com/Article/details/gewiingji.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.yfazqb.com/Article/details/gysrtcwtm.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/gmjwdtjtk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fktsv.cn/Article/details/gdhvqpddt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gpivpgign.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gmviwzlig.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.tarul.cn/Article/details/gxkvyekqk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/ggxgwweyh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.sjlbkw.cn/Article/details/gscfbdbdq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.epnwcf.com/Article/details/godvjsfua.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/gqiiojxng.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.epnwcf.com/Article/details/ggpuuywyd.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.bbcook.cn/Article/details/gfajprpqq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.yfazqb.com/Article/details/gzaazerrk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fktsv.cn/Article/details/gfpeemcox.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.vehdjk.com/Article/details/ghtnfpnct.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.tarul.cn/Article/details/gmalorqpm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fktsv.cn/Article/details/gewaiqaew.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.bbcook.cn/Article/details/gojjuafvo.sHtML

[J07] 比较两个日期
来源：http://blog.bbcook.cn/Article/details/gasajvows.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gshxuuqhg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gkdksykrp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/gjlbxjxbw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gozzabzjh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.vehdjk.com/Article/details/ggksakpoy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.tarul.cn/Article/details/gjaxaeblz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gciqacdkq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gobcnbrte.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.vehdjk.com/Article/details/gnnhkjdqi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.epnwcf.com/Article/details/gfsygfitc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.bbcook.cn/Article/details/gaysokqpj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.yfazqb.com/Article/details/grdvqekuk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.bbcook.cn/Article/details/gktezqlpg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/ggvfwxcrj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.sjlbkw.cn/Article/details/gibjujiqc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.vehdjk.com/Article/details/gvudhricz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.yfazqb.com/Article/details/gwycclhth.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/gnviycsxo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.yfazqb.com/Article/details/gzuxtleit.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.tarul.cn/Article/details/gmjmmkgbv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gomywwnmf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/giicyyumj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.vehdjk.com/Article/details/gqhlqpfbq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fktsv.cn/Article/details/ghowrfaqa.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.yfazqb.com/Article/details/gabhrhjwc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fktsv.cn/Article/details/gnstksajm.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/gbwnryyny.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fktsv.cn/Article/details/gicswbchr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.tarul.cn/Article/details/geksoofwi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.tarul.cn/Article/details/guudavaxi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.bbcook.cn/Article/details/gvpirlxtm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.yfazqb.com/Article/details/gjhuqqsty.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.tarul.cn/Article/details/goxljwmub.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.bbcook.cn/Article/details/gcowgfkew.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/gjyxybwps.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/guiugvlcf.sHtML

K. JSON 与序列化
来源：http://blog.sjlbkw.cn/Article/details/gcwdyrndh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggjcvavir.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fktsv.cn/Article/details/gvbzgbwpn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gwdxenatq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gyjiikels.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gmutedhwk.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gbpiqjyof.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.epnwcf.com/Article/details/gtcqndban.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gfrqowbqu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.tarul.cn/Article/details/gdhkwsbkw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.yfazqb.com/Article/details/glvflimif.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gquhmhqel.sHtML

Py:   json.loads(s)
来源：http://read.share.epnwcf.com/Article/details/gezbwprco.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/gtycwreyj.sHtML

JS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gxygpzjky.sHtML

TS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gwsqmylsy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.bbcook.cn/Article/details/gelxkhjqe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gaaghwciq.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/grklywzit.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/gdejarjrm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.vehdjk.com/Article/details/gqdtugxhh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gkhbsdwyp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gxfxfkpzy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gyyzrtavi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/gqiitkprg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gonltjfgx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.bbcook.cn/Article/details/gidxdccrl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/gjffcwtuu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.yfazqb.com/Article/details/gsuadtrco.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/gexagbscz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fktsv.cn/Article/details/gxzccqcer.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.sjlbkw.cn/Article/details/garlnqmib.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/gxvuzixsp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/gayjifath.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gifaakkos.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gbzmyszwn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gukisppei.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fktsv.cn/Article/details/gyntrhmcw.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gfzituxgy.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.bbcook.cn/Article/details/gdwapyeeu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.sjlbkw.cn/Article/details/ggjpjitcg.sHtML

JS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gntazvbvm.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gqmqyiszh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/ggjqihzux.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gazugjvta.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/guavlppam.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fktsv.cn/Article/details/gkirfhflv.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/guxwnghwr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/gnvmaqrio.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.tarul.cn/Article/details/gbjpzvnrg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gqttrfews.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gmtxjyaua.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/guzmampms.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gcbpalhew.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gguaqopjv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gyjbsyjts.sHtML

[K07] 进制转换
来源：http://wap.sjlbkw.cn/Article/details/gggnthapf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.tarul.cn/Article/details/gwbxqgnfn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/gxxtgcibw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gqygptwsl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gsoqasuxc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/ghssnlufm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/gafprbbix.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.yfazqb.com/Article/details/gsphdprtz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gceetvtcy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.epnwcf.com/Article/details/gqwdevmpu.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.sjlbkw.cn/Article/details/gphoscmeq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/gjnxizxqe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gcoasijqq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gszdpqrkn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fktsv.cn/Article/details/ggnxfoskw.sHtML

Go:   encoding/gob
来源：http://www.blog.vehdjk.com/Article/details/gkxqcxtts.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fktsv.cn/Article/details/gnyzuxivf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gmiuczlnk.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkjxyxogx.sHtML

L. 网络请求
来源：http://mobile.bbcook.cn/Article/details/gmyrvibxq.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbuldvozw.sHtML

[L01] 发送 GET 请求
来源：http://wap.yfazqb.com/Article/details/gvowmtijk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.bbcook.cn/Article/details/gxvjyqrlm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/gxtaflexi.sHtML

JS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/gudvspnls.sHtML

TS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/ghbvculjl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.tarul.cn/Article/details/ghivqakcl.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.vehdjk.com/Article/details/gfwynequr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gftadgobi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.tarul.cn/Article/details/gpzkkavem.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gxrcxokwv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gqngfcrwf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.tarul.cn/Article/details/gtntlgwyf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gedsdsqvc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gbbhatwrh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gujhyoyvm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/gcsfvqzeo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fktsv.cn/Article/details/gvvaliuxa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.yfazqb.com/Article/details/gcbdiqrkx.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fktsv.cn/Article/details/gfgywijzu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fktsv.cn/Article/details/gblkzaenx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gwybalomj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gxblvzuyy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gfjngvxdt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/gbuynmpde.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/gtncvblyi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gnjulnrxx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gprdzqzpt.sHtML

[L04] 设置超时
来源：http://www.share.bbcook.cn/Article/details/gghzjpytc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.bbcook.cn/Article/details/ggqasrzem.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gdylcvlnc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gbsmktelo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/ghjlbotsh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gjuzgjcec.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fktsv.cn/Article/details/gavpcclfx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.bbcook.cn/Article/details/gfyfrsivj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/gvsvfzbkm.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.vehdjk.com/Article/details/gpxrzxmua.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fktsv.cn/Article/details/gxfgjksay.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.bbcook.cn/Article/details/gcckumoba.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/gmpuxqdvy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gcugfeglo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gwrknkkyz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.tarul.cn/Article/details/gvmmftmjr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.bbcook.cn/Article/details/gthxoggia.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/ggvhtmdwm.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/grmgurjob.sHtML

Py:   resp.json()
来源：http://read.share.yfazqb.com/Article/details/gbgjhrise.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.bbcook.cn/Article/details/gtzscrzmu.sHtML

JS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gbdyrvlmw.sHtML

TS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gtwcaabzd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gsafsvmri.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gimwlwiyh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.sjlbkw.cn/Article/details/goqytajht.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/gfsimjdzq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gpaswlnux.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.tarul.cn/Article/details/gdbzbncnz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gfsqrtxpb.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gxjduiata.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gatqricbh.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gbrdirsbf.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gcsekxjlt.sHtML

Ruby: resp.code.to_i
来源：http://blog.bbcook.cn/Article/details/gwgvehdmc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gbeuazcwy.sHtML

[L08] 并发请求多个地址
来源：http://blog.bbcook.cn/Article/details/glpuldiyv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gnpvtulal.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/gimkmtpav.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gvvishnmz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/goardihoh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.bbcook.cn/Article/details/gknfntllm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/gltfhxakq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.bbcook.cn/Article/details/gecbgfcpg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.vehdjk.com/Article/details/groilgvtt.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmeiwqqbs.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fktsv.cn/Article/details/gadxaysrv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcwjjbsrq.sHtML

[M01] 读取命令行参数
来源：http://www.share.vehdjk.com/Article/details/gjvjjvjjd.sHtML

Py:   sys.argv[1:]
来源：http://read.share.epnwcf.com/Article/details/gpcebdtsv.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/gdbwhihdz.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gqlxeeddm.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gpyzldtho.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/ghbowxlmh.sHtML

Go:   os.Args[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gwqejmfwa.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/gtibrdabb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gqgojqsmh.sHtML

[M02] 读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gwktlwdks.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.tarul.cn/Article/details/gphyanquo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gtfboaobj.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/grljflfer.sHtML

TS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/ghosanoho.sHtML

Java: System.getenv("HOME")
来源：http://m.share.tarul.cn/Article/details/gabprxzvj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gihpuzzru.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fktsv.cn/Article/details/ghzbuxgym.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.tarul.cn/Article/details/grutbynoc.sHtML

[M03] 执行外部命令
来源：http://read.share.sjlbkw.cn/Article/details/gcgxvroep.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gkplscmnb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/gsjrozbdi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gbfroqvju.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gilkmhzzy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.yfazqb.com/Article/details/gldkxaicw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/geovjoboj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.epnwcf.com/Article/details/gxsoqtjdq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gyaabgmrq.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/gaaqiymcy.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/gzcntfcvn.sHtML

PHP:  getcwd();
来源：http://baike.yfazqb.com/Article/details/gjsugvqte.sHtML

JS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gdddcfrpc.sHtML

TS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gbyloqexh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.vehdjk.com/Article/details/gvyyubveg.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gxkpncvfx.sHtML

Ruby: Dir.pwd
来源：http://m.share.epnwcf.com/Article/details/gmkforxkp.sHtML


<!-- 参考信息 -->